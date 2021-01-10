project(chip8ASM)

message("Building chip8ASM.")

add_subdirectory(lib)
add_subdirectory(tools)

add_library(chip8ASM_API INTERFACE)
target_include_directories(chip8ASM_API INTERFACE include)

install(DIRECTORY include/chip8ASM
    DESTINATION include
    )
