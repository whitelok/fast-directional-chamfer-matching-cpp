cmake_minimum_required(VERSION 3.2)

project(Fdcm VERSION 1.0 LANGUAGES CXX)

set(CMAKE_BUILD_TYPE "Debug")
set(CMAKE_CXX_FLAGS_DEBUG "$ENV{CXXFLAGS} -O0 -Wall -g -glldb")
SET(CMAKE_CXX_FLAGS_RELEASE "$ENV{CXXFLAGS} -O3 -Wall")

add_subdirectory(Fitline)
add_subdirectory(Image)
add_subdirectory(Fdcm)
