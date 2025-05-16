if ((NOT CONFIG_ZMK_SPLIT) OR CONFIG_ZMK_SPLIT_ROLE_CENTRAL)
  target_sources_ifdef(CONFIG_ZMK_BEHAVIOR_BASE_LAYER app PRIVATE src/behaviors/behavior_base-layer.c)

  zephyr_include_directories(include)
endif()
