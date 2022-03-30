# How to use a include without a libary

## Create a list of all source files that are used
set(SOURCES src/main.cpp src/JamesStuffLib/printer.cpp)

## Add the executable
add_executable(HelloWorld 
	${SOURCES}
)