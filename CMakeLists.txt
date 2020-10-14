cmake_minimum_required(VERSION 3.16) 

project("HelloWorld" VERSION 0.1)
add_library(libraryCalc STATIC calculator.cpp)
add_executable("${PROJECT_NAME}" main.cpp)
target_link_libraries("${PROJECT_NAME}" libraryCalc)	
