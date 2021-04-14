
add_executable(${PROJECT_NAME} main.cpp ../lib/glad/glad.c)

target_include_directories(${PROJECT_NAME} PUBLIC ../submodules/glfw/include)
target_include_directories(${PROJECT_NAME} PUBLIC ../lib/glad)

target_link_directories(${PROJECT_NAME} PUBLIC ../submodules/glfw/src)

target_link_libraries(${PROJECT_NAME} PUBLIC glfw)

