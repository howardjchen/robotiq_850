cmake_minimum_required(VERSION 2.8.2)
project(robotiq_boost)

find_package(Boost REQUIRED COMPONENTS system)

set(CMAKE_CXX_FLAGS "-std=c++11")

add_executable(robotiq_boost robotiq850.cpp)
target_link_libraries(robotiq_boost ${Boost_LIBRARIES})
