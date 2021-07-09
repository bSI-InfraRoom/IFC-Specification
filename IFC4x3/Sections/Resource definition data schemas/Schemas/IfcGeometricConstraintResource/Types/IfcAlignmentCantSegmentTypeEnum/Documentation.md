The IfcAlignmentCantSegmentTypeEnum indicates the type of a segment of a cant alignment segment (IfcAlignmentCantSegment). 

Cant is an important aspect in modern track design.



| Curvature | Segmenttype        | Enumeration Values |
|:----|:------------------|:----------|
| 0 |  both rails without relative elevation        | CONSTANTCANT  |
| constant in the complete segment, <> 0 | elevated rail  | CONSTANTCANT |
| variation along the segment | Transition with linear cant variation | LINEARTRANSITION   |
| variation along the segment | Transition with non-linear cant variation | HELMERTCURVE, BLOSSCURVE, COSINECURVE, SINECURVE, VIENNESEBEND |





**Used Symbols and their meaning**

| Symbol | meaning  | Unit, value range |
|:----|:------------------|:----------|
| L | full length of segment        | positive length  L > 0 |
| s | current position on segment        | 0 < s < L |
| &xi;  |  = s / L  (Greek "xi") standardised, dimensionless path length along the alignment / track centre line        | 0 < &xi; < 1 |
|  D |  cant .... amount by which one running rail is raised above the other running rail, in a track cross section         | length  |
| D<sub>1</sub> | cant at beginning of the alignment segment        | length  |
| D(s) | variable cant at station "s" along the alignment cant segment.  | length |
| &psi; | (Greek "psi") Angle of cant (cross slope angle, bank angle)        | rad |
| &phi; | (Greek "phi") Directional angle (azimuth, bearing)  | rad |

**Terminology**

**Intrinsic coordinate, intrinisc coordinate system of an alignment segment:**

The origin of an intrinsic coordinate system is the start of the segment. The direction of the positive x-axis is the startdirection of the segments.
