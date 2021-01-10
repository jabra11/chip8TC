message("Building the driver for chip8LD.")

set(src
    src/main.cpp
    )

add_executable(chip8LD ${src})
target_link_libraries(chip8LD
                    PRIVATE
                    chip8LD_Driver
                    fmt
                    )

install(TARGETS chip8LD
    RUNTIME DESTINATION bin
    )
