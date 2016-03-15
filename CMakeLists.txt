cmake_minimum_required(VERSION 2.8)

add_library (open-simplex-noise STATIC open-simplex-noise.c)

target_include_directories (open-simplex-noise PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

install(TARGETS open-simplex-noise
        DESTINATION "lib")

install(FILES open-simplex-noise.h
        DESTINATION "include")


