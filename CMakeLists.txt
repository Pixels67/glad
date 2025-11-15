cmake_minimum_required(VERSION 3.5)
project(glad)

set(CMAKE_C_STANDARD 90)

add_library(${PROJECT_NAME} STATIC src/glad.c include/glad/glad.h include/KHR/khrplatform.h)
target_include_directories(${PROJECT_NAME} PUBLIC include)