cmake_minimum_required(VERSION 3.12)

project(glad C)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

include_directories(include)

set(
    SOURCE
    "src/glad.c"
)

set(
    HEADERS 
	"include/glad/glad.h"
	"include/KHR/khrplatform.h"
)

add_library(${PROJECT_NAME} STATIC ${SOURCE} ${HEADERS})



