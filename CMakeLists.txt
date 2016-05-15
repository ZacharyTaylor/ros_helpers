cmake_minimum_required(VERSION 2.8.3)
project(ros_helpers)

find_package(catkin_simple REQUIRED)
catkin_simple()

file(COPY
    "./scripts/node"
    DESTINATION ${CATKIN_DEVEL_PREFIX}/bin/)

file(COPY
    "./scripts/qcatb"
    DESTINATION ${CATKIN_DEVEL_PREFIX}/bin/)
