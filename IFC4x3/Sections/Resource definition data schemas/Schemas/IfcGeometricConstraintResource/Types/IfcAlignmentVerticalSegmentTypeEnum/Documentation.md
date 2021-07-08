The IfcAlignmentVerticalSegmentTypeEnum indicates the type of a segment of a vertical alignment segment (IfcAlignmentVerticalSegment).


| Vertical curvature | Segmenttype        | Enumeration Values |
|:----|:------------------|:----------|
| No vertical curvature | constant gradient        | CONSTANTGRADIENT |
| Derivative of gradient with respect to chainage is constant | Vertical curve, parabola  | PARABOLICARC |
| Derivative of vertical angle with respect to sloping length along the track is constant | Vertical curve, circular | CIRCULARARC  |
| variation of vertical curvature is constant | Vertical clothoid curve | CLOTHOID  |



NOTE A vertical curve in track that starts or ends in canted switches and crossings can be of a higher order polynomial than a parabola.


**Used Symbols and their meaning**


| Symbol | meaning  | Unit, value range |
|:----|:------------------|:----------|
| L | full length of segment        | positive length  L > 0 |
| s | current position on segment        | 0 < s < L |
| &theta; | (Greek "theta") gradient; Longitudinal slope angle (incline or decline)   | rad |
| x(s) | variable longitudinal coordinate of the projection of the alignment / track centreline into the ground plan.  | length |
| y(s) | variable transverse coordinate of the projection of the alignment / track centreline into the ground plan.  | length |
| z(s) | Variable vertical coordinate of the projection of the track centreline in plan in a Cartesian coordinate system in the vertical direction.  | length |
| z<sub>c</sub>(s) | Ordinate of the vertical circular arc of measured away from the tangent line at position s.  | length |
| L<sub>V</sub> | length of vertical radius radius (inverse curvature)  | length |
| R<sub>V</sub> | radius (inverse curvature) of the track centreline at a point in the elevation diagram (longitudinal section)  | length |
| Z<sub>G</sub> | Distance of the tangent intersection from the chord of the vertical circular arc  | length |
| Z<sub>M</sub> |  Distance of the centre of the vertical circular arc to the tangent intersection point (stitch height) | length |
| l<sub>T</sub> | Length of the tangents of the  vertical circular arc | length |

&gt;NOTE Symbols according to EN 13803/2017
