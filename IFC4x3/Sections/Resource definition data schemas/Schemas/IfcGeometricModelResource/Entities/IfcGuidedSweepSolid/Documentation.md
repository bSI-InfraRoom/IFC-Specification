An _IfcGuidedSweepSolid_ is asolid model constructed by sweeping along a directrix with boundaries defined by _GuidingCurves_.

The guiding curves shall correspond with the potentially varying _CrossSections_ that, in general, are placed on the _Directrix_ with _CrossSectionPositions_. The _CrossSections_ might diverge from the _GuidingCurves_ slightly and a consistency check is required by implementers.

As a rule, _CrossSectionPositions_ shall not feature longitudinal offsets.
