cmake_minimum_required(VERSION 2.8)
project(opencv_tests)

find_package(catkin REQUIRED)
catkin_package()

### FOR PROFILING (need to set after catkin_package)
add_compile_options(-pg)
set(catkin_LIBRARIES ${catkin_LIBRARIES} -pg)
###
