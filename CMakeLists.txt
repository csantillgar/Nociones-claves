cmake_minimum_required(VERSION 3.26)
project(untitled)

set(CMAKE_CXX_STANDARD 17)

# Agrega los ejecutables y vincula las bibliotecas apropiadas
add_executable(main main.cpp)
add_library(persona STATIC persona.cpp)
add_library(estudiante STATIC estudiante.cpp)

# Enlaza las bibliotecas con los ejecutables correspondientes
target_link_libraries(main persona estudiante)
