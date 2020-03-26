# Clover configuration for MSI GE72 2QE
MSI GE72 2QE Hackintosh configuration for macOS Catalina 10.15.3

## Hardware

* CPU: Intel i7-4720HQ Haswell
* GPU: Intel HD4600
  * ID: 0x416
* Chipset: Intel HM87
* Memory 8GB*1
* Audio: Realtek ALC892
* Network: Qualcomm Atheros Killer E2200
* WiFi: Intel(R) Dual Band Wireless-AC 3160
* SSD: PLEXTOR-256M7VG

## Kexts

* ACPIBatteryManager.kext - battery.
* Lilu.kext - kext patcher. Requires various plugins:
  * WhateverGreen.kext - Intel integrated video driver.
  * VirtualSMC.kext - Advanced SMC emulation.
  * AppleALC.kext - Native macOS HD audio for not officially supported codecs.
* VoodooPS2Controller_v1.9.2.kext - keyboard and Synaptics touchpad driver.
* AtherosE2200Ethernet.kext - network card driver.
* USBInjectAll.kext - disable unused USB ports.

## What is working

* GPU Acceleration (for success work and avoiding 8 apples required UEFI+CSM settings in BIOS)
* Battery indicator
* Backlight (F7 AND F8)
* Sound
* Touchpad with gestures
* SSD
* Network
* USB ports
* Web camera

Do not allow system to sleep, it cause your system gets stuck! close it in setting menu.