include_directories(../hello ../world)
aux_source_directory(. DIR_APP_SRCS)
add_library(app  ${DIR_APP_SRCS})
