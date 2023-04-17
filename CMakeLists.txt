cmake_minimum_required(VERSION 3.0.0)

project(third-party-libs CXX)

find_package(tsl-robin-map REQUIRED)
find_package(fmt REQUIRED)

add_executable(main main.cpp)
target_link_libraries(main PRIVATE tsl::robin_map fmt::fmt)
