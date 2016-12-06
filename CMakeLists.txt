cmake_minimum_required(VERSION 3.1)
project(game.libretro.4do)

list(APPEND CMAKE_MODULE_PATH ${PROJECT_SOURCE_DIR})

find_package(Kodi REQUIRED)
find_package(libretro-4do REQUIRED)

set(4DO_CUSTOM_BINARY ${4DO_LIB}
    ${PROJECT_NAME}${CMAKE_SHARED_LIBRARY_SUFFIX})

build_addon(${PROJECT_NAME} 4DO "")