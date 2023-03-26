cmake_minimum_required(VERSION 3.0)

project(LULESH CXX)

#set(LULESH_SOURCES
#  others.cc
#  lulesh.cc)

set(LULESH_SOURCES
  src/utils.cc
  src/lulesh.cc)

set(LULESH_EXEC lulesh1.0)

add_executable(${LULESH_EXEC} ${LULESH_SOURCES})
target_link_libraries(${LULESH_EXEC} ${LULESH_EXTERNAL_LIBS})
