cmake_minimum_required(VERSION 3.1)
project(gcc_insects)

add_library(gcc_insects STATIC main.cpp functions.cpp)

target_compile_features(gcc_insects PUBLIC cxx_std_20)
target_precompile_headers(gcc_insects PRIVATE functions.h)
