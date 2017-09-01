# cuda_notes
cuda_notes

@@@@@@@@@2017sep01
get error down below when running offcial CUDA examples provided by nvidia
##########################################################################
fatal error: helper_functions.h: No such file or directory
 #include <helper_functions.h>
##########################################################################
open Makefile

find
#INCLUDES  := -I../../common/inc

change into
INCLUDES  := -I /usr/local/NVIDIA_CUDA-8.0_Samples/common/inc


reason: need to call file(s) helper_functions.h, user needs to provide its location.
##########################################################################
