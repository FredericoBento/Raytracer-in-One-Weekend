cmake_minimum_required(VERSION 3.10)

project(Raytracer VERSION 1.0)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED true)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
set(CMAKE_EXPORT_ADD_DEFINITIONS ON)

include_directories(include/)

add_executable(Raytracer 
  include/color.h
  include/interval.h
  include/vec3.h
  include/ray.h
  include/hittable.h
  include/hittable_list.h
  include/sphere.h
  include/rtweekend.h
  src/main.cpp
)
