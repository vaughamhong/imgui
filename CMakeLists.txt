# ================================================================

CMAKE_MINIMUM_REQUIRED(VERSION 2.8)
PROJECT(imgui)

# ================================================================

set(CMAKE_C_FLAGS "-g -Wall ${CMAKE_C_FLAGS}")
set(CMAKE_CXX_FLAGS "-g -Wall ${CMAKE_CXX_FLAGS}")

# ================================================================

FILE(GLOB src ${CMAKE_CURRENT_SOURCE_DIR}/*.cpp)
FILE(GLOB inc ${CMAKE_CURRENT_SOURCE_DIR}/*.h)
INCLUDE_DIRECTORIES(${CMAKE_CURRENT_SOURCE_DIR})

ADD_LIBRARY(imgui ${src} ${inc})

# ================================================================