cmake_minimum_required(VERSION 3.23)
project(myApp)

find_package(OpenCV REQUIRED)

include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(a1 ./calcBackProject_Demo1.cpp)
add_executable(a2 ./calcBackProject_Demo2.cpp)
add_executable(a3 ./camshiftdemo.cpp)

target_link_libraries(a1 ${OpenCV_LIBS})
target_link_libraries(a2 ${OpenCV_LIBS})
target_link_libraries(a3 ${OpenCV_LIBS})
