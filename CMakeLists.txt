cmake_minimum_required(VERSION 2.8.3)
project(ros_helpers)

find_package(catkin_simple REQUIRED)
catkin_simple()

#ugly and simple copy paste
file(COPY
    "./scripts/node_launcher"
    DESTINATION ${CATKIN_DEVEL_PREFIX}/bin)

file(COPY
    "./scripts/qcatb"
    DESTINATION ${CATKIN_DEVEL_PREFIX}/bin)

file(COPY
    "./scripts/Catkin.sublime-build"
    DESTINATION $ENV{HOME}/.config/sublime-text-3/Packages/User)

file(COPY
    "./scripts/node_manager.desktop"
    DESTINATION $ENV{HOME}/.local/share/applications)
