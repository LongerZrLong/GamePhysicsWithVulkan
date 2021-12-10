cmake_minimum_required(VERSION 3.10)
project(GamePhysicsWithVulkan)

set(CMAKE_CXX_STANDARD 17)

file(GLOB_RECURSE SRCS code/*.cpp)

add_executable(${PROJECT_NAME} ${SRCS})

# GLFW
add_subdirectory(external/GLFW)
target_link_libraries(${PROJECT_NAME} glfw)

# Vulkan
find_package(Vulkan REQUIRED)
target_link_libraries(${PROJECT_NAME} Vulkan::Vulkan)

# ====================== Copy data to binary folder ========================
set(DATA_SOURCE_DIR ${PROJECT_SOURCE_DIR}/data)
set(DATA_DST_PARENT_DIR ${PROJECT_BINARY_DIR})

file(COPY ${DATA_SOURCE_DIR} DESTINATION ${DATA_DST_PARENT_DIR})
