cmake_minimum_required(VERSION 3.29)
project(framework LANGUAGES C CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

add_library(framework src/framework.cc)
target_include_directories(framework PUBLIC include)

