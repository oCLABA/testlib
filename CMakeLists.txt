cmake_minimum_required(VERSION 3.17)
project(testlib)

set(CMAKE_CXX_STANDARD 14)
set(SFML_STATIC_LIBRARIES TRUE)
set(SFML_DIR "C:/Users/pashi/Documents/SFML-2.5.1-windows-gcc-7.3.0-mingw-64-bit/SFML-2.5.1/lib/cmake/SFML")

find_package(SFML REQUIRED system window graphics network)
add_executable(testlib main.cpp)
target_link_libraries(testlib sfml-graphics sfml-window sfml-system)
