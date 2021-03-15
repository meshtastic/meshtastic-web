# Meshtastic-web

This is a ReactJS based front-end designed to be served by the [Meshtastic-device](https://github.com/meshtastic/Meshtastic-device) project's embedded webserver.

This project imports the [Meshtastic.js library](https://github.com/meshtastic/meshtastic.js) for communication with the device

![React App Screenshot](images/screenshot_1.png)


![Gif](images/meshtasticreactv0.5.gif)

## Installation Instructions

1. Connect your radio to your local WiFi network/router (use the python api to set this up: `meshtastic --set wifi_ap_mode false --setstr wifi_ssid mywifissid --setstr wifi_password mywifipsw`

1. Using PlatformIO or `http://meshtastic.local/static` or `http://[IP Displayed on Mestashtic Device]/static` navigate to your radio’s /static page.

1. Delete all files on SPIFFS (SPI Flash File System) using the delete links.

1. Upload the three files attached to the following page https://github.com/crossan007/meshtastic-web/releases/tag/0.1.1 5 ( index.html.gz , app.js.gz and app.css.gz )

1. Navigate to the root URL of your radio.

1. (Optional) If you want to setup softAP mode for the device use the Python API `meshtastic --set wifi_ap_mode true --setstr wifi_ssid mywifissid --setstr wifi_password mywifipsw`
