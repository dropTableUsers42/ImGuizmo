cmake_minimum_required(VERSION 3.10)
set(CMAKE_CXX_STANDARD 17)

project(ImGuizmo)

add_library(ImGuizmo STATIC ImGuizmo.cpp GraphEditor.cpp ImCurveEdit.cpp ImGradient.cpp ImSequencer.cpp)
target_include_directories(ImGuizmo PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

target_include_directories(ImGuizmo PRIVATE ../../../LightFramework/libs/imgui)
