
set(src
        src/Driver.cpp
   )


add_library(chip8ASM_Driver ${src})
target_link_libraries(chip8ASM_Driver PUBLIC chip8ASM_API)

install(TARGETS chip8ASM_Driver
    LIBRARY DESTINATION lib
    ARCHIVE DESTINATION lib
    RUNTIME DESTINATION bin
    )
