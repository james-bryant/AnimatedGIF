set(LIB_NAME AnimatedGIF)

add_library(${LIB_NAME} INTERFACE)

target_compile_definitions(${LIB_NAME} INTERFACE CMAKE_EXPORT_COMPILE_COMMANDS=1)
target_sources(${LIB_NAME} INTERFACE
    ${CMAKE_CURRENT_LIST_DIR}/src/${LIB_NAME}.cpp
)

target_include_directories(${LIB_NAME} INTERFACE ${CMAKE_CURRENT_LIST_DIR}/src)
