aux_source_directory(${CMAKE_CURRENT_SOURCE_DIR} FITLINE_DIR_SRCS)
add_library(Fitline ${FITLINE_DIR_SRCS})
target_include_directories(Fitline PUBLIC ${CMAKE_SOURCE_DIR} ${CMAKE_CURRENT_SOURCE_DIR})
target_link_libraries(Fitline Fdcm ImageIO)

add_executable(FitlineEXE ${FITLINE_DIR_SRCS})
target_link_libraries(FitlineEXE Fitline)