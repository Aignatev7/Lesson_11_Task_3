cmake_minimum_required (VERSION 3.8)
project(Lesson_11_Task_3)
set(CMAKE_WINDOWS_EXPORT_ALL_SYMBOLS ON)
add_library(Lesson_11_Task_3DynamicLib SHARED Leaver.h Leaver.cpp)
add_executable(Lesson_11_Task_3Exe LeaverClient/LeaverClient.cpp)
target_link_libraries(Lesson_11_Task_3Exe Lesson_11_Task_3DynamicLib)

