set(SOURCES
  main.cpp
  mutex.cpp
)

add_executable(paltest_mutex_shared
  ${SOURCES}
)

add_dependencies(paltest_mutex_shared coreclrpal)

target_link_libraries(paltest_mutex_shared
  ${COMMON_TEST_LIBRARIES}
  rt
)
