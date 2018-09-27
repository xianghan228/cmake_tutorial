

cmake_minimum_required(VERSION 3.12)
project(GetFilenameComponent)


message(STATUS ===========================================)

get_filename_component(
    COMP_DIRECTORY
    ${CMAKE_CURRENT_SOURCE_DIR}
    DIRECTORY
    CACHE
)
message(STATUS "DIRECTORY: ${COMP_DIRECTORY}")

get_filename_component(
    COMP_NAME
    ${CMAKE_CURRENT_SOURCE_DIR}
    NAME
)
message(STATUS "NAME: ${COMP_NAME}")

get_filename_component(
    COMP_PATH
    ${CMAKE_CURRENT_SOURCE_DIR}/CMakeLists.txt
    PATH
)
message(STATUS "PATH: ${COMP_PATH}")

get_filename_component(
    COMP_EXT
    ${CMAKE_CURRENT_SOURCE_DIR}/CMakeLists.txt
    EXT
)
message(STATUS "EXT: ${COMP_EXT}")

get_filename_component(
    COMP_NAME_WE
    ${CMAKE_CURRENT_SOURCE_DIR}/CMakeLists.txt
    NAME_WE
)
message(STATUS "NAME_WE: ${COMP_NAME_WE}")

get_filename_component(
    COMP_ABSOLUTE
    CMakeLists.txt
    #BASE_DIR ${CMAKE_CURRENT_SOURCE_DIR}
    ABSOLUTE
)
message(STATUS "ABSOLUTE: ${COMP_ABSOLUTE}")

get_filename_component(
    COMP_REALPATH
    /usr/lib/ruby
    REALPATH
)
message(STATUS "REALPATH: ${COMP_REALPATH}")

get_filename_component(
    COMP_PROGRAM
    "ls -al"
    PROGRAM
    PROGRAM_ARGS COMP_PROGRAM_ARGS
)
message(STATUS "PROGRAM: ${COMP_PROGRAM}")
message(STATUS "COMP_PROGRAM_ARGS: ${COMP_PROGRAM_ARGS}")

message(STATUS ===========================================)