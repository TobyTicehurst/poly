find_package(glfw3 3.3 REQUIRED)
find_package(OpenGL REQUIRED)
find_package(GLEW REQUIRED)

add_executable(test main.cpp)
target_include_directories(test PUBLIC CMAKE_CURRENT_SOURCE_DIR)
target_link_libraries(test glfw GLEW OpenGL::GL)
