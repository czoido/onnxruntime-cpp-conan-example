cmake_minimum_required(VERSION 3.26)
project(onnxruntime_example)

set(CMAKE_CXX_STANDARD 17)

find_package(onnxruntime REQUIRED CONFIG)
find_package(OpenCV REQUIRED COMPONENTS core highgui imgproc CONFIG)

add_executable(onnxruntime_example main.cpp)
target_link_libraries(onnxruntime_example PRIVATE onnxruntime::onnxruntime opencv_core opencv_highgui opencv_imgproc)
