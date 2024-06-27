cmake_minimum_required(VERSION 3.22.1)
project(Cryogen)

add_library(cryogen SHARED native-lib.cpp)

find_library(log-lib log)
target_link_libraries(cryogen ${log-lib})