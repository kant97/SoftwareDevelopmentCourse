find_package(Threads REQUIRED)
include_directories(include .)

add_library(gtest src/gtest-all.cc)
add_library(gtest_main src/gtest_main)
target_link_libraries(gtest_main gtest)
