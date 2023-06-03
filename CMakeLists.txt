cmake_minimum_required(VERSION 3.20)

project(JsonCPP LANGUAGES CXX)
message("[jsonCpp] ")
message("[jsonCpp] JsonCpp Core Library")
message("[jsonCpp] Generate From JsonCpp Library https://github.com/open-source-parsers/jsoncpp")
message("[jsonCpp] ")

add_library(JsonCPP 
    jsoncpp.cpp
    json/json-forwards.h
    json/json.h
)

include_directories(JsonCPP
    ${CMAKE_CURRENT_SOURCE_DIR}
)