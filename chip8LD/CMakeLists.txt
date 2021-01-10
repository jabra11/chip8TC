project(chip8LD)

message("Building chip8LD.")

add_subdirectory(lib)
add_subdirectory(tools)


add_library(chip8LD_API INTERFACE)
target_include_directories(chip8LD_API INTERFACE include)

install(DIRECTORY include/chip8LD
    DESTINATION include
    )
