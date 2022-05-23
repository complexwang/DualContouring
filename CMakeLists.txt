# Set the minimum version of CMake that can be used
# To find the cmake version run
# $ cmake --version
cmake_minimum_required(VERSION 3.5)

# Set the project name
project (DualContouring)

set(SOURCES
    code/eigen.h
    code/GeoCommon.h
    code/HashMap.h
	code/Intersection.h
    code/ModelReader.h
    code/octree.h
	code/PLYReader.h
    code/PLYWriter.h
	code/dc.cpp
	code/eigen.cpp
	code/octree.cpp
)

# Add an executable
add_executable(DualContouring ${SOURCES})
#add_executable(${PROJECT_NAME} main.cpp) 这样写也是可以的