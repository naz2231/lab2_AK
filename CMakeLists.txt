cmake_minimum_required(VERSION 3.16.3)

project("lab2_AK" VERSION 0.1)
 
add_library(mycalculator STATIC calculator.cpp)
add_executable("${PROJECT_NAME}" main.cpp)
target_link_libraries("${PROJECT_NAME}" mycalculator)