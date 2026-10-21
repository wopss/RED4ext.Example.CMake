cmake_minimum_required(VERSION 3.12)

# Change the project name here!
project(RED4ext.Example.CMake LANGUAGES CXX)

# Set this option to ON to be able to use folders / filters in your project when using Visual Studio.
set_property(GLOBAL PROPERTY USE_FOLDERS ON)

# Set the C++ standard to 20 (C++20).
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED YES)

# Add RED4ext.SDK as a dependency.
include(FetchContent)
include("${CMAKE_CURRENT_SOURCE_DIR}/cmake/deps/RED4extSdk.cmake")

# Include the main project.
add_subdirectory(src)
