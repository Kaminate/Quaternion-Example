cmake_minimum_required(VERSION 3.8)

project(myproject)

set(EXECUTABLE_NAME "myproject")
MESSAGE(Building ${EXECUTABLE_NAME})


add_subdirectory(source)
MESSAGE(SOURCES ${SOURCES})
add_executable(${EXECUTABLE_NAME} ${SOURCES})

set_target_properties(${PROJECT_NAME} PROPERTIES VS_DEBUGGER_WORKING_DIRECTORY ${CMAKE_SOURCE_DIR})

