# floor-heating-controller

ESPHome project to expose up to 8x relays and temperature sensors to HomeAssistant

## Highlights

* Plain simple actuator board
* HW available on Aliexpress, super cheap
* Provides temperature of incoming hot/warm water


## ESP32 relay board

* 17.5€, bought on Aliexpress: https://it.aliexpress.com/item/1005007027676026.html?spm=a2g0o.order_list.order_list_main.31.42f53696cth4st&gatewayAdapt=glo2ita
Main characteristics are:

  * ESP32-WROOM-32E module
  * 5V DC power supply terminal
  * 8 relay channels, both NC and NO contacts available

* 4€, 220V to 5V power adapter (5W), bought on Aliexpress
* Temperature sensor, bought on Aliexpress


## ESPHome setup

Aliexpress board pinout:

* GPIO23: led D20
* GPIO13: relay 1
* GPIO12: relay 2
* GPIO14: relay 3
* GPIO27: relay 4
* GPIO26: relay 5
* GPIO25: relay 6
* GPIO33: relay 7
* GPIO32: relay 8

Please note that GPIO12 is a strapping PIN and should only be used for I/O with care.
Attaching external pullup/down resistors to strapping pins can cause unexpected failures.
See https://esphome.io/guides/faq.html#why-am-i-getting-a-warning-about-strapping-pins

