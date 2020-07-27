
set(src
        src/Driver.cpp
   )


add_library(chip8C_Driver STATIC ${src})
target_link_libraries(chip8C_Driver PUBLIC chip8C_API)
