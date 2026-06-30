cmake_minimum_required(VERSION 3.10)

# Required for export symbols
set(CMAKE_WINDOWS_EXPORT_ALL_SYMBOLS ON)

project(aescwc C)

add_library(${PROJECT_NAME} SHARED
    cwc.c
    aescrypt.c
    aeskey.c
    aestab.c
    aes_ni.c
)

target_compile_features(${PROJECT_NAME} PRIVATE c_std_99)
target_include_directories(${PROJECT_NAME} PRIVATE .)