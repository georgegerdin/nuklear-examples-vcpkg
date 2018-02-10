# nuklear-examples-vcpkg
The nuklear gui examples ported to work with vcpkg.

First install dependencies in vcpkg:
vcpkg install nuklear
vcpkg install glfw3
vcpkg install glew

Create a build directory:
mkdir build
cd build

Create visual studio solution file:
cmake .. -DCMAKE_TOOLCHAIN_FILE=C:\path\to\vcpkg\scripts\buildsystems\vcpkg.cmake"

