cmake_minimum_required(VERSION 2.8.3)
project(mds_pointclouds)
find_package(catkin REQUIRED)

catkin_package()

install(DIRECTORY people/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/people
)

install(DIRECTORY objects/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/objects
  PATTERN "objects/table_setups/erl-service-italy-2017-objects" EXCLUDE
)
