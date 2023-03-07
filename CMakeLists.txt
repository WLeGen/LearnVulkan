cmake_minimum_required (VERSION 3.8)

project (LearnVulkan VERSION 1.0 LANGUAGES CXX)

set (LearnVulkan_VERSION_MAJOR 1)
set (LearnVulkan_VERSION_MINOR 0)

configure_file("${PROJECT_SOURCE_DIR}/LearnVulkanConfig.h.in" "${PROJECT_BINARY_DIR}/LearnVulkanConfig.h")

add_subdirectory ("LearnVulkan")

install (FILES "${PROJECT_BINARY_DIR}/LearnVulkanConfig.h" DESTINATION include)