The _IfcRelInterferesElements_ objectified relationship indicates that two elements interfere. Interference is a spatial and/or shape interaction between the two elements. It is a 1 to 1 relationship. The concept of two elements interfering physically or logically is described independently from the elements. The interference may be related to the shape representation of the entities by providing an interference geometry.  
  
* When the interference geometry is available it can be passed by the optional attribute _InterferenceGeometry_ pointing to _IfcConnectionGeometry_. The connection geometry is provided as a point, curve, surface, or solid within the placement coordinate systems of the connecting elements. The _IfcConnectionVolumeGeometry_ is the default type to be used for interference in 3D space, as indicated in e.g. clash detections.  
* If the interference geometry is omitted then the interference is provided as a logical relationship. Under this circumstance, the connection point, curve, surface, or solid has to be recalculated by the receiving application.  
  
The _RelatingElement_ and _RelatedElement_ define the two elements in the relationship, that may have different roles. The relation orientation may be required by certain _InterferenceType_ values, this is done  by setting the attribute _ImpliedOrder_ accordingly:
  
* _ImpliedOrder_=TRUE The _RelatingElement_ constitutes the primary element of the interference relationship that is oriented from _RelatingElement_ (source) to _RelatedElement_ (target). If the interference is to be resolved by subtracting the overlapping part, it should be subtracted from the _RelatingElement_. The net result would be the _RelatingElement_ subtracted by the _InterferenceGeometry_. This would be the case in interference relationships where the _RelatedElement_ creates a void in the _RelatingElement_ dynamically.  
* _ImpliedOrder_=FALSE The _RelatingElement_ and _RelatedElement_ have no priority among each other. If the interference is to be resolved then no information about whether the _InterferenceGeometry_ should be subtracted from the _RelatingElement_ or the _RelatedElement_ can be traced. This would be the case for clash detection results.  
* _ImpliedOrder_=UNKNOWN No information about the priorities is provided.  
 
The _InterferenceGeometry_ attribute is used to define the physical interference shape, it can be part of the shape of one of the elements of the relationship or define the interface between the two shapes.
The _InterferenceSpace_ attribute is used to define the spatial interference space, expressed by a specific _IfcSpatialZone_ of predefined type INTERFERENCE.

The _InterferenceType_ property optionally specifies the type of interference between the two elements, two set of default types are provided:
* **Oriented interferences types** imply usage of _ImpliedOrder_ set to TRUE and specific choice of _RelatingElement_ and _RelatedElement_ to be meaningful:
  * Crosses: the _RelatingElement_ is crossing the _RelatedElement_ (e.g. Railway crossing a road)
  * PassesThrough: the _RelatingElement_ is passing through the _RelatedElement_ (e.g. a Road passing inside a tunnel)
  * PassesOver: the _RelatingElement_ is passing over the _RelatedElement_ (e.g a bridge passing over a water canal)
  * PassesUnder: the _RelatingElement_ is passing under the _RelatedElement_ (e.g a Pipe passing under a road)
* **Non oriented interferences types** do not imply specific values of _ImpliedOrder_ (but can still be set to detail shape interference calculation)
  * Clash: The _RelatingElement_ and _RelatedElement_ have a spatial or shape-based clash
  * Along: The _RelatingElement_ and _RelatedElement_ have a common frontier/surface
 
> HISTORY&nbsp; New entity in IFC4.
