set (HEADERS_PATH ${CMAKE_SOURCE_DIR}/headers)
set (
    HEADERS_FILE ${HEADERS_PATH}/Company.h 
    ${HEADERS_PATH}/Head.h ${HEADERS_PATH}/Human.h 
    ${HEADERS_PATH}/Manager.h ${HEADERS_PATH}/Worker.h
    ${HEADERS_PATH}/Teams.h
)
set (SRC_FILE main.cpp Company.cpp Head.cpp Human.cpp Manager.cpp Worker.cpp Teams.cpp)

add_executable(run ${SRC_FILE} ${HEADERS_FILE})

target_include_directories(run PUBLIC ${CMAKE_SOURCE_DIR}/headers)