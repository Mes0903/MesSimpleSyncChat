SET(CMAKE_TOOLCHAIN_FILE "C:/Users/Mes/vcpkg/scripts/buildsystems/vcpkg.cmake")
cmake_minimum_required(VERSION 3.21)
project(MesClient)

find_package(Boost REQUIRED COMPONENTS system)

file(GLOB_RECURSE SOURCE_FILES src/*.cpp)
add_executable(MesClient ${SOURCE_FILES})

target_include_directories(MesClient PRIVATE include)
target_link_libraries(MesClient
                ${Boost_LIBRARIES})