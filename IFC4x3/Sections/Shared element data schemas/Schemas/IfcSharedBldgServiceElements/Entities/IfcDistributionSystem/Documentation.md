A distribution system is a network designed to receive, store, maintain, distribute, or control the flow of a distribution media. A common example is a heating hot water system that consists of a pump, a tank, and an interconnected piping system for distributing hot water to terminals.  
The group _IfcDistributionSystem_ defines the occurrence of a specialized system for use within the context of building services or utilities for built facilities.  
Important functionalities for the description of a distribution system are derived from existing IFC entities:  
* <font color="#ff0000">From </font>_IfcSystem_<font color="#ff0000">  it inherits the ability to couple the built system via </font>_IfcRelReferencedInSpatialStructure_<font color="#ff0000">  to one or more </font>_IfcSpatialElement_<font color="#ff0000"> subtypes as necessary.</font>
* From _IfcGroup_ it inherits the inverse attribute IsGroupedBy, pointing to the relationship class _IfcRelAssignsToGroup_. This allows the grouping of distribution elements (instances of _IfcDistributionElement_ subtypes).
* From _IfcObjectDefinition_ it inherits the inverse attribute IsDecomposedBy pointing to the relationship class _IfcRelAggregates_. It provides the hierarchy between the separate (partial) distribution systems. For example, an electrical main circuit may be aggregated into branch circuits.

  
HISTORY New entity in IFC4.
