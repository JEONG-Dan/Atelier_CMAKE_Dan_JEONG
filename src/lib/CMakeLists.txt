file(GLOB LIB CONFIGURE_DEPENDS *.c)
add_library(lib ${LIB})
target_include_directories(lib PUBLIC ${PROJECT_SOURCE_DIR}/include)
