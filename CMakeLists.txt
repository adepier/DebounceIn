 
set(DEBOUNCE_SOURCES DebounceIn.cpp) 
add_library(DebounceIn STATIC ${DEBOUNCE_SOURCES})
target_link_libraries( DebounceIn mbed-os)

set(DEBOUNCE_HEADER_DIR ${CMAKE_CURRENT_SOURCE_DIR} )
target_include_directories(DebounceIn PUBLIC ${DEBOUNCE_HEADER_DIR})