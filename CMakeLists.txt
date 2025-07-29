cmake_minimum_required(VERSION 3.15)
project(demo-vcpkg-project)

# Enable CMake integration with vcpkg
find_package(fmt CONFIG REQUIRED)

add_executable(main main.cpp)
target_link_libraries(main PRIVATE fmt::fmt)