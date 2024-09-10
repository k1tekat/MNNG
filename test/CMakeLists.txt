cmake_minimum_required(VERSION 3.22.1)# создаем проект для библиотеки
project(
    test_lib
    VERSION 1.0
    DESCRIPTION "Test lib for Mobile Network New Generation"
    LANGUAGE C
)

target_link_libraries(
    header
    ${ZMQ_LIB}
    ${CZMQ_LIB}
)

target_include_directories(
    headers
    PRIVATE
    ${ZMQ_DIR}
    ${CZMQ_DIR}
    )
