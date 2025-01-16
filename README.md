# Arcg
Personal archlinux themes for vm



Mirrors
curl -o /etc/pacman.d/mirrorlist https://archlinux.org/mirrorlist/all/https/

fstab
Genfstab -U /mnt /mnt/etc/fstab

Packages
pacstrap -K /mnt base base-devel lvm2 vim networkmanager mtools dosfstools git plasma sddm curl linux linux-lts linux-headers linux-firmware acpi  grub efibootmgr firefox 

useradd -m -G wheel -p /bin/bash user

AUR
https://aur.archlinux.org/yay-bin.git
gnome-terminal-transparency
brave-browser-bin
surfshark

Grub

grub-install --target=x86_64-efi --efi-directory=/boot --bootloader-id=
grub-mkconfig -o /boot/grub/grub.cfg

Grub Theme
https://www.gnome-look.org/p/2235245

Gnome Theme
https://github.com/devansharora18/dotfiles

Pacman.conf 

Ilovecandy
