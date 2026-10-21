# Ultimate Weather, 4.3 inch

Freenove FNK0115B, 480 by 272. The pages match the 7 inch desk. The picture is drawn at 800 by 480 and fitted onto this glass.

Version on the desk: 1.0

## Folders

`ota` is what the desk downloads.
CHECK reads `ota/version.txt`.
INSTALL reads `ota/sky_43.bin`.

This desk uses

https://github.com/stefi01/Ultimate-Weather-Station-Earthquake-Lightning-ISS-4.3-inch

The 7 inch desk uses a different page and a different bin.

`sketch/ultimate_weather` is the sketch. It holds `ultimate_weather.ino`, `usa_map.h`, `iss_world.h`, and the XPT2046 touch files. Open that folder in the Arduino IDE. The folder name matches the sketch name.

`libraries` is GFX Library for Arduino 1.6.8 and TJpg_Decoder 1.1.0.
Copy both folders into your Arduino libraries folder.
This sketch does not use ArduinoJson.

`ARDUINO-IDE.txt` is the Tools menu for this board.

`Ultimate-Weather-User-Manual.pdf` is the printed manual.

## Update from the desk

SET, then ABOUT, then CHECK FOR UPDATES.
If `ota/version.txt` is a higher number than the version on the desk, tap INSTALL.
Leave the desk plugged in until it restarts.

A desk already on 1.0 says the newest firmware is already installed.
Raise the version in the sketch and in `ota/version.txt` together when you ship a newer bin.
Flash this export from USB once so the board is pointed at this page.
