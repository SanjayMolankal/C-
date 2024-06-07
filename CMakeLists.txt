cmake_minimum_required(VERSION 3.10)

# Set the project name
project(MyProject)

#Add the Source directory
add_subdirectory(src)

#Add an executable
add_executable(MyExecutable main.cpp Hello.cpp)

# Add tests - New tests
enable_testing()
add_test(NAME MyTest COMMAND MyExecutable)

