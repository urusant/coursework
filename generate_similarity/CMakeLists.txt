cmake_minimum_required(VERSION 2.8)

set(CMAKE_CXX_FLAGS "-std=c++11 -g")
set(SOURCE_EXE generate_similarity.cpp)

include_directories(libs ../lib/)
add_subdirectory(../lib/ lib)

add_executable(gen ${SOURCE_EXE})

target_link_libraries(gen document)
