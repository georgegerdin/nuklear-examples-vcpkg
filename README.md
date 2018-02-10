# nuklear-examples-vcpkg
The nuklear gui examples ported to work with vcpkg including ports of unistd.h, getopt.h, getopt.c and dirent.h for the file_browser example.

## Building

First install dependencies in vcpkg:
```
vcpkg install nuklear
vcpkg install glfw3
vcpkg install glew
```



Create a build directory and enter it:
```
mkdir build && cd build
```


Create visual studio solution file:
```
cmake .. -DCMAKE_TOOLCHAIN_FILE=C:\path\to\vcpkg\scripts\buildsystems\vcpkg.cmake"
```

Open in visual studio and run with Start Debugging (F5) or Start without Debugging (Ctrl+F5).