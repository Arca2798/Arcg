# Arcg
Personal archlinux themes for vm

If installing from manjaro:

curl -o /etc/pacman.d/mirrorlist https://archlinux.org/mirrorlist/all/https/ | vim /etc/pacman.d/mirrorlist | pacman -S arch-install-scripts



Packages

pacstrap -K /mnt base base-devel zsh vim networkmanager mtools dosfstools git plasma sddm curl git linux linux-lts linux-headers linux-firmware acpi  grub efibootmgr firefox nautilus



Genfstab -U /mnt /mnt/etc/fstab


useradd -m -G wheel -p /bin/bash user

vim /etc/locale.gen | locale-gen

git clone https://aur.archlinux.org/yay-bin.git

yay -S gnome-terminal-transparency



grub-install --target=x86_64-efi --efi-directory=/boot --bootloader-id=
grub-mkconfig -o /boot/grub/grub.cfg



Grub Theme

https://www.gnome-look.org/p/2235245


Gnome Theme

https://github.com/devansharora18/dotfiles

