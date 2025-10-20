cmake_minimum_required(VERSION 3.20)
project(coding_task C)

set(CMAKE_C_STANDARD 11)
set(CMAKE_C_STANDARD_REQUIRED ON)

# Include all C source files in src/
file(GLOB SRC_FILES "src/*.c")

add_executable(coding_task ${SRC_FILES})

# Add include folder so headers are found
target_include_directories(coding_task PRIVATE include)
