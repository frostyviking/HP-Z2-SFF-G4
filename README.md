![HP Z2 Small Form Factor](https://support.hp.com/doc-images/411/c06100891.jpg)

# This is not a guide, this is just a tribute.
I run this machine on a daily basis, its solid as a rock.
Thinking about putting a Radeon WX4100 in it for some gpu performance.

Learn OpenCore, don't just copypasta EFI's, kexts, .plist files, pathces,
when you find them on the wildweb. Open, read, put some brain's into it,
learn something. You owe it to ALL creators, contributors before you.

Fun and frustrating at times =)

**[Dont forget to unzip "unzip_me.zip" in EFI/OC/Resources]**


## Specs:
- HP Z2 Small Form Factor G4
- BIOS: Q50 Ver. 01.07.00 04/28/2021
- CPU: Intel® Core i9-9900K @ 3.60 GHz processor
- GPU: Intel® UHD Graphics 630 (2 DisplayPorts)
- Memory: 4 x 8GB Samsung DDR4-2667
- Pri LAN: Asus XG-C100C 10GbE "AQC107" (en3) 
- Sec LAN: Intel® I219-LM GbE (en0)
- WLAN/BT: BCM94360NG 2.4&5G WiFi Bluetooth 4.0 (en1)
- Audio: Conexant CX20632 5.1 HD Audio

## Current OS
- macOS Monterey 12.0.1 (Build 21A559)

## Bootloader
- OpenCore 0.7.5

## BIOS Settings
- Advanced -> HP Sure Recover
  - All is **Off**

- Advanced -> Boot Options
  - Startup Delay 5
  - Disable **Fast Boot**
  - Disable **CD-ROM Boot**
  - Enable **USB Storage Boot**
  - Disable **Network (PXE) Boot**
  - After Power Loss **Power Off**
  - UEFI & Legacy Boot order, is up to you.
  
- Advanced -> Secure Boot Configuration
  - Select **Legacy Support Disable and Secure Boot Disable**
  - Everything else unchecked.

- Advanced -> System Options
  - Enable **Turbo-boost**
  - Enable **Hyperthreading**
  - Enable **Multi-processor**
  - Enable **Virtualization Technology (VTx)**
  - Disable **Virtualization Technology for Directed I/O (VTd)**
  - Enable **Allow PCIe/PCI SERR# Interrupt**
  - Everything else unchecked.

- Advanced -> Built-in Device Options
  - Enable **Embedded LAN Controller**
  - Disable **Wake on LAN**
  - Disable **Dust Filter**
  - Video memory size **512MB**
  - Enable **Audio Device**
  - Enable **Microphone**
  - Enable **Internal Speakers**
  - Idle Fan Speed set @ **10%**
  - Enable **M.2 USB / Bluetooth**
  - Everything else unchecked.

- Advanced -> Port Options
  - Disable **eSATA Port**
  - Everything else **Enabled**
  - Restrict USB Devices **Allow all USB Devices**

- Advanced > Option ROM Launch Policy
  - Configure Option ROM Launch Policy **All UEFI**

- Advanced -> Power Management Options
  - Runtime Power Management **Enable**
  - Extended Idle Power States **Enable**
  - S4/S5 Maximum Power Savings **Disable**
  - SATA Power Management **Enable**
  - Allow waking from S4/S5 via keyboard/mouse **Disable**
  - Unique Sleep State Blink Rates **Disable** 

- Advanced -> Remote Management Options
  - Intel Management Engine is **enabled**
  - Everything else unchecked or greyed out.

- Advanced -> Slot Settings
  - All slots **enabled** and **auto**
