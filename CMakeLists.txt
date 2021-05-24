set(NETCODE_SOURCES 
    netcode.c
)

file(GLOB NETCODE_INCLUDE_FILES "netcode.h")

add_library(netcode STATIC ${NETCODE_SOURCES})

target_link_libraries(netcode)

install_our_headers(${NETCODE_INCLUDE_FILES})

set(NETCODE_LINK_WITH netcode PARENT_SCOPE)

#-----------------------------------------------------------------------------#
# vim: set ts=8 sts=4 sw=4 et:
