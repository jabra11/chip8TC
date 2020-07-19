add_executable(chip8ASM driver.cpp)

target_link_libraries(chip8ASM 
                    PRIVATE
                    Driver
                    fmt
                    )
