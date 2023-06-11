cmake_minimum_required(VERSION 3.10)


include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)
file(GLOB SOURCES ${CMAKE_CURRENT_SOURCE_DIR}/src/*.cc)

project(main)


add_executable(main ${SOURCES})


# find_package(raylib CONFIG REQUIRED)
# target_link_libraries(main raylib)