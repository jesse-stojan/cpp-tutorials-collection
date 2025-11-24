
set(TARGET CPP_00_Intro)

set(SRC_DIR ${CMAKE_CURRENT_SOURCE_DIR}/src)
# set(INC_DIR ${CMAKE_CURRENT_SOURCE_DIR}/inc)

set(SRC_FILES
    ${SRC_DIR}/main.cpp
)

add_executable(${TARGET})
target_sources(${TARGET}
    PRIVATE
        ${SRC_FILES}
)
