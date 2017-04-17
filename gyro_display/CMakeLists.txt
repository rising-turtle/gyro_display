project(display)

include_directories(${CMAKE_CURRENT_SOURCE_DIR})
link_directories(/usr/lib/i386-linux-gnu)

add_executable(test_gyro_display test_gyro_display.cpp gl_cubic.cpp ros_gl_cube.cpp)
target_link_libraries(test_gyro_display ${catkin_LIBRARIES} GL GLU glut)
