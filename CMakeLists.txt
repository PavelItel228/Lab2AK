cmake_minimum_required(VERSION 2.8)

project("lab2")
 
add_library(calculator STATIC calculator.cpp)
add_executable("${PROJECT_NAME}" main.cpp)

target_link_libraries("${PROJECT_NAME}" calculator)