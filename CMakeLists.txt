cmake_minimum_required(VERSION 3.16.0)
project(boost_test VERSION 0.1.0)


#set(Boost_USE_STATIC_LIBS OFF)
#set(Boost_USE_STATIC_RUNTIME OFF)
set_property(GLOBAL PROPERTY USE_FOLDERS ON)
set(Boost_INCLUDE_DIR "E:/src/vcpkg/installed/x86-windows/include")

find_package(Boost)

add_executable(boost_test boost_for_each.cpp)

include_directories(${Boost_INCLUDE_DIRS})
link_directories(${Boost_LIBRARY_DIRS})


