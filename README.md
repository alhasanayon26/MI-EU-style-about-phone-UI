# MI-EU Specs UI for HyperOS

A systemless module that enables the **Xiaomi EU-style "About Device" specifications interface** on HyperOS. Compatible with **Magisk**, **KernelSU**, and **KernelSU Next**, this module allows users to customize and display their device specifications in the About Device section, similar to the Xiaomi EU ROM experience.

Unlike a plug-and-play module, this package requires a one-time configuration before installation. Users must edit the included configuration file with their own device specifications to ensure the information displayed is accurate.

---

## Features

- 📱 Xiaomi EU-style About Device specifications layout
- ✨ Customizable device information
- ⚡ Lightweight and systemless implementation
- 🔒 Compatible with **Magisk**, **KernelSU**, and **KernelSU Next**
- ♻️ Easy to modify and update
- 🚀 Enhances the HyperOS About Device interface
- 💯 Stable and optimized for daily use

---

## Requirements

- HyperOS
- Root access
- **Magisk**, **KernelSU**, or **KernelSU Next**

---

## Installation Guide

> **⚠️ Important:** Do **NOT** flash this module directly. It must be configured before installation.

### Step 1

Download the latest release and extract the ZIP using a file manager such as:

- MiXplorer
- MT Manager

### Step 2

Navigate to:

```text
/system/product/etc/
```

Locate the file:

```text
device_info.json
```

### Step 3

Open `device_info.json`.

The file will look similar to this:

```json
{
  "basic": {
    "CPU": "",
    "Battery": "",
    "Camera": "",
    "Screen": "",
    "Resolution": ""
  },
  "camera": {
    "front_camera": "",
    "rear_camera": ""
  }
}
```

### Step 4

Fill in each empty field with your device's actual specifications.

Example:

```json
{
  "basic": {
    "CPU": "Snapdragon 8 Elite",
    "Battery": "6000mAh",
    "Camera": "50MP + 50MP + 50MP",
    "Screen": "6.67-inch AMOLED",
    "Resolution": "3200 × 1440"
  },
  "camera": {
    "front_camera": "32MP",
    "rear_camera": "50MP + 50MP + 50MP"
  }
}
```

### Step 5

Save the edited file.

### Step 6

Repack the extracted files into a ZIP archive.

### Step 7

Flash the newly created ZIP using:

- Magisk
- KernelSU
- KernelSU Next

### Step 8

Reboot your device.

The customized Xiaomi EU-style specifications will now appear in the **About Device** section.

---

## Compatibility

- Xiaomi devices
- Redmi devices
- POCO devices
- Supported HyperOS versions

> Compatibility may vary depending on your device model and HyperOS version.

---

## Credits

Original MI-EU Specs UI module created by **Harsh10R - https://t.me/AboutHarshZXR **.

This repository contains my adapted version with packaging and usage instructions for compatible HyperOS devices.

---

## Disclaimer

This module is provided **as-is** without any warranty. Modifying system components always carries a degree of risk. You are responsible for any issues, including bootloops or data loss, resulting from the installation or use of this module. Always create a backup before making system modifications.

---

## License

Please respect the original author's work and any applicable licenses associated with the original project.
