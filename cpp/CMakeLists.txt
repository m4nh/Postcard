cmake_minimum_required(VERSION 2.8)
project( PostcardCppClient )

add_definitions(-std=c++11)

find_package( OpenCV REQUIRED )

add_executable( client_example client_example.cpp )
target_link_libraries( client_example ${OpenCV_LIBS} )