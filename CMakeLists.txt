set(CORE_SRCS
  cores/esp32/base64.cpp
  cores/esp32/cbuf.cpp
  cores/esp32/esp32-hal-adc.c
  cores/esp32/esp32-hal-bt.c
  cores/esp32/esp32-hal-dac.c
  cores/esp32/esp32-hal-gpio.c
  cores/esp32/esp32-hal-i2c.c
  cores/esp32/esp32-hal-ledc.c
  cores/esp32/esp32-hal-matrix.c
  cores/esp32/esp32-hal-misc.c
  cores/esp32/esp32-hal-sigmadelta.c
  cores/esp32/esp32-hal-spi.c
  cores/esp32/esp32-hal-time.c
  cores/esp32/esp32-hal-timer.c
  cores/esp32/esp32-hal-touch.c
  cores/esp32/esp32-hal-uart.c
  cores/esp32/Esp.cpp
  cores/esp32/HardwareSerial.cpp
  cores/esp32/IPAddress.cpp
  cores/esp32/IPv6Address.cpp
  cores/esp32/libb64/cdecode.c
  cores/esp32/libb64/cencode.c
  cores/esp32/MD5Builder.cpp
  cores/esp32/Print.cpp
  cores/esp32/stdlib_noniso.c
  cores/esp32/Stream.cpp
  cores/esp32/StreamString.cpp
  cores/esp32/wiring_pulse.c
  cores/esp32/wiring_shift.c
  cores/esp32/WMath.cpp
  cores/esp32/WString.cpp
  )

set(LIBRARY_SRCS
  libraries/ArduinoOTA/src/ArduinoOTA.cpp
  libraries/AsyncUDP/src/AsyncUDP.cpp
  libraries/BluetoothSerial/src/BluetoothSerial.cpp
  libraries/DNSServer/src/DNSServer.cpp
  libraries/EEPROM/EEPROM.cpp
  libraries/ESPmDNS/src/ESPmDNS.cpp
  libraries/FS/src/FS.cpp
  libraries/FS/src/vfs_api.cpp
  libraries/HTTPClient/src/HTTPClient.cpp
  libraries/NetBIOS/src/NetBIOS.cpp
  libraries/Preferences/src/Preferences.cpp
  libraries/SD_MMC/src/SD_MMC.cpp
  libraries/SD/src/SD.cpp
  libraries/SD/src/sd_diskio.cpp
  libraries/SD/src/sd_diskio_crc.c
  libraries/SimpleBLE/src/SimpleBLE.cpp
  libraries/SPIFFS/src/SPIFFS.cpp
  libraries/SPI/src/SPI.cpp
  libraries/Ticker/src/Ticker.cpp
  libraries/Update/src/Updater.cpp
  libraries/WebServer/src/WebServer.cpp
  libraries/WebServer/src/Parsing.cpp
  libraries/WebServer/src/detail/mimetable.cpp
  libraries/WiFiClientSecure/src/ssl_client.cpp
  libraries/WiFiClientSecure/src/WiFiClientSecure.cpp
  libraries/WiFi/src/ETH.cpp
  libraries/WiFi/src/WiFiAP.cpp
  libraries/WiFi/src/WiFiClient.cpp
  libraries/WiFi/src/WiFi.cpp
  libraries/WiFi/src/WiFiGeneric.cpp
  libraries/WiFi/src/WiFiMulti.cpp
  libraries/WiFi/src/WiFiScan.cpp
  libraries/WiFi/src/WiFiServer.cpp
  libraries/WiFi/src/WiFiSTA.cpp
  libraries/WiFi/src/WiFiUdp.cpp
  libraries/Wire/src/Wire.cpp
  )

