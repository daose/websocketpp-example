# CMakeList.txt : CMake project for KinectServer, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.8)

add_compile_definitions(ASIO_STANDALONE)
add_compile_definitions(_WEBSOCKETPP_CPP11_STL_)
# Add source to this project's executable.
add_executable (Server "Server.cpp")
target_include_directories(Server SYSTEM PRIVATE "include")
