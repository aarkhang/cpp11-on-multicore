cmake_minimum_required(VERSION 3.12)
set(CMAKE_CONFIGURATION_TYPES "Debug;Release" CACHE INTERNAL "limited configs")
project(BaseTests VERSION 1.0
        LANGUAGES CXX)

set(MACOSX_BUNDLE_GUI_IDENTIFIER "com.mycompany.\${PRODUCT_NAME:identifier}")
file(GLOB FILES *.cpp *.h)
add_executable(${PROJECT_NAME} MACOSX_BUNDLE ${FILES})
include(../../cmake/BuildSettings.cmake)

include_directories(../../common)
target_link_libraries(${PROJECT_NAME} cpp11_om)
