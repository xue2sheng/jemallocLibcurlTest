cmake_minimum_required(VERSION 3.5)

#project(JemallocLibcurlTest CXX) 
set(LOCAL_CMAKE_PROJECT_NAME JemallocLibcurlTest) 
project(${LOCAL_CMAKE_PROJECT_NAME} NONE) 

### Specific configuration ###
set(CMAKE_MODULE_PATH "${CMAKE_CURRENT_SOURCE_DIR}/cmake" ${CMAKE_MODULE_PATH})
message(STATUS "${LOCAL_CMAKE_PROJECT_NAME} cmake module path: ${CMAKE_MODULE_PATH}")
find_package(JemallocLibcurlTestRules)

### Code ###
add_subdirectory("src")

### Testing ###
#if(${LOCAL_CMAKE_PROJECT_NAME}_TEST)
#  enable_testing()
#  add_subdirectory("test")
#endif()
