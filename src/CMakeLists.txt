set( CMAKE_INCLUDE_CURRENT_DIR ON )

add_library( demangle demangle.cpp )

target_compile_options( demangle
                        PUBLIC
                        ${BUILD_FPIC_FLAG} )

install( TARGETS demangle
         ARCHIVE DESTINATION ${CMAKE_INSTALL_PREFIX}/lib )
