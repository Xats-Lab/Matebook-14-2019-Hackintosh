# Hackintosh for MateBook 14 2019 👨‍💻

## Description 📄

🚀 Transform your MateBook 14 2019 into a Hackintosh and experience macOS on your own hardware setup! Dive into the world of Hackintoshing with your MateBook's specifications:

| Specification     | Details               |
|-------------------|-----------------------|
| Model             | MateBook 14           |
| CPU               | Whiskey Lake i5 8265u |
| Memory            | DDR3L 8GB             |
| Graphics          | UHD620@MX250          |
| Storage           | WD SN720 512GB        |
| Audio             | Realtek ALC256        |
| LCD               | 2160x1440 resolution  |
| BIOS              | Version 1.26          |

This project brings to life a fully functional Hackintosh with key features already driven:

- CPU Turbo Boost
- intel UHD620 Graphics Card
- Wake from Sleep
- Recording and Playback
- Speaker and Headphone Output
- Touchpad and Gestures
- USB 3.0 and 2.0 Compatibility
- HiDPI Display
- HDMI Output
- Bluetooth
- Wi-Fi (Intel wireless card)

Currently Not Supported:

- Camera
- MX250 Graphics Card
- Fingerprint and TouchID

Please note that Hackintoshing involves modifying your hardware and installing macOS, which might void warranties and have potential risks. This guide is intended for educational and experimental purposes.

## Compatibility ⚙️

- MateBook 14 2019
- macOS Ventura 13.5.1 (22G90)

## Prerequisites 📋

- Basic understanding of computer hardware and software.
- USB drive with sufficient storage for macOS installation.
- Backup of important data before attempting any changes.
- Patience and willingness to troubleshoot issues.

## Installation Steps ⬇️

This project does **not** provide a detailed guide for installing macOS, you may need [related informations](#acknowledgments-👏) for help. Instead, it provides a prebuilt EFI folder that can be used to boot macOS on your MateBook 14 2019. You will need to modify the `EFI/OC/config.plist`, prepare the macOS installer, configure your BIOS/UEFI settings yourself.

1. **Preparation:**
   - Download the macOS Ventura 13.5.1 installer(Choose one).
      - [Download-macOS](https://github.com/Comp-Labs/Download-macOS)
      - [Follow OpenCore's guide](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/)
      - [macOShome](https://macoshome.com/hackintosh/uefistart/17045.html)(Recommended to Chinese user)
      - [Mist](https://github.com/ninxsoft/Mist)
      - etc.
   - Create a bootable USB drive using a tool like Ventoy or balenaEtcher.
   - Replace the USB drive's EFI partition with the release file.

2. **BIOS/UEFI Settings:**
   - Access your laptop's BIOS/UEFI settings by restarting and pressing the F2.
   - Configure settings recommended for Hackintoshing.
     - Disable Secure Boot
     - Disable TPM

3. **Installation:**
   - Boot from the USB drive and start the macOS installation process with `(External)` tag.
   - Format your target drive to both of GUID partition Scheme and APFS using Disk Utility during installation.
   - Install macOS on the formatted drive.
   - When rebooting in the installation process, boot from the USB drive again, but this time choose your macOS installation(without `(External)` tag).

4. **Post-Installation:**
   - After installation, mount the EFI partition, copy the release file to the mounted hard disk EFI partition 
   - boot without the USB drive again, but this time choose your macOS (without `(External)` tag).
   - Configure your system according to your preferences.

5. **Troubleshooting:**
   - If you encounter issues, refer to online Hackintosh communities for solutions.
   - Be prepared to tweak settings and try different configurations.
   - Open an issue here.

## Acknowledgments 👏

This project wouldn't have been possible without the invaluable contributions from the following projects:

- [OpenCore-Install-Guide](https://github.com/dortania/OpenCore-Install-Guide)(*Recommended to read*)
- [Acidanthera](https://github.com/acidanthera)(*OpenCore and Core Kexts*)
- [OpenIntelWireless](https://github.com/OpenIntelWireless)(*Kexts for Intel bluetooth and wifi*)

We extend our heartfelt thanks to the creators and maintainers of these repositories for their dedication and effort in the Hackintosh community.

Related repositories:
- [ske1996/matebook-13and14-OpenCore-Hackintosh](https://github.com/ske1996/matebook-13and14-OpenCore-Hackintosh)
- [frezs/MateBook14-Hackintosh](https://github.com/frezs/MateBook14-Hackintosh)
- [laozhiang/MateBook_13_14_XPro-Hackintosh](https://github.com/laozhiang/MateBook_13_14_XPro-Hackintosh)
- [K1ruo/matebook14-hack](https://github.com/K1ruo/matebook14-hack)

## Disclaimer ⚠️

- This project involves modifying hardware and software, which may void warranties or cause instability.
- Use this guide at your own risk.
- The creator of this guide is not responsible for any damage to your hardware or data.

## Contributing 🙋‍♂️

Contributions to this guide are welcome! If you find improvements or have additional tips, feel free to contribute.

## License 📜

This project is licensed under the [MIT License](LICENSE).
