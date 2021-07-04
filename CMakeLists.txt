cmake_minimum_required(VERSION 3.10)

project(nodecey VERSION 1.0)

configure_file(config.h.in config.h)

add_executable(nodecey ./src/main.cpp)

target_include_directories(nodecey PUBLIC
        "${PROJECT_BINARY_DIR}"
        )
