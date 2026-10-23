cmake_minimum_required(VERSION 3.20)
project(dedupli LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)  # for clangd / editor tooling

add_executable(dedupli src/main.cpp)
target_compile_options(dedupli PRIVATE -Wall -Wextra -Wpedantic)
