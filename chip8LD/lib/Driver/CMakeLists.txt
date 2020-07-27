set(src
        src/Driver.cpp
   )

add_library(chip8LD_Driver STATIC ${src})
target_link_libraries(chip8LD_Driver PUBLIC chip8LD_API)
