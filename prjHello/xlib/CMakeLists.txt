

aux_source_directory(./app   APP_SRC_DIR)
aux_source_directory(./hello HELLO_SRC_DIR)
aux_source_directory(./world WORLD_SRC_DIR)

include_directories(./app)
include_directories(./hello)
include_directories(./world)


add_library(xlib   ${APP_SRC_DIR}   ${HELLO_SRC_DIR} ${WORLD_SRC_DIR})



