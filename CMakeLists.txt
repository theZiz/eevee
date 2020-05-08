cmake_minimum_required(VERSION 3.1)

set(PROJECTNAME eevee)

project( ${PROJECTNAME} )

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

set(SRCS
	${CMAKE_SOURCE_DIR}/src/eevee.cpp
)

add_executable( ${PROJECTNAME} ${HDRS} ${SRCS} )
#include_directories(${PROJECTNAME} ${INCLUDE})
#target_link_libraries(${PROJECTNAME} ${LIBS})

install(TARGETS ${PROJECTNAME} RUNTIME DESTINATION bin)
