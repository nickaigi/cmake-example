cmake_minimum_required(VERSION 3.0)
project(test_cpp)

# set allows us to set variables and their corresponding values
set(CMAKE_BUILD_TYPE Debug)

# tell cmake that the code we are compilling uses c++ 14 syntax
# ${} interpolate  the value in the braces
set(CMAKE_CXX_FLAGS "-std=c++14 ${CMAKE_CXX_FLAGS}")

# first line, name of the executable we would like to produce
# followed by the source files to use to compile this program
add_executable(
    hello
    hello_world.cpp
)
