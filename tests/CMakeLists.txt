project(google_tests)
add_subdirectory(lib)
include_directories(${gtest_SOURCE_DIR}/include ${gtest_SOURCE_DIR})

add_executable(run_tests test.cpp)

target_link_libraries(run_tests ${CMAKE_PROJECT_NAME}_lib)

target_link_libraries(run_tests gtest gtest_main)