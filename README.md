# zmk-module-battery-nrf-vddh-oversampling

External ZMK module that replaces the built-in `zmk,battery-nrf-vddh`
driver with a compatible variant whose ADC oversampling value is configurable.

## west.yml

```yaml
manifest:
  projects:
    - name: zmk-module-battery-nrf-vddh-oversampling
      remote: te9no
      revision: main
```

## Usage

Add the snippet to your build:

```yaml
snippet: battery-nrf-vddh-oversampling
```

Override the oversampling value if needed:

```conf
CONFIG_ZMK_BATTERY_NRF_VDDH_OVERSAMPLING_VALUE=4
```
