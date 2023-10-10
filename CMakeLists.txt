cmake_minimum_required(VERSION 3.25)
project(OpenGLStudy)

set(CMAKE_CXX_STANDARD 11)

include_directories(./glad/include)
include_directories(./glm-0.9.9.1)
include_directories(/opt/homebrew/Cellar/glfw/3.3.8/include)
link_directories(/opt/homebrew/Cellar/glfw/3.3.8/lib)

add_executable(
        OpenGLStudy
        ./glad/src/glad.c
#        Triangle.cpp
#        2Triangles.cpp
#        Tutorial1/Tutorial1.cpp
#        Tutorial1/init.cpp
#        Tutorial2/Tutorial2.cpp
#        Tutorial3/Tutorial3.cpp
#        Tutorial3/Tutorial3_2.cpp
        Tutorial4/Source.cpp
#        Tutorial3/Tutorial3.cpp
#        Tutorial3/Tutorial3_3/Tutorial3_3.cpp
#        Tutorial3/Tutorial3_3/shader.h
        Tutorial4/shader.h
)


target_link_libraries(
        OpenGLStudy
        glfw
)