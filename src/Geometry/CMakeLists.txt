ADD_LIBRARY(OpenEngine_Geometry
  Tests.h
  Tests.cpp
#  BoundingGeometry.h
  Box.h
  Box.cpp
  Sphere.h
  Sphere.cpp
  Line.h
  Line.cpp
  Ray.h
  Ray.cpp
  Plane.h
  Plane.cpp
  Square.h
  Square.cpp
  Face.h
  Face.cpp
  FaceSet.h
  FaceSet.cpp
  Material.h
  Material.cpp
  VertexArray.h
  VertexArray.cpp
  GeometrySet.h
  GeometrySet.cpp
  Vertex.h
  Mesh.h
  Mesh.cpp
  Light.h
)

TARGET_LINK_LIBRARIES(OpenEngine_Geometry
  OpenEngine_Math
  OpenEngine_Logging
  OpenEngine_Resources
)

IF(OE_BUILD_TESTS)
  SUBDIRS(tests)
ENDIF(OE_BUILD_TESTS)
