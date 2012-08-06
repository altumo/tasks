

cmake_minimum_required( VERSION "2.8.0" )
project( tasks )


add_executable( t src/main.cc )


if( CMAKE_COMPILER_IS_GNUCXX )
    message( STATUS "GCC detected, adding compile flags" )
    set( CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -Wextra -O2" )
endif( CMAKE_COMPILER_IS_GNUCXX )
