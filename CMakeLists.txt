cmake_minimum_required(VERSION 3.21)
project(co_context)

set(CMAKE_CXX_STANDARD 20)

FIND_PACKAGE(Boost)
IF (Boost_FOUND)

    INCLUDE_DIRECTORIES(${Boost_INCLUDE_DIR})

    ADD_DEFINITIONS( "-DHAS_BOOST" )

ENDIF()
add_executable(co_context main.cpp)
