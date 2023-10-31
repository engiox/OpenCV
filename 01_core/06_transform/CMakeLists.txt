cmake_minimum_required(VERSION 3.24)

project(MyApp)

find_package(OpenCV REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(myapp BasicLinearTransforms.cpp)
add_executable(conbri contrast_brightness.cpp)
target_link_libraries(myapp ${OpenCV_LIBS})
target_link_libraries(conbri ${OpenCV_LIBS})
