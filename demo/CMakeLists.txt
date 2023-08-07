add_library(demo SHARED
    Agent.cpp
)
target_include_directories(demo
PUBLIC
    /usr/local/include
    ${CMAKE_SOURCE_DIR}/include
    .
)
target_link_directories(demo
PUBLIC
    /usr/local/lib
    ${CMAKE_SOURCE_DIR}/lib
)
target_link_libraries(demo
PUBLIC
    pthread
)
