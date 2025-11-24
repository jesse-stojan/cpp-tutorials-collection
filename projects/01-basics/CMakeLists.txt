
set(TARGET CPP_01_Basics)

set(INC_DIR ${CMAKE_CURRENT_SOURCE_DIR}/inc)
set(SRC_DIR ${CMAKE_CURRENT_SOURCE_DIR}/src)

set(PRIVATE_HEADERS
    ${INC_DIR}/app.hh
)

set(SRC_FILES
    ${SRC_DIR}/main.cpp
)

add_executable(${TARGET})
target_sources(${TARGET}
    PRIVATE
        ${SRC_FILES}
        ${PRIVATE_HEADERS}
)
target_include_directories(${TARGET}
    PRIVATE
        ${INC_DIR}
)
