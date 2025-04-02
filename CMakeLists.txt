cmake_minimum_required(VERSION 3.30)
project(Server)

set(CMAKE_CXX_STANDARD 20)
include_directories(include)
add_executable(Server main.cpp
        SSL/main.cpp
        SSL/Database.h
        SSL/HTTPRequest.h
        SSL/HTTPResponse.h
        SSL/HTTPServer.h
        SSL/Logger.h
        SSL/Router.h
        SSL/ThreadPoll.h)
