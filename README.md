# ASRock Z790M-ITX WiFi EFI
EFI for the ASRock Z790M-ITX WiFi with OpenCore 0.9.7.

* **BIOS Version:** 9.01
* **macOS Version:** Sonoma 14.1.2
* **Processor:** i7-14700K

_**Note: This is still a work in progress and configuration settings are likely to change very drastically.**_

## Current Status
* Boots.
* No graphics acceleration with iGPU.

## USB Port Mapping
Ports mapped using Hackintool. The system case is a Lian Li Dan A4-H2O case with a front panel having only 1 USB-C port and 1 USB A port, so all ports are functional. 16 ports are listed below, but I disabled the LED Controller port since I have no LEDs connected. The descriptions in the table are only for some important observations made when mapping. All other ports are on the motherboard, unless otherwise specified.
| Port | Description                                         |
|------|-----------------------------------------------------|
| HS01 | Front panel USB-C with a USB2 device connected      |
| HS03 | Front panel USB-A with a USB2 device connected      |
| HS04 | Motherboard USB 2 port (black)                      |
| HS05 |                                                     |
| HS06 | Motherboard USB-C port with a USB2 device connected |
| HS07 | Should be a USB 3 port on the motherboard? However, only got USB2 speeds with a USB3 flash drive connected.                                       |
| HS09 |                                                     |
| HS10 |                                                     |
| HS13 | LED Controller. Disabled.                           |
| HS14 | IOUSBHostDevice (Bluetooth)                         |
| SS01 | Motherboard USB-C port with a USB3 device connected |
| SS03 |                                                     |
| SS04 |                                                     |
| SS05 |                                                     |
| SS06 | Front panel USB-C with a USB3 device connected      |
| SS08 | Front panel USB-A with a USB3 device connected      |

## BIOS Settings

### Enabled
| Setting                        | Where?                           |
| ------------------------------ | -------------------------------- |
| Above 4G Decoding              | Advanced \ Chipset Configuration |
| C.A.M. Clever Access Memory*   | Advanced \ Chipset Configuration |
| VT-d                           | Advanced \ Chipset Configuration |
| Intel Virtualization Techology | Advanced \ CPU Configuration     |
| SATA Mode Selection: AHCI      | Advanced \ Storage Configuration | 
| XHCI Hand-off                  | Advanced \ USB Configuration     |

\* Clever Access Memory refers to Resizable BAR

### Disabled
| Setting              | Where?                       |
| -------------------- | ---------------------------- |
| CFG Lock**           | Advanced \ CPU Configuration |
| CSM                  | Boot                         |
| Fast Boot            | Boot                         |
| Intel Platform Trust | Security                     |
| Secure Boot          | Security                     |

\** Can be found after enabling **CPU C States Support**.

## Hardware
| Component        | Model                                      |
| ---------------- | ------------------------------------------ |
| CPU              | Intel Core i7-14700K                       |
| Motherboard      | ASRock Z790M-ITX WiFi                      |
| RAM              | 32GB (2 x 16GB) Crucial Pro RAM @ 5600MT/s |
| GPU              | N/A (in transit)                           |
| OS Disk          | WD_BLACK SN850X 1TB                        |
| WiFi / Bluetooth | Intel Wi-Fi 6E AX211                       |
