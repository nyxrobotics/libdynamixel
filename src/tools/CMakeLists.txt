set(p2-dynamixel_SOURCES
    dynamixel.cpp)

set(p2-dynamixel_INCLUDES
    .
    ..
    .
    ..
    /usr/include)

include_directories(${p2-dynamixel_INCLUDES})

add_executable(p2-dynamixel ${p2-dynamixel_SOURCES})
target_link_libraries(p2-dynamixel ${Boost_LIBRARIES})

set(dynamixel_SOURCES
    dynamixel.cpp)

set(dynamixel_INCLUDES
    .
    ..
    .
    ..
    /usr/include)

include_directories(${dynamixel_INCLUDES} )

add_definitions(-DPROTOCOL1)

add_executable(dynamixel ${dynamixel_SOURCES})
target_link_libraries(dynamixel ${Boost_LIBRARIES})