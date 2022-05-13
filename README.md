# How to use a include without a libary

This project was simply to show how to include extra cpp files when building an application using CMake

## Create a list of all source files that are used
Inside of the CMakeLists.txt file add a line that sets a var called sources to contain all the source CPP files.
set(SOURCES src/main.cpp src/JamesStuffLib/printer.cpp)

## Add the executable
Inside the same CMakeLists.txt file add a like that adds the files in the sources var to the EXE we want to create.
add_executable(HelloWorld 
	${SOURCES}
)