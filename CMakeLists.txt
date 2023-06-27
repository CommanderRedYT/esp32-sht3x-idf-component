set(COMPONENT_ADD_INCLUDEDIRS ".")

set(COMPONENT_SRCS
    sht3x.c
    sht3x.h
)

idf_component_register(
    SRCS
        ${COMPONENT_SRCS}
    INCLUDE_DIRS
        ${COMPONENT_ADD_INCLUDEDIRS}
    REQUIRES
        driver esp_rom
)
