# HowTo-create-a-UEFI-Shell-Boot-Device

1. format the _USB Flash device_ with FAT32
2. create the directories _\EFI\BOOT_ on that formatted device
3. download _shell.efi_ from:<br>https://github.com/tianocore/edk2/blob/edk2-stable201903/ShellBinPkg/UefiShell/X64/Shell.efi<BR>
   **NOTE:** Please also find <img src="https://github.com/KilianKegel/pictures/blob/master/New-icon.png"  width="18" height="18">https://github.com/KilianKegel/Visual-UEFI-SHELL to create an *up-to-date* **UEFI Shell**
4. rename _shell.efi_ to _BOOTX64.efi_
5. copy _BOOTX64.efi_ to the boot device into the folder _\EFI\BOOT_ - that's it
6. make sure, that on the platform SECURE BOOT is disabled in BIOS Setup!
7. adjust boot order to start UEFI Shell boot device

Nice to have: <br>**find** and **more** MSDOS clone for UEFI Shell:<br>

8. create the directories _\EFI\TOOLS_ on that formatted device<br>
9. download _find.efi_ and _more.efi_ from https://github.com/KilianKegel/Visual-DOS-Tools-for-UEFI-Shell/tree/master/x64/UEFIx86-64%20(Torito%20C%20Library)<br>
10. copy _find.efi_ and _more.efi_ to the boot device into the folder _\EFI\TOOLS_ - that's it

Alternative solution from [**congatec**](https://www.congatec.com/us/support/application-notes/article/an31-how-to-create-a-bootable-usb-stick-with-a-uefi-shell/).


