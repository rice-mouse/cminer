set(SOURCES
    ApiServer.h ApiServer.cpp
)

add_library(apicore ${SOURCES})
target_link_libraries(apicore PRIVATE ethcore devcore cminer-buildinfo Boost::filesystem)
target_include_directories(apicore PRIVATE ..)
