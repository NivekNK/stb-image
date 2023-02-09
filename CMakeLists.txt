cmake_minimum_required(VERSION 3.12)

project("stb-image"
    VERSION 0.0.1
    DESCRIPTION "Image loading/decoding from file/memory"    
    HOMEPAGE_URL "https://github.com/NivekNK/stb-image"
)

add_library(${PROJECT_NAME} INTERFACE)

target_include_directories(${PROJECT_NAME}
    INTERFACE
        $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>
        $<INSTALL_INTERFACE:${CMAKE_INSTALL_INCLUDEDIR}>
)
