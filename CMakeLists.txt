cmake_minimum_required(VERSION 3.13)
project(soil)

add_library(soil src/SOIL.c src/image_DXT.c src/image_helper.c src/stb_image_aug.c)
set_target_properties(soil PROPERTIES INTERFACE_INCLUDE_DIRECTORIES "${CMAKE_CURRENT_SOURCE_DIR}/include")
