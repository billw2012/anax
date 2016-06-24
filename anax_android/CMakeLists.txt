cmake_minimum_required(VERSION 3.5)

file(GLOB_RECURSE header_files ../include/*.h ../include/*.hpp ../include/*.inc)
file(GLOB_RECURSE src_files ../src/*.cpp ../src/*.c ../src/*.cxx)

include_directories(
	../include
	../../cereal/include
	)


add_library(anax ${src_files} ${header_files})
