# 🤖 flipper-xiaomi-filter-reset - Reset Xiaomi air purifier filter life easily

[![](https://img.shields.io/badge/Download-Latest_Release-blue.svg)](https://github.com/rashithawaragoda-code/flipper-xiaomi-filter-reset/releases)

This application allows you to reset the filter life counter on your Xiaomi air purifier. It uses the NFC capabilities of your Flipper Zero to communicate with the NTAG213 chip inside the filter. This tool saves you money by extending the use of filters that still function correctly. 

## 📋 Requirements

Before you start, ensure you have the following items:

* A Flipper Zero device.
* A computer running Windows 10 or Windows 11.
* A USB-C cable to connect your Flipper Zero.
* The latest official Flipper Zero firmware installed on your device.

## 📥 How to download and install

Follow these steps to obtain the app and move it to your Flipper Zero.

1. Go to the [official release page](https://github.com/rashithawaragoda-code/flipper-xiaomi-filter-reset/releases) to access the files.
2. Look for the file ending in the extension .fap. This is the application file for your device.
3. Click the file name to save it to your computer.
4. Plug your Flipper Zero into your computer using the USB cable.
5. Open the qFlipper desktop application on your computer.
6. Click the File Manager icon on the left side of the qFlipper window.
7. Open the folder named 'apps'.
8. Open the subfolder named 'nfc'.
9. Drag and drop the downloaded .fap file from your computer into the 'nfc' folder on the Flipper Zero.
10. Wait for the transfer to finish.
11. Disconnect your Flipper Zero from the computer.

## ⚙️ How to use the app

Once the file is on your device, you can run it through the Flipper Zero menu.

1. Press the middle button on your Flipper Zero to open the main menu.
2. Select the 'Applications' folder.
3. Locate and select the 'NFC' folder.
4. Choose the 'Xiaomi Filter Reset' application from the list.
5. Hold the Flipper Zero near the NFC tag located on the Xiaomi air purifier filter.
6. Press the 'Read' button on the screen to view the current status of your filter.
7. If you decide to reset the life counter, select the 'Reset' option in the menu.
8. Keep the Flipper Zero steady while it writes the new data to the tag.
9. Verify the success message on your screen.

## 💡 Understanding the filter status

The application displays specific information about your filter health. 

* **Remaining Life:** This shows the percentage of usage left before the air purifier software prompts you to buy a new filter.
* **Usage Time:** This displays the total time the filter remained in use.
* **Chip ID:** This represents the unique identifier for the NTAG213 chip.

You can reset the filter life at any time. Use this feature if you cleaned your filter or if the sensor reported a low life incorrectly.

## 🛠️ Troubleshooting common issues

If you encounter problems during the process, check these solutions:

* **Device not detected:** Ensure the USB cable connects properly to both your computer and the Flipper Zero. Try a different USB port if the connection fails.
* **App does not launch:** Confirm that you placed the .fap file in the correct folder on your device. Ensure your Flipper firmware is up to date through qFlipper.
* **Read error:** Move the Flipper Zero closer to the filter tag. External interference might cause issues, so ensure no other metal objects remain near the filter during the scan.
* **Write error:** Check that the filter is not locked. Some filters allow only one reset cycle.

## 🛡️ Safety precautions

This software interacts with the electronics of your filter. While the process is safe, follow these guidelines:

* Do not physically damage the NFC tag area on the filter.
* Ensure you use clean air filters only. A clogged or damaged filter compromises the air quality in your room.
* Keep the Flipper Zero away from high-heat sources.

Keywords: air-purifier, fap, flipper-zero, flipper-zero-app, flipperzero, mifare-ultralight, nfc, ntag213, reverse-engineering, xiaomi