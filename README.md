**Dell Inspiron 7460 Sonoma EFI with Unsupported BCM Wifi cards**

_This only works on Sonoma 14.3.1 and below as 14.4 blocked any patches._

I already created CSR-ACTIVE-ARG codes for you to patch root easily on OCLP (SIP Disable), MinKernel Values for Wi-FI Kexts as well as Blocking com.apple.iokit.skywalkfamily on OCConfigurator.

Special Thanks to HowieHye who laid the ground work for the DSDT patches for Dell Inspiron 7460, I already included his patches to this build

https://github.com/HowieHye/Dell-7460-Hackintosh-OC

Instructions:
1. Open OpenCore Configurator and mount your EFI partition
2. Delete EFI Folder and Replace it with the EFI that you downloaded

   (In case you are on Multiboot DELETE EFI/OC FOLDER AND REPLACE IT WITH THE OC FOLDER FROM THE DOWNLOADED EFI)
4. Restart your PC
5. Open OpenCore Legacy Patcher (I also proveded this on Applications.zip), Click Post-Install Root Patch and then Start Root Patching
   
![Screenshot 2024-03-18 at 1 06 36 PM](https://github.com/ervinavales/Hackintosh-Inspiron-7460-Sonoma/assets/66302821/6abf1d08-80d1-4d9e-8308-82312da7766b)

6. Reset NVRAM once on boot
7. You should have a working Wi-Fi after reboot

![Screenshot 2024-03-18 at 1 10 16 PM](https://github.com/ervinavales/Hackintosh-Inspiron-7460-Sonoma/assets/66302821/419b6357-aa18-428d-99a3-7b5a7ef08857)

For Intel Wi-Fi/BT cards download airportitwlm kext file and paste it on EFI/OC/Kexts
Download link: https://github.com/OpenIntelWireless/itlwm

**Known Issues for this build**
1. DRM doesn't work for Prime Video, Apple TV
2. Touchpad kext is a bit buggy (Disabled it for now)
3. Palm Rejection doesn't work
4. AirDrop doesn't work on BCM (Deleted Kexts since it doesn't work)
5. Bluetooth doesn't work on BCM (Deleted Kexts since it doesn't work)