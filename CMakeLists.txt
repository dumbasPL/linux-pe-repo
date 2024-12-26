cmake_minimum_required(VERSION 3.15)

project(linux-pe-repo LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_subdirectory(linux-pe)

add_executable(linux-pe-repo main.cpp)
target_link_libraries(linux-pe-repo PRIVATE linux-pe)