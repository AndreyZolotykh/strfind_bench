cmake_minimum_required(VERSION 3.21)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_BUILD_TYPE "Debug")
project(bench)
find_package(benchmark REQUIRED)
add_executable(
    strfind_bench
    bench.cpp)
target_link_libraries(strfind_bench benchmark::benchmark)