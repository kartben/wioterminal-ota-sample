# Welcome to wioterminal-ota-sample 👋
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](/LICENSE)
[![Twitter: kartben](https://img.shields.io/twitter/follow/kartben.svg?style=social)](https://twitter.com/kartben)
[![PlatformIO CI](https://github.com/kartben/wioterminal-ota-sample/workflows/PlatformIO%20CI/badge.svg)](https://github.com/kartben/wioterminal-ota-sample/actions?query=workflow%3A%22PlatformIO+CI%22)
This sample application shows you how to perform an over-the-air (OTA) update of the application running on your Wio Terminal. It s

As [PlatformIO](https://platformio.org/) [supports](https://docs.platformio.org/en/latest/boards/atmelsam/seeed_wio_terminal.html) the Wio Terminal, the sample comes in the form a PlatformIO project. 
This means that you don't have to worry about installing the [multiple Arduino libraries](https://wiki.seeedstudio.com/Wio-Terminal-Network-Overview/) the Wio Terminal requires for Wi-Fi & TLS, as well as the HTTP Client and OTA Helper needed for the OTA operations. All dependencies are automatically fetched from Github by the PlatformIO Library Manager.

In order to run the sample, just update the ``ssid`` and ``password`` variables in [``main.cpp``](src/main.cpp) with your Wi-Fi SSID and password.

```cpp
const char *ssid = "<your-ssid>";      // your network SSID
const char *password = "<your-password>"; // your network password
```

Use the [PlatformIO IDE](https://marketplace.visualstudio.com/items?itemName=platformio.platformio-ide) (VS Code extension) or the [PlatformIO command-line interface](https://platformio.org/install/cli) to deploy the application to your Wio Terminal. 

Once running, the sample will connect to the Wi-Fi network that you have configured earlier, and will try to download the binary firmware passed to the `enterURL()` function. If the operation succeeds, the device automatically reboots and runs the new firmware. You can follow the progress of the operation by monitoring the device's serial output.

## Author

👤 **Benjamin Cabé**

* Website: https://blog.benjamin-cabe.com
* Twitter: [@kartben](https://twitter.com/kartben)
* Github: [@kartben](https://github.com/kartben)
* LinkedIn: [@benjamincabe](https://linkedin.com/in/benjamincabe)

## 🤝 Contributing

Contributions, issues and feature requests are welcome!

Feel free to check [issues page](https://github.com/kartben/wioterminal-ota-sample/issues).

## Show your support

Give a ⭐️ if this project helped you!


## 📝 License

Copyright &copy; 2021 [Benjamin Cabé](https://github.com/kartben).
Copyright (c) 2015 Volodymyr Shymanskyy (from [Blynk library](https://github.com/blynkkk/blynk-library/blob/master/examples/Blynk.Edgent/Edgent_Wio_Terminal/OTA.h)) 

This project is [MIT](/LICENSE) licensed.

***
_This README was generated with ❤️ by [readme-md-generator](https://github.com/kefranabg/readme-md-generator)_
