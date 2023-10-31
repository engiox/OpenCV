cmake_minimum_required(VERSION 3.23)
project(myApp)

message(Build type : "${CMAKE_BUILD_TYPE}")

find_package(OpenCV REQUIRED)

include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(myapp ./how_to_use_OpenCV_parallel_for_new.cpp)

target_link_libraries(myapp ${OpenCV_LIBS})
