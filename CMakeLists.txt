cmake_minimum_required(VERSION 3.13)
project(IntrusivePtr)

set(CMAKE_CXX_STANDARD 17)

add_library(intrusive_ptr STATIC
        src/ip/ref_counter.cpp
        src/ip/ref_counter.hpp
        src/ip/intrusive_ptr.hpp)
target_include_directories(intrusive_ptr PUBLIC src)