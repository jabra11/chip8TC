message("Building the driver for chip8C.")

set(src
    src/main.cpp
    )

add_executable(chip8C ${src})
target_link_libraries(chip8C
                    PRIVATE
                    Driver
                    fmt
                    )
