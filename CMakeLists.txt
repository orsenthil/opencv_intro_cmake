cmake_minimum_required(VERSION 3.13)
project(opencv_sudoku)

set(CMAKE_CXX_STANDARD 14)

find_package( OpenCV REQUIRED )
add_executable( DisplayImage DisplayImage.cpp )
target_link_libraries( DisplayImage ${OpenCV_LIBS} )

