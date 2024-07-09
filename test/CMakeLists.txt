enable_testing()
find_package(GTest REQUIRED)

add_executable(
    test_framework
    framework.cc
)
    
target_link_libraries(
    test_framework
    GTest::gtest_main
    framework
)

gtest_discover_tests(test_framework)

