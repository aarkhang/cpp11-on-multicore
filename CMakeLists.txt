cmake_minimum_required(VERSION 3.12)

project(cpp11-on-multicore VERSION 1.0
                  DESCRIPTION "Various synchronization primitives for multithreaded applications in C++11"
                  LANGUAGES CXX)
                  
option(CPP11_ON_MULTICORE_BUILD_TESTS "Build tests" OFF)

add_subdirectory(common)
if(CPP11_ON_MULTICORE_BUILD_TESTS)
    add_subdirectory(tests)
endif()
