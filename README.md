# HowTo-create-a-UEFI-Shell-Boot-Device

 1. format the _USB Flash device_ with FAT32
 2. create the directories _\EFI\BOOT_ on that formatted device
 3. download _shell.efi_ from https://github.com/tianocore/edk2/tree/master/ShellBinPkg/UefiShell/X64
 4. rename _shell.efi_ to _BOOTX64.efi_
 5. download _shell.efi_ from https://github.com/tianocore/edk2/tree/master/ShellBinPkg/UefiShell/Ia32
 6. rename _shell.efi_ to _BOOTIA32.efi_
 7. download _shell.efi_ from https://github.com/tianocore/edk2/tree/master/ShellBinPkg/UefiShell/Arm
 8. rename _shell.efi_ to _BOOTARM.efi_
 9. download _shell.efi_ from https://github.com/tianocore/edk2/tree/master/ShellBinPkg/UefiShell/AArch64
10. rename _shell.efi_ to _BOOTAA64.efi_
11. copy _BOOTX64.efi_, _BOOTIA32.EFI_, _BOOTARM.EFI_ and _BOOTAA64.EFI_ to the boot device into the folder _\EFI\BOOT_ - that's it
12. make sure, that on the platform SECURE BOOT is disabled in BIOS Setup!
13. adjust boot order to start UEFI Shell boot device

