cmake_minimum_required (VERSION 2.6)

add_executable( ${APPLICATION_NAME} LeMonADEViewerMain.cpp Camera.cpp LineParser.cpp )
target_link_libraries( ${APPLICATION_NAME} ${OPENGL_LIBRARIES} ${FLTK_LIBRARIES} LeMonADE )
SET_TARGET_PROPERTIES( ${APPLICATION_NAME} PROPERTIES VERSION "${APPLICATION_VERSION_MAJOR}.${APPLICATION_VERSION_MINOR}.${APPLICATION_VERSION_PATCH}" OUTPUT_NAME ${APPLICATION_NAME} CLEAN_DIRECT_OUTPUT 1 )
