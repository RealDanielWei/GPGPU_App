cmake_minimum_required(VERSION 3.18.1)

project(GPGPU_App)

set(ROOT_PATH ${CMAKE_CURRENT_SOURCE_DIR})

add_subdirectory(submodules/glfw)
add_subdirectory(submodules/glm)
add_subdirectory(lib/GLWrapper)
add_subdirectory(app)
