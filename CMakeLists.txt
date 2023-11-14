project(FasterTransformer LANGUAGES CXX CUDA)

find_package(CUDA REQUIRED)
set(CUTLASS_DIR ${CMAKE_CURRENT_SOURCE_DIR}/cutlass)

add_subdirectory(tensorrt_llm/kernels/cutlass_kernels)
