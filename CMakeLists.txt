cmake_minimum_required(VERSION 3.21)

# Set the project name
project(cpp-engine)

# Specify the C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Add include directory
include_directories(include)

# Add all the source files in the src directory
file(GLOB SOURCES "src/*.cpp")

# Add the executable
add_library(${PROJECT_NAME} STATIC ${SOURCES})