set(dynamixel_simple_check_SOURCES
    dynamixel_simple_check.cpp)
set(dynamixel_simple_check_INCLUDES
    .
    ..
    .
    ..)
include_directories(${dynamixel_simple_check_INCLUDES})

add_executable(dynamixel_simple_check ${dynamixel_simple_check_SOURCES})
target_link_libraries(dynamixel_simple_check ${Boost_LIBRARIES})

set(omnipointer_arm_SOURCES
    omnipointer_arm.cpp)
set(omnipointer_arm_INCLUDES
    .
    ..
    .
    ..)
include_directories(${omnipointer_arm_INCLUDES})

add_executable(omnipointer_arm ${omnipointer_arm_SOURCES})
target_link_libraries(omnipointer_arm ${Boost_LIBRARIES})

set(operating_mode_SOURCES
    operating_mode.cpp)
set(operating_mode_INCLUDES
    .
    ..
    .
    ..)
include_directories(${operating_mode_INCLUDES})

add_executable(operating_mode ${operating_mode_SOURCES})
target_link_libraries(operating_mode ${Boost_LIBRARIES})

set(dynamixel_test_SOURCES
    dynamixel_test.cpp)
set(dynamixel_test_INCLUDES
    .
    ..
    .
    ..)
include_directories(${dynamixel_test_INCLUDES})

add_executable(dynamixel_test ${dynamixel_test_SOURCES})
target_link_libraries(dynamixel_test ${Boost_LIBRARIES})
