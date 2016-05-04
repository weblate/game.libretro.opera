project(game.libretro.4do)

cmake_minimum_required(VERSION 2.6)

list(APPEND CMAKE_MODULE_PATH ${PROJECT_SOURCE_DIR})

enable_language(CXX)

find_package(kodi REQUIRED)
find_package(libretro-4do REQUIRED)

set(DEPLIBS 4do
set(4DO_CUSTOM_BINARY ${4DO_LIB}
                      ${PROJECT_NAME}${CMAKE_SHARED_LIBRARY_SUFFIX} 4do)

build_addon(${PROJECT_NAME} 4DO DEPLIBS)
