
add_executable(${PROJECT_NAME} main.cpp ${ROOT_PATH}/lib/glad/glad.c)

target_include_directories(${PROJECT_NAME} PUBLIC ${ROOT_PATH}/lib/GLWrapper)
target_include_directories(${PROJECT_NAME} PUBLIC ${ROOT_PATH}/submodules/glfw/include)
target_include_directories(${PROJECT_NAME} PUBLIC ${ROOT_PATH}/submodules/glm)
target_include_directories(${PROJECT_NAME} PUBLIC ${ROOT_PATH}/lib/glad)

target_link_directories(${PROJECT_NAME} PUBLIC ${ROOT_PATH}/lib/GLWrapper)

target_link_libraries(${PROJECT_NAME} PUBLIC GLWrapper)

file(COPY ./resource DESTINATION ${CMAKE_CURRENT_BINARY_DIR})

