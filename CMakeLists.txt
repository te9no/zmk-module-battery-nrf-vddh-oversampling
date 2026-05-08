# SPDX-License-Identifier: MIT

if(CONFIG_ZMK_BATTERY_NRF_VDDH_OVERSAMPLING)
  zephyr_library()
  zephyr_library_sources(src/battery_nrf_vddh_oversampling.c)
endif()
