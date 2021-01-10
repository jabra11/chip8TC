message("Building the driver for chip8ASM.")

set(src
    src/main.cpp
    )

add_executable(chip8C ${src})
target_link_libraries(chip8C 
                    PRIVATE
                    chip8C_Driver
                    fmt
                    )

install(TARGETS chip8C
    RUNTIME DESTINATION bin
    )
