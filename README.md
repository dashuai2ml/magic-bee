# Magic-Bee

![](https://img.shields.io/badge/Language-C++-brightgreen) ![](https://img.shields.io/badge/License-MIT-orange)


<div align=center>
  <img src="https://github.com/dashuai2ml/magic-bee/blob/main/other/bee.png"></img>
</div>

magic-bee is an Arduino project aimed at creating a personalized full-color dot matrix pixel screen. It utilizes the ESP32-S3 DevKitC-1 as the main controller and relies on the ESP32-HUB75-MatrixPanel-I2S-DMA C++ library for functionality.

[![](https://github.com/dashuai2ml/magic-bee/blob/main/other/video.png)](//player.bilibili.com/player.html?aid=1852694718&bvid=BV1up421y7LA&cid=1493747455&p=1)


## Features

* Personalized full-color dot matrix pixel screen
* Utilizes ESP32-S3 DevKitC-1 as the main controller
* Relies on ESP32-HUB75-MatrixPanel-I2S-DMA C++ library


## Usage

	1.Define the pin configurations for the display screen and SD card in your Arduino sketch.
	2.Use the provided functions and methods to interact with the screen and SD card.

## Pin Definitions

![](https://github.com/dashuai2ml/magic-bee/blob/main/doc/%E5%BC%95%E8%84%9A.png)

    /**** HUB75 GPIO mapping ****/
    // GPIO 34+ are on the ESP32 are input only!!
    // https://randomnerdtutorials.com/esp32-pinout-reference-gpios/

    #define R1_PIN  4  // library default for the esp32, unchanged
    #define G1_PIN  5  // library default for the esp32, unchanged
    #define B1_PIN  6  // library default for the esp32, unchanged
    #define R2_PIN  7  // library default for the esp32, unchanged
    #define G2_PIN  15  // library default for the esp32, unchanged
    #define B2_PIN  16  // library default for the esp32, unchanged

    #define A_PIN   18  // remap esp32 library default from 23 to 33
    #define B_PIN   8  // remap esp32 library default from 19 to 32
    #define C_PIN   3   // remap esp32 library defaultfrom 5 to 22
    #define D_PIN   42  // library default for the esp32, unchanged
    #define E_PIN   1 // IMPORTANT: Change to a valid pin if using a 64x64px panel.

    #define CLK_PIN 40  // library default for the esp32, unchanged
    #define LAT_PIN 2  // library default for the esp32, unchanged
    #define OE_PIN  41  // library default for the esp32, unchanged

    /**** SD Card GPIO mappings ****/
    #define SS_PIN          10
    #define MOSI_PIN        11
    #define MISO_PIN        13
    #define CLK_PIN         12


## License

This project is licensed under the MIT License - see the LICENSE file for details.
