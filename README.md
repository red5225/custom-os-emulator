# Custom OS Emulator

A lightweight macOS Intel app for booting x86 ISO images in an emulated PC.

## What it does

- Drag/drop or choose an ISO
- Emulates a 32-bit/legacy x86 PC
- Boots BIOS/GRUB ISOs
- Emulates VGA display
- Captures keyboard input
- Start, pause, reset, and eject controls
- macOS-style desktop UI
- Built as an x86_64 macOS app for Intel Macs

The emulator engine is v86, embedded locally in the app. v86 is an x86 PC emulator with BIOS, VGA, PS/2 keyboard and CD-ROM support.

## Build

GitHub Actions builds the macOS Intel application.

The artifact is a ZIP containing:

custom-os-emulator.app

## Compatibility

The first target is small 32-bit x86 operating systems and custom-os. The emulator can also boot many other BIOS-compatible x86 ISO images, although compatibility depends on the guest OS hardware requirements.

## License

The application shell is MIT licensed. The embedded v86 runtime remains under its own BSD-2-Clause license.
