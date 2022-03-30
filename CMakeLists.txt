# Set minimum required CMake version
cmake_minimum_required(VERSION 3.10)

# Set the project_name and version
project(HelloWorld VERSION 1.0)

# Specify the C++ standard
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Create a list of all source files that are used
set(SOURCES src/main.cpp src/JamesStuffLib/printer.cpp)

# Add the executable
add_executable(HelloWorld 
${SOURCES}
)

# Add the targeted cpp features
target_compile_features(HelloWorld PUBLIC cxx_std_20)