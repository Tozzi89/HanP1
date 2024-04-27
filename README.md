# About

This is a ESPHome firmware for the HanP1 devices created by [Tozzi89](https://github.com/Tozzi89/HanP1). the code is originaly from https://github.com/psvanstrom/esphome-p1reader, with some minor modifications.

## Instructions

1. Connect HanP1 electrical meter to the RJ-12 port with included cable.
2. Use a computer/mobile and connect to the Wifi created by HanP1, the SSID is "hanp1-" with the mac adress in the end. The password is "12345678"
3. Fill in your Wifi network you would like the HanP1 to connect to (which has access to your ESPHome instance).
4. After a few minutes a new device should appear in your ESPHome panel to adopt.
5. Adopt, change name if you want, and when prompted, choose "Install".

   ESPHome should now download the rest of the yaml config from this GitHub repository and reboot once again. It should now start giving you some measurements.
   Don't forgett to add the device to your "Energy" control panel in HomeAssistant.

## Advanced users

The hardware is open source, but not for commercial purposes, however you are free to edit/modify to your liking. Inside HanP1 there is UART header and a switch to set the unit into programing mode. There is also a reset button if needed.
However, in Version 1.x there was a design error on my part, to be able to program it from the UART header you need to desolder Q1 transistor since it interferes with Rx signals on the ESP8266. Please use OTA updates if possible, the UART pins should really be only for recovery.
