# ArchInstallScript
This script belongs to Ermanno Ferrari. I have tewaked it according to my needs.

### Note: I have yet to test this script.

## Arch Basic Install Commands-Script

In this repository you will find packages-scripts for the base install of Arch Linux

Make the script executable with chmod +x scriptname and then run with ./scriptname.
Install the base packages and make sure to include git so that you can clone the repository in chroot.

A small summary:

1. Connect to Network with iwctl
2. Refresh the servers with pacman -Syy
3. Partition the disk
4. Format the partitions
5. Mount the partitions
6. Install the base packages into /mnt (pacstrap /mnt base linux linux-firmware git vim intel-ucode (or amd-ucode))
7. Generate the FSTAB file with genfstab -U /mnt >> /mnt/etc/FSTAB
8. Chroot in with arch-chroot /mnt
9. Download the git repository with git clone [https://github.com/AnukulPoudel/ArchInstallScript]
10. chmod +x installArch.sh
11. run with ./installArch.sh
