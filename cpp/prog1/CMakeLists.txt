# CMakeList.txt : CMake project for prog3, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.8)

project ("prog1")

find_package(fmt CONFIG REQUIRED)

# Add source to this project's executable.
add_executable (prog1 "prog1.cc" "prog1.h")
target_link_libraries(prog1 PRIVATE fmt::fmt)
