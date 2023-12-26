cmake_minimum_required(VERSION 3.15)

project(slang_subproject_example)

find_package(slang 5.0.0)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

add_executable(test main.cpp)
target_link_libraries(test PUBLIC slang::slang)
