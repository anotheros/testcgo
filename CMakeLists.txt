cmake_minimum_required(VERSION 3.0)
project(test)

add_subdirectory(go)

set(TARGET test)
set(SRCS test.cpp)

add_executable(${TARGET} ${SRCS})
target_link_libraries(${TARGET} goshim pthread)