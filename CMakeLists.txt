cmake_minimum_required(VERSION 3.15)

project(slang_subproject_example)

find_package(slang 2.0.0)

add_executable(test main.cpp)
target_link_libraries(test PUBLIC slang::slang)