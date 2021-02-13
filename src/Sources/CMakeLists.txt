# Settings
include_directories(${CMAKE_SOURCE_DIR}/src/Headers)

# Files
file(GLOB_RECURSE ENGINE_SOURCES *.cpp *.c)
file(GLOB_RECURSE ENGINE_HEADERS *.hpp *.h)

# Executable
add_executable(SRE ${ENGINE_SOURCES} ${ENGINE_HEADERS})
target_link_libraries(SRE sfml-graphics-d.lib sfml-audio-d.lib sfml-network-d.lib sfml-window-d.lib sfml-system-d.lib)