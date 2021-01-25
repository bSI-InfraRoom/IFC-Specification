{ .std}
The first Addendum of the IFC4 release has the main scope to provide documentation improvements, resolve issues that had occurred since the official release of IFC4 in March 2013, and to addresses implementation issues and concerns.

The main change incorporated into IFC4 ADD1 schema is:

\* Improvement and simplification of the explicit geometric representation of composite curves: addition of a new geometric item for indexed based poly curves. It requires the addition of the following entities and types: 
    \* entities _IfcIndexedPolyCurve_, _IfcCartesianPointList2D_
    \* select type _IfcSegmentIndexSelect_
    \* defined types _IfcArcIndex_, _IfcLineIndex_ 

Minor corrections and improvements to the IFC4 ADD1 schema include:

\* Use of defined types throughout the schema, i.e. using _IfcInteger_ instead of <eminteger, including the addition of _ifcbinary_
* use of the new type _ifcpositiveinteger_ to restrict the indices used e.g. for tessellated items to positive, one-based integers
* adding the missing attribute _longname_ to _ifcbuildingsystem_ in order to make it consistent with _ifcdistributionsystem_.
* promoting the inverse attribute _hascoverings_ from _ifcbuildingelement_ to _ifcelement_ to enable the inverse navigation also for _ifcdistributionelement_
* adding the inverse attribute _hascoordinateoperation_ to _ifcgeometricrepresentationsystem_ and _ifccoordinatereferencesystem_ to enable the inverse navigation to the gis coordinate transformation
* making the indespensible _name_ attribute mandatory at _ifccoordinatereferencesystem_ while making the _geodeticdatum_ optional
* changing the cardinality of the inverse attribute _definesoccurrence_ at _ifcpropertysetdefinition_ to allow property sets to be shared by many such relationships
* adding the where rule _nocoordoperation_ to _ifcgeometricrepresentationsubcontext_ to prevent the use of conflicting gis transformations of sub contexts
* adding the where rule _unboundedsurface_ to _ifcboxedhalfspace_ to prevent the use of bounded surfaces as clipping planes
* adding the where rule _uniquepropertysetnames_ at _ifcobject_ and _ifctypeobject_ to enforce property sets attached to a single object to have unique names
* remove the where rule _hasownerhistory_ at _ifcproject_ to enable model views not using owner history information
* remove the where rule _correctshapedecomposition_ at _ifcramp_, _ifcroof_, _ifcstair_ to enable model views to determine correct use of geometric shape representations including="" the="" addition="" of="" _ifcbinary_="" *="" use="" of="" the="" new="" type="" _ifcpositiveinteger_="" to="" restrict="" the="" indices="" used="" e.g.="" for="" tessellated="" items="" to="" positive,="" one-based="" integers="" *="" adding="" the="" missing="" attribute="" _longname_="" to="" _ifcbuildingsystem_="" in="" order="" to="" make="" it="" consistent="" with="" _ifcdistributionsystem_.="" *="" promoting="" the="" inverse="" attribute="" _hascoverings_="" from="" _ifcbuildingelement_="" to="" _ifcelement_="" to="" enable="" the="" inverse="" navigation="" also="" for="" _ifcdistributionelement_="" *="" adding="" the="" inverse="" attribute="" _hascoordinateoperation_="" to="" _ifcgeometricrepresentationsystem_="" and="" _ifccoordinatereferencesystem_="" to="" enable="" the="" inverse="" navigation="" to="" the="" gis="" coordinate="" transformation="" *="" making="" the="" indespensible="" _name_="" attribute="" mandatory="" at="" _ifccoordinatereferencesystem_="" while="" making="" the="" _geodeticdatum_="" optional="" *="" changing="" the="" cardinality="" of="" the="" inverse="" attribute="" _definesoccurrence_="" at="" _ifcpropertysetdefinition_="" to="" allow="" property="" sets="" to="" be="" shared="" by="" many="" such="" relationships="" *="" adding="" the="" where="" rule="" _nocoordoperation_="" to="" _ifcgeometricrepresentationsubcontext_="" to="" prevent="" the="" use="" of="" conflicting="" gis="" transformations="" of="" sub="" contexts="" *="" adding="" the="" where="" rule="" _unboundedsurface_="" to="" _ifcboxedhalfspace_="" to="" prevent="" the="" use="" of="" bounded="" surfaces="" as="" clipping="" planes="" *="" adding="" the="" where="" rule="" _uniquepropertysetnames_="" at="" _ifcobject_="" and="" _ifctypeobject_="" to="" enforce="" property="" sets="" attached="" to="" a="" single="" object="" to="" have="" unique="" names="" *="" remove="" the="" where="" rule="" _hasownerhistory_="" at="" _ifcproject_="" to="" enable="" model="" views="" not="" using="" owner="" history="" information="" *="" remove="" the="" where="" rule="" _correctshapedecomposition_="" at="" _ifcramp_,="" _ifcroof_,="" _ifcstair_="" to="" enable="" model="" views="" to="" determine="" correct="" use="" of="" geometric="" shape=""></eminteger, including the addition of _ifcbinary_
* use of the new type _ifcpositiveinteger_ to restrict the indices used e.g. for tessellated items to positive, one-based integers
* adding the missing attribute _longname_ to _ifcbuildingsystem_ in order to make it consistent with _ifcdistributionsystem_.
* promoting the inverse attribute _hascoverings_ from _ifcbuildingelement_ to _ifcelement_ to enable the inverse navigation also for _ifcdistributionelement_
* adding the inverse attribute _hascoordinateoperation_ to _ifcgeometricrepresentationsystem_ and _ifccoordinatereferencesystem_ to enable the inverse navigation to the gis coordinate transformation
* making the indespensible _name_ attribute mandatory at _ifccoordinatereferencesystem_ while making the _geodeticdatum_ optional
* changing the cardinality of the inverse attribute _definesoccurrence_ at _ifcpropertysetdefinition_ to allow property sets to be shared by many such relationships
* adding the where rule _nocoordoperation_ to _ifcgeometricrepresentationsubcontext_ to prevent the use of conflicting gis transformations of sub contexts
* adding the where rule _unboundedsurface_ to _ifcboxedhalfspace_ to prevent the use of bounded surfaces as clipping planes
* adding the where rule _uniquepropertysetnames_ at _ifcobject_ and _ifctypeobject_ to enforce property sets attached to a single object to have unique names
* remove the where rule _hasownerhistory_ at _ifcproject_ to enable model views not using owner history information
* remove the where rule _correctshapedecomposition_ at _ifcramp_, _ifcroof_, _ifcstair_ to enable model views to determine correct use of geometric shape representations>
