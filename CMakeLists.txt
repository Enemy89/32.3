cmake_minimum_required(VERSION 3.25)
project(untitled5)

set(CMAKE_CXX_STANDARD 17)

set(JSON_BuildTests OFF CACHE INTERNAL "")

add_subdirectory(nlohmann_json)

add_executable(untitled5 main.cpp)

target_link_libraries(untitled5 PRIVATE nlohmann_json::nlohmann_json)