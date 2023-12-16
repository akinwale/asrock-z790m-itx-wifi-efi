# ASRock Z790M-ITX WiFi EFI
EFI for the ASRock Z790M-ITX WiFi with OpenCore 0.9.7. macOS Sonoma 14.1.2 installed.

** Note: This is still a work in progress and configuration settings are likely to change very drastically **

### Current Status
* Boots.
* No graphics acceleration with iGPU.

### BIOS Settings
#### Enabled
* Clever Access Memory (Resizable BAR)
* Intel VT-d
* Intel Virtulisation Techology
* SATA Operation: AHCI
* XHCI Hand-off

#### Disabled
* Secure Boot
* Fast Boot
* CFG Lock
* CSM Compatibility

### Hardware
| Component        | Model                              |
| ---------------- | ---------------------------------- |
| CPU              | Intel Core i7-14700K               |
| Motherboard      | ASRock z790M-ITX WiFi              |
| RAM              | 32GB (2 x 16GB) Corsair @ 5200MT/s |
| GPU              | N/A (in transit)                   |
| OS Disk          | WD_BLACK SN850X 1TB                |
| WiFi / Bluetooth | on-board Intel*                    |
