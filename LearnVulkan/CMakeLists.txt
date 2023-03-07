cmake_minimum_required (VERSION 3.8)

file(GLOB_RECURSE INCLUDE_FILES *.h)
file(GLOB_RECURSE SOURCE_FILES *.cpp)

add_executable (LearnVulkan ${INCLUDE_FILES} ${SOURCE_FILES})

target_include_directories(LearnVulkan PUBLIC
                           "${PROJECT_BINARY_DIR}"
                           )

install (TARGETS LearnVulkan DESTINATION bin)
install (FILES )