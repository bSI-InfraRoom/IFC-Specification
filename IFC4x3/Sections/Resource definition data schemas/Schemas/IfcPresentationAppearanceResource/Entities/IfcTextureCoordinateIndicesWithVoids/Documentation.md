The _IfcTextureCoordinateIndicesWithVoids_ is a subtype of _IfcTextureCoordinateIndices_ to be used to provide texture coordinates to polygonal faces with inner loops. The two dimensional list of _TexCoordIndex_ holds the indices into the _IfcTextureVertexList_ that correspond to the list of _CoordIndex_ at _TexCoordsOf_ where:

- the first dimension corresponds to the list position of the inner loops at _IfcIndexedPolygonalFaceWithVoids_ referenced by _TexCoordsOf_
- the second dimension corresponds to the list position of the vertices at the n-th inner loop at _IfcIndexedPolygonalFaceWithVoids_

>HISTORY New entity in IFC4.3.0.0
