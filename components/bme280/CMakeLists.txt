cmake_minimum_required(VERSION 3.5)

idf_component_register(
    SRC_DIRS "driver"
)
if (IDF_VER STRGREATER_EQUAL "v4.0")
target_compile_options(${COMPONENT_LIB} PRIVATE -Wno-expansion-to-defined)
endif()
