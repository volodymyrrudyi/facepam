cmake_minimum_required (VERSION 2.6) 
project (facepam) 

set(CMAKE_C_FLAGS "-Wall -g -pg -Werror -fPIC -fno-stack-protector")

add_subdirectory (src)
add_library(facepam SHARED ${FACEPAM_HEADERS} ${FACEPAM_SOURCES})
