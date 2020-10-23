cmake_minimum_required(VERSION 3.0.0)
project(voronoi VERSION 1.0.0)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

file(GLOB ALL_SOURCE
    "src/*.cpp"
)

file(GLOB ALL_HEADERS
    "src/*.h"
)

include_directories(include)

add_library(voronoi ${ALL_SOURCE})

