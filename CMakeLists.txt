cmake_minimum_required(VERSION 3.0.0)

project(testCMakeTOS7 VERSION 1.0 LANGUAGES CXX C)

add_executable(testCMakeTOS7 src/main.cpp)

set(CMAKE_SYSTEM_NAME Linux)

set_target_properties(testCMakeTOS7 PROPERTIES
    RUNTIME_OUTPUT_DIRECTORY "bin"
    ARCHIVE_OUTPUT_DIRECTORY "lib"
    LIBRARY_OUTPUT_DIRECTORY "lib"
)
