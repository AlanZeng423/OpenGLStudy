cmake_minimum_required(VERSION 3.25)
project(OpenGLStudy)

set(CMAKE_CXX_STANDARD 11)

include_directories(./glad/include)
include_directories(/opt/homebrew/Cellar/glfw/3.3.8/include)
link_directories(/opt/homebrew/Cellar/glfw/3.3.8/lib)

add_executable(
        OpenGLStudy
        ./glad/src/glad.c
#        Triangle.cpp
#        2Triangles.cpp
#        Tutorial1/Tutorial1.cpp
#        Tutorial1/init.cpp
        Tutorial2/Tutorial2.cpp)


target_link_libraries(
        OpenGLStudy
        glfw
)