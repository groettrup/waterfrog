cmake_minimum_required(VERSION 3.15)
project(waterfrog C CXX)

add_executable(${PROJECT_NAME} src/main.c)

find_package(glad REQUIRED)
find_package(glfw3 REQUIRED)

# Use the global target
target_link_libraries(${PROJECT_NAME} glad::glad)
target_link_libraries(${PROJECT_NAME} glfw)
