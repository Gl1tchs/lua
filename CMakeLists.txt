project(lua)

file(GLOB LUA_SOURCES "*.c")

add_library(lua ${LUA_SOURCES})
add_library(lua::lua ALIAS lua)

target_include_directories(lua PUBLIC ${CMAKE_CURRENT_LIST_DIR})
