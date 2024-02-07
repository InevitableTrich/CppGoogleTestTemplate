set(SOURCES
        example.cpp)

set(HEADERS
        example.h)

add_library(${CMAKE_PROJECT_NAME}_lib STATIC ${SOURCES} ${HEADERS})