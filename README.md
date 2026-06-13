![Build Status](https://github.com/LonFas/klein-kbd/actions/workflows/build.yml/badge.svg)

# 🎹 Klein Firmware & Configuration

This repository contains the custom firmware, my keymap configurations, and build artifacts for the **Klein** split ergonomic keyboard. 

The keymap is designed to be easily modified using a graphical user interface.

---

## 🛠️ Tech Stack & Tools

* **Keyboard:** [snsten/Klein](https://github.com/snsten/Klein) – A sleek, ergonomic split keyboard.
* **Firmware:** [ZMK Firmware](https://zmk.dev/) (customized layout).
* **Original Firmware:** [snsten/Klein-zmk](https://github.com/snsten/Klein-zmk) – The original firmware repository for reference.
* **Keymap Editor:** [Keymap Editor](https://nickcoutsos.github.io/keymap-editor/) – A web-based visual layout configurator.

---

## 🚀 Quick Start

### 1. Visual Keymap Editing
To modify the keymap layout using a user-friendly interface:
1. **Fork or clone** this repository.
2. Open the [Keymap Editor](https://nickcoutsos.github.io/keymap-editor/).
3. Grant the Keymap Editor application access to your repository.
4. Make your changes visually - the tool will automatically commit them back to your GitHub repo.

### 2. Building and Flashing
> [!IMPORTANT]  
> Make sure to put your controllers into bootloader mode (usually by double-tapping the reset button) before flashing.

1. Compile the firmware (via GitHub Actions or locally).
2. Download the `firmware.uf2` (or `.hex`) files for both the **left** and **right** halves.
3. Connect the controller via USB and drag-and-drop the respective file onto the storage drive.

---

## ⌨️ Current Layout Overview

*Here is a brief summary of the layers configured in this repo:*

| Layer | Type | Description |
| :--- | :--- | :--- |
| `0` | **Default** | Standard QWERTY |
| `1` | **Special** | Functional keys (`F1`-`F12`), navigation arrows. |
| `2` | **Media** | Numbers, media controls and BLE management |
| `3` | **Mouse** | Mouse emulator layer |

---

## 📂 Repository Structure

```text
├── .github/workflows/       # Automated build pipelines (if applicable)
├── config/                  # Main configuration directory
│   ├── klein.keymap         # The core keymap file (editable via GUI)
│   └── klein.conf           # Hardware and features configuration
└── README.md                # You are here!
```

## 🤝 Acknowledgements

* Thanks to [snsten](https://github.com/snsten) for the amazing Klein keyboard design.
* Special thanks to [Nick Coutsos](https://github.com/nickcoutsos) for the invaluable Keymap Editor tool.

