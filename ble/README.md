# BLE

## AI usage

No AI was used for generating the code. AI was only used for learning purposes.

## How I made this

For learning the concepts, I used the [ESP-IDF BLE documentation](https://docs.espressif.com/projects/esp-idf/en/stable/esp32/api-guides/ble/get-started/ble-introduction.html) provided by Espressif Systems.

BLE rqeuires a lot of boilerplate. So I copied the [NimBLE_GATT_Server](https://github.com/espressif/esp-idf/tree/v6.1/examples/bluetooth/ble_get_started/nimble/NimBLE_GATT_Server) official example, and adapted it as per my needs. `gap.c` is full boilerplate.

## Menuconfig

You don't have to update these manually. They have been added to `sdkconfig.defaults` so they will be automatically taken care of when `sdkconfig` gets generated or regenerated.

- **Component config -> Bluetooth**: checked
- **Component config -> Bluetooth -> Host**: NimBLE - BLE only
