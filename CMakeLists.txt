cmake_minimum_required(VERSION 3.15)
project(vk_engine)

set(CMAKE_CXX_STANDARD 17)
find_package(Vulkan REQUIRED)

add_executable(
    vk_engine 
    first_app.cpp
    first_app.hpp
    lve_pipeline.cpp
    lve_pipeline.hpp
    lve_device.cpp
    lve_device.hpp
    lve_window.cpp
    lve_window.hpp
    main.cpp
)
target_link_libraries(vk_engine Vulkan::Vulkan glfw)