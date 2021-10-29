![HP Z2 Small Form Factor](https://support.hp.com/doc-images/411/c06100891.jpg)

# This is not a guide, this is just a tribute.
I run this machine on a daily basis, its solid as a rock.
Thinking about putting a Radeon WX4100 in it for some gpu performance.

Learn OpenCore, don't just copypasta EFI's, kexts, .plist files, pathces,
when you find them on the wildweb. Open, read, put some brain's into it,
learn something. You owe it to ALL creators, contributors before you.

Fun and frustrating at times =)


## Specs:
- HP Z2 Small Form Factor G4
- BIOS: 
- CPU: Intel® Core i9-9900K @ 3.60 GHz processor
- GPU: Intel® UHD Graphics 630 (2 DisplayPorts)
- Memory: 4 x 8GB Samsung DDR4-2667
- Pri LAN: Asus XG-C100C 10GbE "AQC107" (en3) 
- Sec LAN: Intel® I219-LM GbE (en0)
- WLAN/BT: BCM94360NG 2.4&5G WiFi Bluetooth 4.0 (en1)
- Audio: Conexant CX20632 5.1 HD Audio

## BIOS Settings
- Advanced -> Boot Options
  - Startup Delay 5
  - Disable **Fast Boot**
  - Disable **CD-ROM Boot**
  - Enable **USB Storage Boot**
  - Disable **Network (PXE) Boot**
  - After Power Loss **Power Off**
  - UEFI & Legacy Boot order, is up to you.
  
- Advanced -> Secure Boot Configuration
  - Select **Legacy Support Enable and Secure Boot Disable**
  - Everything else unchecked.

- Advanced -> System Options
  - Enable **Turbo-boost**
  - Enable **Hyperthreading**
  - Enable **Multi-processor**
  - Enable **Virtualization Technology (VTx)**
  - Disable **Virtualization Technology for Directed I/O (VTd)**
  - Enable **M.2 WLAN/BT**
  - Enable **M.2 SSD**
  - Enable **Allow PCIe/PCI SERR# Interrupt**
  - Power Button Override **4 sec**

- Advanced -> Built-in Device Options
  - Enable **Embedded LAN Controller**
  - Disable **Wake on LAN**
  - Disable **Dust Filter**
  - Video memory size **64MB**
  - Enable **M.2 USB / Bluetooth**
  - Enable **Audio Device**
  - Enable **Internal Speakers**
  - Increase Idle Fan Speed (%), set at 0

- Advanced -> Port Options
  - Everything **Enabled**
  - Restrict USB Devices **Allow all USB Devices**

- Advanced > Option ROM Launch Policy
  - Configure Option ROM Launch Policy **All UEFI**

- Advanced -> Power Management Options
  - Runtime Power Management **Enable**
  - Extended Idle Power States **Enable**
  - S5 Maximum Power Savings **Disable**
  - SATA Power Management **Enable**
  - PCI Express Power Managment **Disable**
  - Power On from Keyboard Ports **Disable**
  - Unique Sleep State Blink Rates **Disable** 

- Advanced -> Remote Management Options
  - I have not touched anything in here, running defaults AFAIK..


## Current OS
- macOS Monterey 12.0.1 (Build 21A559)

## Bootloader
- OpenCore 0.7.5
