# ASRock Z790M-ITX WiFi EFI
EFI for the ASRock Z790M-ITX WiFi with OpenCore 0.9.7.

* **BIOS Version:** 9.01
* **macOS Version:** Sonoma 14.1.2
* **Processor:** i7-14700K

_**Note: This is still a work in progress and configuration settings are likely to change very drastically.**_

## Current Status
* Boots.
* No graphics acceleration with iGPU.

## BIOS Settings

### Enabled
| Setting                       | Where?                           |
| ----------------------------- | -------------------------------- |
| Above 4G Decoding             | Advanced \ Chipset Configuration |
| C.A.M. Clever Access Memory*  | Advanced \ Chipset Configuration |
| VT-d                          | Advanced \ Chipset Configuration |
| Intel Virtulization Techology | Advanced \ CPU Configuration     |
| SATA Mode Selection: AHCI     | Advanced \ Storage Configuration | 
| XHCI Hand-off                 | Advanced \ USB Configuration     |

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
| Motherboard      | ASRock z790M-ITX WiFi                      |
| RAM              | 32GB (2 x 16GB) Crucial Pro RAM @ 5200MT/s |
| GPU              | N/A (in transit)                           |
| OS Disk          | WD_BLACK SN850X 1TB                        |
| WiFi / Bluetooth | on-board Intel*                            |
