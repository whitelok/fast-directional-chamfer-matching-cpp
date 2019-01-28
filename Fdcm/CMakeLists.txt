aux_source_directory(${CMAKE_CURRENT_SOURCE_DIR} FDCM_DIR_SRCS)
add_library(Fdcm ${FDCM_DIR_SRCS})
target_link_libraries(Fdcm Fitline ImageIO)

add_executable(FdcmEXE ${FDCM_DIR_SRCS})
target_link_libraries(FdcmEXE Fdcm)

