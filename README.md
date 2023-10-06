# C++ Standard Module Test

## About

This program uses the C++ standard module in for the typical "Hello, World!" application. CMake is used to build and install the executable file.

This program was created to provide a helpful example to other users of the basic configuration neccessary (at this time) for a simple application to employ the C++ standard module. Future versions will improve on the configuration.

## Copyright

This is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later
version. See the file COPYING.txt in this directory or [http://www.gnu.org/licenses/](http://www.gnu.org/licenses/), for a description of the GNU General Public License terms under which you can copy the files.

## Installation

The `CMakeLists.txt` file is setup to create two binary files: an executable and a static library file. The installion procedure using git is as follows:
```
mkdir <project_directory>
cd <project_directory>
git clone <PROJECT>
cd <PROJECT>
```
Although CMake provides an essentially system-independent build process, the procedures for compiling, building, and installing code using the C++ standard module may vary depending upon the system and compilier used.

The following procudure was employed for Windows (10), Visual Studio (17.7.4), and CMake (3.27.6). 

Edit the `CMakeLists.txt` file for you environment: set the `STD_MODULE_DIR` to the location of the file: `std.ixx` (Visual Studio example).

To compile, build, and install the executable release version, issue the following commands:
```
cmake -S . -B build
cmake --build build --config Release
cmake --install build --prefix .
```
The executable will be installed in `/bin` of the directory indicated by `--prefix`.

## Conclusion

Although the application is very simple, I hope this project has been helpful to someone needing to configure a project for employing the C++ standard module with CMake (3.27.6). The standard module is compiled with the main program - this is not ideal and future versions will improve on this.