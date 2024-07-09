cmake_minimum_required(VERSION 3.29)
project(backend LANGUAGES C CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

add_subdirectory(framework)

add_executable(blog src/main.cc)
target_link_libraries(blog framework)

option(ENABLE_TESTS "Enable Google Test suites" On)

if(ENABLE_TESTS)
	add_subdirectory(test)
endif()
