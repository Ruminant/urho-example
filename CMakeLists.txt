cmake_minimum_required(VERSION 3.0)
project(urho3d_example)

# Define target name
set (TARGET_NAME UrhoExample)

file(TO_CMAKE_PATH "$ENV{URHO3D_HOME}" URHO3D_HOME)
set (CMAKE_MODULE_PATH ${URHO3D_HOME}/share/CMake/Modules)
include (UrhoCommon)

#add_executable(urho3d_example main.cpp)
define_source_files (EXTRA_CPP_FILES main.cpp)
setup_main_executable()