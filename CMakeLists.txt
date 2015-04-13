project(dyad)

INCLUDE_DIRECTORIES(${CMAKE_CURRENT_SOURCE_DIR}/src)

file(GLOB src_lib ${CMAKE_CURRENT_SOURCE_DIR}/src/*.h ${CMAKE_CURRENT_SOURCE_DIR}/src/*.c)

add_executable(echoserv ${CMAKE_CURRENT_SOURCE_DIR}/example/echoserv.c ${src_lib})

add_executable(IRCBOT ${CMAKE_CURRENT_SOURCE_DIR}/example/ircbot.c ${src_lib})

add_executable(httpget ${CMAKE_CURRENT_SOURCE_DIR}/example/httpget.c ${src_lib})

add_executable(HTTPSERV ${CMAKE_CURRENT_SOURCE_DIR}/example/httpserv.c ${src_lib})

add_executable(DAYTIME ${CMAKE_CURRENT_SOURCE_DIR}/example/daytime.c ${src_lib})