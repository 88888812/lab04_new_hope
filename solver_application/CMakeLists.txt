cmake_minimum_required (VERSION 3.4) 
project (solver)
set (CMAKE_CXX_STANDART 11)
set (CMAKE_CXX_STANDART_REQUIRED ON)
add_library  (solver STATIC ~/8888812/workspace/projects/lab03/solver_lib/solver.cpp
~/8888812/workspace/projects/lab03/formatter_ex_lib/formatter_ex.cpp
~/8888812/workspace/projects/lab03/formatter_lib/formatter.cpp)
include_directories (~/8888812/workspace/projects/lab03/solver_lib
~/8888812/workspace/projects/lab03/formatter_ex_lib
~/8888812/workspace/projects/lab03/formatter_lib)
add_executable (Solver ~/8888812/workspace/projects/lab03/solver_application/equation.cpp)
target_link_libraries(Solver solver)

