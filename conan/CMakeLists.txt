cmake_minimum_required(VERSION 3.2)
project(testConanPackageManager)

set(CMAKE_CXX_STANDARD 14)
set (CMAKE_CXX_FLAGS "-Werror -Wall -Wextra -Wpedantic")


include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
conan_basic_setup()

add_executable(formater src/main.cpp)
target_link_libraries(formater ${CONAN_LIBS})