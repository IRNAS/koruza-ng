cmake_minimum_required(VERSION 2.6)

project(koruza-ng C)
add_definitions(-Os -Wall -Werror --std=gnu99 -Wmissing-declarations)

set(SOURCES
main.c
)

set(LIBS
)

include_directories(include)

add_executable(koruza-ng ${SOURCES})
target_link_libraries(koruza-ng ${LIBS})

install(TARGETS koruza-ng
  RUNTIME DESTINATION bin
  LIBRARY DESTINATION lib
)

