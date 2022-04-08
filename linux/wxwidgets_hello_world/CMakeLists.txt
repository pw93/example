# Set the minimum version of CMake that can be used
# To find the cmake version run
# $ cmake --version
cmake_minimum_required(VERSION 3.5)

# Set the project name
project (hello_cmake)

include_directories( "C:/msys64/mingw64/wxWidgets-3.1.6/include" )
include_directories( "c:/msys64/mingw64/wxWidgets-3.1.6/lib/wx/include/msw-unicode-3.1")


# Add an executable
add_executable(hello_cmake main.cpp)

target_link_libraries(hello_cmake
C:/msys64/mingw64/wxWidgets-3.1.6/lib/libwx_mswu_core-3.1.dll.a
C:/msys64/mingw64/wxWidgets-3.1.6/lib/libwx_baseu-3.1.dll.a
)
