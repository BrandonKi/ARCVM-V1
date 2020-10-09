cmake_minimum_required(VERSION 3.0.0)
project(ARCVM VERSION 0.1.0)

set (CMAKE_CXX_STANDARD 17)

SET(EXECUTABLE_OUTPUT_PATH ${CMAKE_CURRENT_SOURCE_DIR}/bin)

set(VM_SOURCES ${CMAKE_CURRENT_SOURCE_DIR}/src/VMDriver.cpp ${CMAKE_CURRENT_SOURCE_DIR}/src/VM.cpp)

add_executable(ARCVM ${VM_SOURCES})

target_compile_definitions(ARCVM PRIVATE DEBUG_BUILD)

target_include_directories(ARCVM PRIVATE ${CMAKE_CURRENT_SOURCE_DIR}/include)