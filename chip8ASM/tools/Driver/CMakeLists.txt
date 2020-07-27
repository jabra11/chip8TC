message("Building the driver for chip8ASM.")

set(src
    src/main.cpp
    )

add_executable(chip8ASM ${src})
target_link_libraries(chip8ASM 
                    PRIVATE
                    chip8ASM_Driver
                    fmt
                    )
