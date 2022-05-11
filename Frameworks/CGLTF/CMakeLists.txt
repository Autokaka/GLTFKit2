project(CGLTF)

file(GLOB_RECURSE SOURCE Headers)
source_group(TREE ${PROJECT_SOURCE_DIR} FILES ${SOURCE})

add_library(CGLTF INTERFACE ${SOURCE})
target_include_directories(CGLTF INTERFACE Headers)
target_include_directories(CGLTF INTERFACE Headers/CGLTF)
