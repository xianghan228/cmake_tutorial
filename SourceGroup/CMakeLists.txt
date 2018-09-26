project(SourceGroup)

file(GLOB_RECURSE Header_Files ${PROJECT_SOURCE_DIR}/*.h)
#set(Header_Files ${Header_Files} ${PROJECT_SOURCE_DIR}/header.hpp)

set(SOURCE1_FILES 
    ${PROJECT_SOURCE_DIR}/source1.cpp
    ${PROJECT_SOURCE_DIR}/source2.cpp)

set(SOURCE2_FILES 
    ${PROJECT_SOURCE_DIR}/source3.cpp
    ${PROJECT_SOURCE_DIR}/source4.cpp
    ${PROJECT_SOURCE_DIR}/source7.cpp)

set(SOURCE3_FILES 
    ${PROJECT_SOURCE_DIR}/source5.cpp
    ${PROJECT_SOURCE_DIR}/source6.cpp
    ${PROJECT_SOURCE_DIR}/source8.cpp)

source_group(GROUP1 FILES ${SOURCE1_FILES})
source_group(HEADERS FILES ${Header_Files})
source_group(GROUP2 FILES ${SOURCE2_FILES})
source_group(TREE ${PROJECT_SOURCE_DIR} PREFIX GROUP2\\GROU2_SUB FILES ${SOURCE3_FILES})
source_group(HEADERS_HPP REGULAR_EXPRESSION "${PROJECT_SOURCE_DIR}/*.h")

add_library(SourceGroup SHARED 
    ${Header_Files}
    ${SOURCE1_FILES}
    ${SOURCE2_FILES}
    ${SOURCE3_FILES}
    ${PROJECT_SOURCE_DIR}/header.hpp)

