﻿# Copyright 2024 Yonggang Luo
# SPDX-License-Identifier: MIT

cpk_add_test(
  NAME pebteb-test
  SOURCES
    peb-test.cpp
    teb-test.cpp
    test-include-ntpebteb.c
    test-include-phnt.c
    test-main.cpp
    win-polyfill.cpp
  WORKING_DIRECTORY
    ${CMAKE_CURRENT_LIST_DIR}
)
target_link_libraries(pebteb-test PRIVATE win-polyfill-phnt)
