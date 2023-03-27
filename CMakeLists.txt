cmake_minimum_required(VERSION 3.24)
project(transportation_quiz)

set(CMAKE_CXX_STANDARD 20)

set(wxBUILD_SHARED OFF)

add_subdirectory(lib/wxWidgets)
add_executable(transportation_quiz src/main.cpp)

target_link_libraries(transportation_quiz wx::net wx::core wx::base)

set_target_properties(transportation_quiz PROPERTIES WIN32_EXECUTABLE ON)
