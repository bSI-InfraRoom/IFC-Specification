the concept of Group Spatial Connectivity allows for the association of a _IfcGroup_ (and its relevant subtypes) representing a grouping of objects to a particular spatial structure, either an entire facility (and its specific subtypes e.g. buildings, bridges, roads, or marine facilities), a facility part, a building storey, or any part of these structures.

The group (_IfcGroup_) in question should be human identifiable by its _Name_ attribute.

The relationship (_IfcRelReferencedInSpatialStructure_) in question can provide context of the connection through the _Name_ and _Description_ attributes.

The use of _IfcRelReferencedInSpatialStructure_ in this template provides the relationship across spatial and functional hierarchies allowing the spatial coverage of functional groups.

It is permissable for an IfcGroup not to be related to any spatial structure element. In the event that an IfcGroup (and its relevant subtypes) does not have a parent group through composition it must be related to the IfcProject using _Project declaration template_ via the IfcRelDeclares relationship.
