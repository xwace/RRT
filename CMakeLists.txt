cmake_minimum_required(VERSION 3.23)
project(RRT)

set(CMAKE_CXX_STANDARD 14)
find_package(OpenCV REQUIRED)
include_directories( ${OpenCV_INCLUDE_DIRS})
aux_source_directory(./ EXEFILES)
add_executable(RRT ${EXEFILES})
target_link_libraries(RRT ${OpenCV_LIBS})

