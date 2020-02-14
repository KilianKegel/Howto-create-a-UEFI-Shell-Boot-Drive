# HowTo-create-a-UEFI-Shell-Boot-Device

1. format the _USB Flash device_ with FAT32
2. create the directories _\EFI\BOOT_ on that formatted device
3. download _shell.efi_ from https://github.com/tianocore/edk2/blob/edk2-stable201903/ShellBinPkg/UefiShell/X64/Shell.efi 
4. rename _shell.efi_ to _BOOTX64.efi_
5. copy _BOOTX64.efi_ to the boot device into the folder _\EFI\BOOT_ - that's it
6. make sure, that on the platform SECURE BOOT is disabled in BIOS Setup!
7. adjust boot order to start UEFI Shell boot device

If you want to run PYTHON, here is the installation package:<br>
https://github.com/chipsec/chipsec/blob/master/__install__/UEFI/chipsec_uefi_x64.zip


