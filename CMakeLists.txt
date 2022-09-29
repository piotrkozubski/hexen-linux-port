cmake_minimum_required (VERSION 2.6)
project (MyProject LANGUAGES C)
add_compile_definitions(__WATCOMC__)
add_compile_options(-std=c2x)

file(GLOB all_SRCS
        "src/*.h"
        "src/*.c"
        )
add_executable(hexen ${all_SRCS})