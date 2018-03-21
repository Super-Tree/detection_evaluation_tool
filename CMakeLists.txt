cmake_minimum_required (VERSION 2.6)
project(devkit_object)

#add_library(
#            gt_parse/parse.h
#)
include_directories(gt_parse)
#add_definitions(-DPATH /home/hexindong/)
add_executable( evaluate_object
                evaluate_object_bv.cpp
                gt_parse/parse.cpp
                )
SET_TARGET_PROPERTIES(evaluate_object  PROPERTIES    #表示生成的执行文件所在路径
                      RUNTIME_OUTPUT_DIRECTORY "${PROJECT_SOURCE_DIR}")