# boost
#message(STATUS "Using boost at ${BOOST_ROOT}")
#find_package( Boost 1.58.0 REQUIRED)
#if(Boost_FOUND)
# ## test doesn't belong to Boost test framework
# file(GLOB SOURCES *.cpp)
# include_directories(${CMAKE_CURRENT_SOURCE_DIR} ${Boost_INCLUDE_DIR})
# add_executable(${LOCAL_CMAKE_PROJECT_NAME} ${SOURCES})
# target_link_libraries(${LOCAL_CMAKE_PROJECT_NAME})
#endif(Boost_FOUND)

file(GLOB SOURCES main.cpp)
include_directories(${CMAKE_CURRENT_SOURCE_DIR})
add_executable(${LOCAL_CMAKE_PROJECT_NAME} ${SOURCES})
target_link_libraries(${LOCAL_CMAKE_PROJECT_NAME} jemalloc curl xml2)


