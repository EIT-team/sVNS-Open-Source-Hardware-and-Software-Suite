# sVNS-Open-Source-Hardware-and-Software-Suite
This repository serves as an index for the open-source hardware and software developed for the **implantable wireless battery-free selective vagus nerve stimulator (sVNS)**.

The project consists of four main components:

| **PCB Design** | Hardware design of the implantable 16-channel stimulator in Autodesk EAGLE.

| **Device Firmware** | Firmware running on the implantable stimulator (Silicon Labs EFM8).

| **Transmitter Firmware** | Firmware for the PN532-based NFC transmitter used for wireless powering and control.

| **Control GUI** | Python graphical user interface for configuring stimulation parameters and communicating with the transmitter.

## Repositories

### PCB Design
**sVNS_15chan_EAGLE**

Hardware design files, schematics, board layout, and manufacturing files.

https://github.com/EIT-team/sVNS_EAGLE

---

### Device Firmware
**sVNS_EFM8_firmware_2**

Firmware for the implantable stimulator based on the Silicon Labs EFM8 microcontroller.

https://github.com/EIT-team/sVNS_EFM8_firmware_2

---

### Transmitter Firmware
**sVNS_PN532**

Firmware for the PN532 NFC transmitter responsible for wireless powering and communication with the implant.

https://github.com/EIT-team/sVNS_PN532

---

### Transmitter GUI
**sVNS_GUI**

Python-based graphical user interface for configuring stimulation parameters and controlling the transmitter.

https://github.com/EIT-team/sVNS_GUI

---

## System Overview

```
┌────────────────────────┐
│      Python GUI        │
└──────────┬─────────────┘
           │ USB
           ▼
┌────────────────────────┐
│  PN532 NFC Transmitter │
└──────────┬─────────────┘
           │ 13.56 MHz NFC

           |
           ▼
┌────────────────────────┐
│ Implantable Stimulator │
│   (EFM8 + 16 channels) │
└──────────┬─────────────┘
           │
           ▼
      Vagus Nerve
```

## Citation

If you use this project in your research, please cite the preprint:

https://doi.org/10.64898/2026.04.10.717669
