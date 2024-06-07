# List all source files in the src directory
set(SRC_FILES
    Hello.cpp
)

# Set the source files to the parent scope so it can be accessed by the parent CMakeLists.txt
set(SRC_FILES ${SRC_FILES} PARENT_SCOPE)

# Add an executable with the source files from the src directory
add_executable(MyExecutable ${SRC_FILES})

# Optionally, if you have header files, you can add them too:
# set(HEADER_FILES
#     hello.h
# )

# Optionally, if you have subdirectories within src, you can add them using add_subdirectory()
# add_subdirectory(subdir)