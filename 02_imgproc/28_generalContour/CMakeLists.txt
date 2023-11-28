cmake_minimum_required(VERSION 3.23)
project(myApp)

find_package(OpenCV REQUIRED)

include_directories(${OpenCV_INCLUDE_DIRS})

#add_executable(a ./generalContours_demo1.cpp)
add_executable(b ./generalContours_demo1mod.cpp)

#target_link_libraries(a ${OpenCV_LIBS})
target_link_libraries(b ${OpenCV_LIBS})