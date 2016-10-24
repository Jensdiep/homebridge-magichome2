# homebridge-magichome

**A Homebridge plugin for devices running on the Magic Home Wi-Fi system.**

The plugin includes and uses a slightly modified version of [flux_led.py](https://github.com/beville/flux_led).

## Installation

First, install the plugin globally.

````
npm install -g homebridge-magichome
````

Next, add a new accessory to your Homebridge `config.json`. You can add as many Magic Home-based accessories as you like in the following format:

````
"accessories": [
   {
       "accessory": "MagicHome",
       "name": "LED Strip",
       "ip": "192.168.1.111",
       "extrawhite": false // (OPTIONAL)
   }
]
````

The `extrawhite` option is false by default and is only required for devices that support both warm white (WW) and cool white (CW).

## Compatible Devices

Any devices created by Zengge and running on the Magic Home Wi-Fi (or other apps by the same developer such as LED Magic Color) app should work with this plugin. Some examples of compatible devices are:

- [5 Channel Controller for RGB LED Strip](http://amzn.to/2eAljEV)
- [Magic UFO RGBW LED Strip controller](http://amzn.to/2eyoRdE)
- [SuperLegends Wi-Fi smart bulb](http://amzn.to/2eCxq6a)
- [Victorstar Wi-Fi Smart Light Bulb](http://amzn.to/2eCCM13)
- [Flux Wi-Fi Light Bulb](http://amzn.to/2eCx3IC)
- [Fen-Yi Light Bulb](http://amzn.to/2ehjP3s)
- [Waterproof RGB LED Strips WIFI Controller](http://amzn.to/2eoDQZx)
- [Eastlion RGB Wi-Fi Strip Controller](http://amzn.to/2eCF8wV)

**I have only tested this myself with the first item on the list** which as far as I know is also the only product to require the `extrawhite` option. I will however be buying some of the bulbs to try soon.

Please let me know if you find any other compatible devices.