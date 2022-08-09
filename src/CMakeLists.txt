cmake_minimum_required(VERSION 3.13)

project(patchelf VERSION 0.1.0)

set(CMAKE_CXX_STANDARD 17)
add_executable(patchelf
    patchelf.cc
    patchelf.h
    elf.h)
target_compile_definitions(patchelf PRIVATE -D_FILE_OFFSET_BITS=64)
