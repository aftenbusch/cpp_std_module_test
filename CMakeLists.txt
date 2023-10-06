#
# project cpp_std_module_test
#
cmake_minimum_required(VERSION 3.27)
#
set(CMAKE_CXX_STANDARD 23)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
#
# Edit file location for your specific environment:
#
set(STD_MODULE_DIR "C:/Program Files/Microsoft Visual Studio/2022/Community/VC/Tools/MSVC/14.37.32822/modules")
#
project(cpp_std_module_test VERSION 1.0 DESCRIPTION "C++ Standard Module Test" LANGUAGES CXX)
#
add_executable(cpp_std_module_test)
target_sources(cpp_std_module_test PRIVATE src/main.cpp ${STD_MODULE_DIR}/std.ixx)
install(TARGETS cpp_std_module_test DESTINATION bin)
#