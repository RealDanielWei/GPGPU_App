set(LIBRARY_NAME "GLWrapper")

add_library(${LIBRARY_NAME} GLWrapper.cpp)

target_include_directories(${LIBRARY_NAME} PUBLIC ${ROOT_PATH}/submodules/glfw/include)
target_include_directories(${LIBRARY_NAME} PUBLIC ${ROOT_PATH}/submodules/glm)
target_include_directories(${LIBRARY_NAME} PUBLIC ${ROOT_PATH}/lib/glad)

target_link_directories(${LIBRARY_NAME} PUBLIC ${ROOT_PATH}/submodules/glfw/src)
target_link_directories(${LIBRARY_NAME} PUBLIC ${ROOT_PATH}/submodules/glm)

target_link_libraries(${LIBRARY_NAME} PUBLIC glfw)
target_link_libraries(${LIBRARY_NAME} PUBLIC glm)