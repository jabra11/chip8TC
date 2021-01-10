cmake_minimum_required(VERSION 3.14)
project(chip8TC)

set(CMAKE_CXX_STANDARD 20)

add_subdirectory(chip8ASM)
add_subdirectory(chip8LD)
add_subdirectory(chip8C)
