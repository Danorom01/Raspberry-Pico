# Pico 2 W HID Payload Demo

A simple USB HID (BadUSB-style) project for the **Raspberry Pi Pico 2 W** using CircuitPython.

When plugged into a Windows computer, the device:
1. Opens the Run dialog
2. Launches Command Prompt
3. Changes the text color to red
4. Displays a "SYSTEM SCAN" message
5. Runs `ipconfig /all`
6. Immediately shuts down the computer

---

## ⚠️ Disclaimer

This project is for **educational purposes and authorized testing only**.  
Do **not** use it on any system you do not own or do not have explicit permission to test.

---

## Requirements

- Raspberry Pi Pico 2 W
- CircuitPython 10.x
- `adafruit_hid` library

---

## Installation

1. Flash CircuitPython for the Pico 2 W from [circuitpython.org](https://circuitpython.org/board/raspberry_pi_pico2_w/)
2. Download the CircuitPython library bundle and copy the `adafruit_hid` folder into the `lib` folder on the CIRCUITPY drive
3. Copy `code.py` to the root of the CIRCUITPY drive
4. Safely eject the drive and plug the Pico into a Windows computer

The payload will run automatically after a few seconds.

---

## Notes

- The initial 5-second delay gives Windows time to recognize the device as a keyboard.
- You can change the final command if you want a different action (restart, logoff, etc.).
