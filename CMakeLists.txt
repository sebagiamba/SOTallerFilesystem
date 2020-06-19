# cmake_minimum_required(VERSION <specify CMake version here>)
project(Taller_FS)

set(CMAKE_CXX_STANDARD 14)

include_directories(.)
include_directories(include)
include_directories(src)
include_directories(test)

add_executable(Taller_FS
        include/ext2fs.h
        include/fs.h
        include/hdd.h
        include/mbr.h
        include/pentry.h
        src/ext2fs.cpp
        src/hdd.cpp
        src/mbr.cpp
        src/pentry.cpp
        test/testhdd.cpp)
