cmake_minimum_required(VERSION 3.2)

project(TWAMPP VERSION 0.0.1 LANGUAGES CXX)

add_library(twamppp src/twamppp.cpp)

add_executable(demo examples/main.cpp)

target_include_directories(demo
	PRIVATE include
	)

target_link_libraries(demo
	PRIVATE twamppp
	)

