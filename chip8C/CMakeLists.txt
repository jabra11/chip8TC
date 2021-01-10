project(chip8C)

message("Building chip8C.")

add_subdirectory(lib)
add_subdirectory(tools)

add_library(chip8C_API INTERFACE)
target_include_directories(chip8C_API INTERFACE include)

install(DIRECTORY include/chip8C
    DESTINATION include
    )
