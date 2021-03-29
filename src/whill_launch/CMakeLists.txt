cmake_minimum_required(VERSION 2.8.3)
project(whill_launch)


find_package(catkin REQUIRED COMPONENTS
)

#catkin_package(
#  CATKIN_DEPENDS
#)

include_directories(
  ${catkin_INCLUDE_DIRS}
)

if(CATKIN_ENABLE_LINTS)
  # catkin-lint
  add_custom_target(${PROJECT_NAME}_CATKIN_LINT ALL COMMAND catkin_lint --pkg ${PROJECT_NAME} -W2)
endif()
