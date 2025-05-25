cmake_minimum_required(VERSION 3.31)
project(251RCOSE34102 C)

set(CMAKE_C_STANDARD 11)

if(WIN32)
    add_compile_definitions(_CRT_SECURE_NO_WARNINGS)
    # MinGW(GCC)용 UTF-8 설정
    if(CMAKE_COMPILER_IS_GNUCC)
        add_compile_options(-finput-charset=UTF-8 -fexec-charset=UTF-8)
    endif()
endif()

add_executable(251RCOSE34102 TermProject.c)