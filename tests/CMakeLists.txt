set(unittests_SOURCES
  testmain.cpp
  tests.cpp
  )

set(unittests_HEADERS
  ../src/list.h
  tests.hpp
  )

add_definitions(-Wno-write-strings)
add_executable(unittests ${unittests_SOURCES})
target_link_libraries(unittests cppunit list)
