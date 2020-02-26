cmake_minimum_required(VERSION 2.8)
project(helloworld)


#add the source in project root directory
aux_source_directory(. DIRSRCS)

#add header file include directories
include_directories(./app)

#add block directory
add_subdirectory(hello)
add_subdirectory(world)
add_subdirectory(app)


#target
add_executable(helloworld ${DIRSRCS})
target_link_libraries(helloworld  app hello world)


