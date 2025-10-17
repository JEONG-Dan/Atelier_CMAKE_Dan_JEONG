cmake_minimum_required(VERSION 3.15)
project(calculator C)
add_subdirectory(src)
enable_testing()
add_test(NAME calculator_square_5
         COMMAND $<TARGET_FILE:calculator> car 5)
set_tests_properties(calculator_square_5 PROPERTIES
  PASS_REGULAR_EXPRESSION "^[[:space:]]*25(\\.0+)?[[:space:]]*$"
)
