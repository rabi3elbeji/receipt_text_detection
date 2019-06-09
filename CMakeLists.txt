cmake_minimum_required(VERSION 3.14)
project(receipt_text_detection)

set(CMAKE_CXX_STANDARD 14)

# Find OpenCV Package
find_package(OpenCV REQUIRED)



add_executable(receipt_text_detection main.cpp)
include_directories(receipt_text_detection ${OpenCV_INCLUDE_DIRS})
target_link_libraries(receipt_text_detection ${OpenCV_LIBS})