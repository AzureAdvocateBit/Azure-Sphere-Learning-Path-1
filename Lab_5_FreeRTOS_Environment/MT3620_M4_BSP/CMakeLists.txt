CMAKE_MINIMUM_REQUIRED(VERSION 3.11)

PROJECT(MT3620_M4_BSP C)

ADD_LIBRARY(MT3620_M4_BSP
            ./mt3620/src/nvic.c
            ./mt3620/src/cirq_common.c
            ./mt3620/src/vector_table.c)

TARGET_INCLUDE_DIRECTORIES(MT3620_M4_BSP PUBLIC
                           ./CMSIS/include
                           ./mt3620/inc)

