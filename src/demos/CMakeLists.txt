
set(dynamixel_simple_check_SOURCES
    dynamixel_simple_check.cpp)

set(dynamixel_simple_check_INCLUDES
    .
    ..
    .
    ..)

include_directories(${dynamixel_simple_check_INCLUDES})

add_executable(dynamixel_simple_check ${dynamixel_simple_check_SOURCES})
set(omnipointer_arm_SOURCES
    omnipointer_arm.cpp)

set(omnipointer_arm_INCLUDES
    .
    ..
    .
    ..)

include_directories(${omnipointer_arm_INCLUDES})

add_executable(omnipointer_arm ${omnipointer_arm_SOURCES})
set(operating_mode_SOURCES
    operating_mode.cpp)

set(operating_mode_INCLUDES
    .
    ..
    .
    ..)

include_directories(${operating_mode_INCLUDES})

add_executable(operating_mode ${operating_mode_SOURCES})
set(dynamixel_test_SOURCES
    dynamixel_test.cpp)

set(dynamixel_test_INCLUDES
    .
    ..
    .
    ..)

include_directories(${dynamixel_test_INCLUDES})

add_executable(dynamixel_test ${dynamixel_test_SOURCES})
