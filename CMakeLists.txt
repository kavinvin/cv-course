cmake_minimum_required(VERSION 3.9)
project(cv)

set(CMAKE_CXX_STANDARD 17)

add_executable(cv main.cpp)

find_package( OpenCV REQUIRED )
target_link_libraries( cv ${OpenCV_LIBS} )