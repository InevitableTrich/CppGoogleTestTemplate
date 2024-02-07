cmake_minimum_required(VERSION 3.27)
project(tested_project)

set(CMAKE_CXX_STANDARD 17)
add_executable(${CMAKE_PROJECT_NAME}_run main.cpp)

set(CMAKE_CXX_FLAGS "-g")

include_directories(src)
add_subdirectory(src)

add_subdirectory(tests)

target_link_libraries(${CMAKE_PROJECT_NAME}_run)
