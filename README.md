# Simple example using onnxruntime with Conan

Code of the example comes from: https://github.com/cassiebreviu/cpp-onnxruntime-resnet-console-app

This is just an adaptation to manage the dependencies with Conan and also adding the [cmake-conan provider](https://github.com/conan-io/cmake-conan/tree/develop2) for CMake

## Building

```
cmake -DCMAKE_BUILD_TYPE=Release -DCMAKE_PROJECT_TOP_LEVEL_INCLUDES=conan_provider.cmake -S . -B ./build-release
cd build-release
cmake --build .
./onnxruntime_example
```