set(AZURE_SRCS
  libraries/AzureIoT/src/az_iot/azureiotcerts.c
  libraries/AzureIoT/src/az_iot/c-utility/pal/agenttime.c
  libraries/AzureIoT/src/az_iot/c-utility/pal/dns_async.c
  libraries/AzureIoT/src/az_iot/c-utility/pal/freertos/lock.c
  libraries/AzureIoT/src/az_iot/c-utility/pal/freertos/threadapi.c
  libraries/AzureIoT/src/az_iot/c-utility/pal/freertos/tickcounter.c
  libraries/AzureIoT/src/az_iot/c-utility/pal/lwip/sntp_lwip.c
  libraries/AzureIoT/src/az_iot/c-utility/pal/socket_async.c
  libraries/AzureIoT/src/az_iot/c-utility/pal/src/platform_openssl_compact.c
  libraries/AzureIoT/src/az_iot/c-utility/pal/src/tlsio_openssl_compact.c
  libraries/AzureIoT/src/az_iot/c-utility/pal/tlsio_options.c
  libraries/AzureIoT/src/az_iot/c-utility/src/base64.c
  libraries/AzureIoT/src/az_iot/c-utility/src/buffer.c
  libraries/AzureIoT/src/az_iot/c-utility/src/connection_string_parser.c
  libraries/AzureIoT/src/az_iot/c-utility/src/consolelogger.c
  libraries/AzureIoT/src/az_iot/c-utility/src/constbuffer.c
  libraries/AzureIoT/src/az_iot/c-utility/src/constmap.c
  libraries/AzureIoT/src/az_iot/c-utility/src/crt_abstractions.c
  libraries/AzureIoT/src/az_iot/c-utility/src/doublylinkedlist.c
  libraries/AzureIoT/src/az_iot/c-utility/src/gballoc.c
  libraries/AzureIoT/src/az_iot/c-utility/src/gb_stdio.c
  libraries/AzureIoT/src/az_iot/c-utility/src/gb_time.c
  libraries/AzureIoT/src/az_iot/c-utility/src/hmac.c
  libraries/AzureIoT/src/az_iot/c-utility/src/hmacsha256.c
  libraries/AzureIoT/src/az_iot/c-utility/src/httpapiex.c
  libraries/AzureIoT/src/az_iot/c-utility/src/httpapiexsas.c
  libraries/AzureIoT/src/az_iot/c-utility/src/httpheaders.c
  libraries/AzureIoT/src/az_iot/c-utility/src/http_proxy_io.c
  libraries/AzureIoT/src/az_iot/c-utility/src/map.c
  libraries/AzureIoT/src/az_iot/c-utility/src/optionhandler.c
  libraries/AzureIoT/src/az_iot/c-utility/src/sastoken.c
  libraries/AzureIoT/src/az_iot/c-utility/src/sha1.c
  libraries/AzureIoT/src/az_iot/c-utility/src/sha224.c
  libraries/AzureIoT/src/az_iot/c-utility/src/sha384-512.c
  libraries/AzureIoT/src/az_iot/c-utility/src/singlylinkedlist.c
  libraries/AzureIoT/src/az_iot/c-utility/src/strings.c
  libraries/AzureIoT/src/az_iot/c-utility/src/string_tokenizer.c
  libraries/AzureIoT/src/az_iot/c-utility/src/urlencode.c
  libraries/AzureIoT/src/az_iot/c-utility/src/usha.c
  libraries/AzureIoT/src/az_iot/c-utility/src/vector.c
  libraries/AzureIoT/src/az_iot/c-utility/src/xio.c
  libraries/AzureIoT/src/az_iot/c-utility/src/xlogging.c
  libraries/AzureIoT/src/az_iot/iothub_client/src/blob.c
  libraries/AzureIoT/src/az_iot/iothub_client/src/iothub_client_authorization.c
  libraries/AzureIoT/src/az_iot/iothub_client/src/iothub_client.c
  libraries/AzureIoT/src/az_iot/iothub_client/src/iothub_client_ll.c
  libraries/AzureIoT/src/az_iot/iothub_client/src/iothub_client_retry_control.c
  libraries/AzureIoT/src/az_iot/iothub_client/src/iothub_message.c
  libraries/AzureIoT/src/az_iot/iothub_client/src/iothubtransport.c
  libraries/AzureIoT/src/az_iot/iothub_client/src/iothubtransportmqtt.c
  libraries/AzureIoT/src/az_iot/iothub_client/src/iothubtransport_mqtt_common.c
  libraries/AzureIoT/src/az_iot/iothub_client/src/version.c
  libraries/AzureIoT/src/az_iot/umqtt/src/mqtt_client.c
  libraries/AzureIoT/src/az_iot/umqtt/src/mqtt_codec.c
  libraries/AzureIoT/src/az_iot/umqtt/src/mqtt_message.c
  libraries/AzureIoT/src/AzureIotHub.cpp
  libraries/AzureIoT/src/Esp32MQTTClient.cpp
  )

