idf_component_register(
    SRCS "wsl_bypasser.c"
    INCLUDE_DIRS "interface"
    REQUIRES esp_event esp_wifi
)
target_link_libraries(${COMPONENT_LIB} -Wl,-zmuldefs)