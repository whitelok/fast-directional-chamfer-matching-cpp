aux_source_directory(${CMAKE_CURRENT_SOURCE_DIR} IMAGEIO_DIR_SRCS)
add_library(ImageIO ${IMAGEIO_DIR_SRCS})
target_include_directories(ImageIO PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

