# PIN Brute Force Script

This script simulates a brute force attempt to enter all possible 4-digit PIN combinations (`0000` to `9999`) on a device. It acts as a USB HID keyboard and sends keypresses to the target device.

## Features

- **Brute Force:** The script goes through all 10,000 possible 4-digit PIN combinations (from `0000` to `9999`).
- **Keyboard Emulation:** It simulates typing the PINs and pressing `Enter` for each attempt.

## Prerequisites

- **Hardware Requirements:**
  - A device running **Sprig** or a similar microcontroller acting as a USB HID keyboard.
  - The device must be connected to the phone, PC, or any system you want to interact with via USB.

- **Software Requirements:**
  - **CircuitPython** or **MicroPython** installed on the device.
  - The `adafruit_hid` library should be available for use in your CircuitPython setup.

## How It Works

1. The script starts by sending the PIN `0000` and pressing `Enter`.
2. It then proceeds to the next combination (`0001`) and repeats the process until `9999`.
3. Each PIN combination is sent one at a time with a short delay (`1 second`), and `Enter` is pressed after each.
4. After attempting all combinations, the script terminates.

## Installation

1. **Download the script** and upload it to your **Sprig** device running CircuitPython.
2. Ensure the device is recognized as a **USB HID keyboard** by the connected system (phone, PC, etc.).
3. Upload the code to your device and execute the script.

