cmake_minimum_required(VERSION 3.10)
project(BayesLocalization)

set(CMAKE_CXX_STANDARD 14)

if (UNIX)
    # Silence warnings in Eigen
    add_compile_options(-Wno-deprecated-register)
endif()



add_executable(BayesLocalization
    ${CMAKE_SOURCE_DIR}/src/main.cpp
)

target_link_libraries(BayesLocalization)
