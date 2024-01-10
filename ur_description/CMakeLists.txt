cmake_minimum_required(VERSION 3.10.2)
project(ur_description)

find_package(ament_cmake REQUIRED)

ament_package()

# if (CATKIN_ENABLE_TESTING)
#   find_package(roslaunch REQUIRED)
#   roslaunch_add_file_check(tests/roslaunch_test_ur10e.xml)
#   roslaunch_add_file_check(tests/roslaunch_test_ur10.xml)
#   roslaunch_add_file_check(tests/roslaunch_test_ur16e.xml)
#   roslaunch_add_file_check(tests/roslaunch_test_ur3e.xml)
#   roslaunch_add_file_check(tests/roslaunch_test_ur3.xml)
#   roslaunch_add_file_check(tests/roslaunch_test_ur5e.xml)
#   roslaunch_add_file_check(tests/roslaunch_test_ur5.xml)
# endif()

install(DIRECTORY cfg config launch meshes urdf
  DESTINATION share/${PROJECT_NAME})