set(BLE_SRCS
  libraries/BLE/src/BLE2902.cpp
  libraries/BLE/src/BLE2904.cpp
  libraries/BLE/src/BLEAddress.cpp
  libraries/BLE/src/BLEAdvertisedDevice.cpp
  libraries/BLE/src/BLEAdvertising.cpp
  libraries/BLE/src/BLEBeacon.cpp
  libraries/BLE/src/BLECharacteristic.cpp
  libraries/BLE/src/BLECharacteristicMap.cpp
  libraries/BLE/src/BLEClient.cpp
  libraries/BLE/src/BLEDescriptor.cpp
  libraries/BLE/src/BLEDescriptorMap.cpp
  libraries/BLE/src/BLEDevice.cpp
  libraries/BLE/src/BLEExceptions.cpp
  libraries/BLE/src/BLEHIDDevice.cpp
  libraries/BLE/src/BLERemoteCharacteristic.cpp
  libraries/BLE/src/BLERemoteDescriptor.cpp
  libraries/BLE/src/BLERemoteService.cpp
  libraries/BLE/src/BLEScan.cpp
  libraries/BLE/src/BLESecurity.cpp
  libraries/BLE/src/BLEServer.cpp
  libraries/BLE/src/BLEService.cpp
  libraries/BLE/src/BLEServiceMap.cpp
  libraries/BLE/src/BLEUtils.cpp
  libraries/BLE/src/BLEUUID.cpp
  libraries/BLE/src/BLEValue.cpp
  libraries/BLE/src/FreeRTOS.cpp
  libraries/BLE/src/GeneralUtils.cpp
  )

set(COMPONENT_SRCS ${CORE_SRCS} ${LIBRARY_SRCS} ${AZURE_SRCS} ${BLE_SRCS})

set(COMPONENT_ADD_INCLUDEDIRS
  variants/esp32/
  cores/esp32/
  libraries/ArduinoOTA/src
  libraries/AsyncUDP/src
  libraries/AzureIoT/src
  libraries/BLE/src
  libraries/BluetoothSerial/src
  libraries/DNSServer/src
  libraries/ESP32/src
  libraries/ESPmDNS/src
  libraries/FS/src
  libraries/HTTPClient/src
  libraries/NetBIOS/src
  libraries/Preferences/src
  libraries/SD_MMC/src
  libraries/SD/src
  libraries/SimpleBLE/src
  libraries/SPIFFS/src
  libraries/SPI/src
  libraries/Ticker/src
  libraries/Update/src
  libraries/WebServer/src
  libraries/WiFiClientSecure/src
  libraries/WiFi/src
  libraries/Wire/src
  )

set(COMPONENT_PRIV_INCLUDEDIRS cores/esp32/libb64)

set(COMPONENT_REQUIRES spi_flash mbedtls mdns ethernet)
set(COMPONENT_PRIV_REQUIRES fatfs nvs_flash app_update spiffs bootloader_support openssl)

register_component()