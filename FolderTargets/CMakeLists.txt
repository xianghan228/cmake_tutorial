
project(FolderTargets)

set_property(GLOBAL PROPERTY USE_FOLDERS ON)

add_library(Target1 Target1.cpp)

add_library(Target2 Target2.cpp)
set_target_properties(Target2 PROPERTIES
    FOLDER "FOLDER2")

add_library(Target3 Target3.cpp)
set_target_properties(Target3 PROPERTIES
    FOLDER "FOLDER3")

add_library(Target4 Target4.cpp)
set_target_properties(Target4 PROPERTIES
    FOLDER "FOLDER3/FOLDER4")

add_library(Target5 Target5.cpp)
set_target_properties(Target5 PROPERTIES
    FOLDER "FOLDER3/FOLDER4")