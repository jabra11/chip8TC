
set(src
        src/Driver.cpp
   )


add_library(chip8ASM_Driver STATIC ${src})
target_link_libraries(chip8ASM_Driver PUBLIC chip8ASM_API)
