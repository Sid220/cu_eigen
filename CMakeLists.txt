cmake_minimum_required(VERSION 3.22)
project(cu_eigen CUDA)

set(CMAKE_CUDA_STANDARD 20)

add_library(cu_eigen STATIC library.cu)

set_target_properties(cu_eigen PROPERTIES
        CUDA_SEPARABLE_COMPILATION ON)
