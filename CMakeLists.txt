cmake_minimum_required(VERSION 3.21)
project(simple_sync_chat)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

add_subdirectory(client)
add_subdirectory(server)