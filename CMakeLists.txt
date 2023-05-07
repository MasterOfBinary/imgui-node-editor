cmake_minimum_required(VERSION 3.26)

project(imgui-node-editor)

set(SOURCE_FILES
    crude_json.cpp
    crude_json.h
    imgui_bezier_math.h
    imgui_bezier_math.inl
    imgui_canvas.cpp
    imgui_canvas.h
    imgui_extra_math.h
    imgui_extra_math.inl
    imgui_node_editor.cpp
    imgui_node_editor.h
    imgui_node_editor_api.cpp
    imgui_node_editor_internal.h
    imgui_node_editor_internal.inl
)

add_library(imgui_node_editor STATIC ${SOURCE_FILES})
target_include_directories(imgui_node_editor PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
