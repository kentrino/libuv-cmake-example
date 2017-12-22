cmake_minimum_required(VERSION 2.8)

include(deps/uv.cmake)
set(LIBUV_LIBRARIES uv)

add_executable(main src/main.cc)

target_link_libraries(main ${LIBUV_LIBRARIES})
