The _IfcRelAdheresToElement_ is an objectified relationship between an element and one surface feature element that that adheres to the surface on the element. The relationship is defined to be a 1:1 relationship, if an element has more than one surface feature, several relationship objects have to be used, each pointing to a different surface feature element. The _IfcRelAdheresToElement_ establishes an aggregation relationship between the main element and a sub ordinary surface feature.

> NOTE&nbsp; In contrary the _IfcRelAggregates_ relationship establishs an aggregation of equal parts to a whole.

The _IfcRelAdheresToElement_ implies a surface interface between the geometric bodies of the element and the surface feature . As with all decomposition relationships it determines:

* existence dependency - the _RelatedSurfaceFeature_ cannot exist without the _RelatingElement_
* hierarchical and non-cyclical relationship - the _IfcRelAdheresToElement_ can only alter a single _IfcElement_
* no spatial containment - the _IfcSurfaceFeature_ as related element never participates in the hiearchical spatial containment relationship _IfcRelContainedInSpatialStructure_

> HISTORY&nbsp; New entity in IFC4x3.
