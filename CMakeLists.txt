cmake_minimum_required(VERSION 3.9)
project(DALIGNER)

set(CMAKE_CXX_STANDARD 11)

add_executable(daligner
        align.c
        align.h
        daligner.c
        DB.c
        DB.h
        filter.c
        filter.h
        QV.c
        QV.h)

target_link_libraries (daligner pthread)
target_link_libraries(daligner m)

#add_executable(HPC.daligner
#        HPC.daligner.c
#        DB.c
#        DB.h
#        QV.c
#        QV.h)
#target_link_libraries(HPC.daligner m)
