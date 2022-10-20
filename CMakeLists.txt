# 버젼 정보
cmake_minimum_required(VERSION 3.11)

# 프로젝트 정보
project(server_all)

set(
	SOURCE_LIST
	"Util/Util.h"
	"Util/Util.cpp"
	"main.cpp"
)

add_executable(App ${SOURCE_LIST})

#target_include_directories(app PUBLIC ${CMAKE_SOURCE_DIR}/Util)

source_group(TREE ${CMAKE_CURRENT_SOURCE_DIR} FILES ${SOURCE_LIST})
