cmake_minimum_requited (VERSION 3.4)
set (CMAKE_CXX_STANDARD 11) 
set (CMAKE_CXX_STANDARD_REQUIRED ON ) 
project (solver_lib)
add_library (solver_lib STATIC solver.cpp)

