cmake_minimum_required(VERSION 3.6)
project(thumbsim_sbem5)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(SOURCE_FILES
    inputs/bytetest.s
    inputs/bytetest.sim
    inputs/fib.s
    inputs/fib.sim
    inputs/shang.c
    inputs/shang.O0.s
    inputs/shang.O0.sim
    inputs/shang.O1.s
    inputs/shang.O1.sim
    inputs/shang.O2.s
    inputs/shang.O2.sim
    outputs/fib.completeoutput
    outputs/shang.O0.objdump
    outputs/shang.O1.completeoutput
    outputs/shang.O1.objdump
    outputs/shang.O2.completeoutput
    outputs/shang.O2.objdump
    outputs/shangO0.completeoutput
    outputs/shangO0.memstatscache.out
    test/gensimcode
    .gitignore
    decode.cpp
    execute.cpp
    LICENSE
    main.cpp
    Makefile
    parse.cpp
    README.md
    thumbsim.hpp
    thumbsim_driver.cpp)

add_executable(thumbsim_sbem5 ${SOURCE_FILES})