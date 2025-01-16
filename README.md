# Arcg
Personal archlinux command guide

If installing from manjaro:  curl -o /etc/pacman.d/mirrorlist https://archlinux.org/mirrorlist/all/https/ | vim /etc/pacman.d/mirrorlist | pacman -S arch-install-scripts


If time needs to be set: ln -sf /usr/share/zoneinfo/region/city   /etc/localtime | find region by: ls /usr/share/zoneinfo/



Packages

pacstrap -K /mnt base base-devel zsh vim networkmanager mtools dosfstools git plasma sddm curl git linux linux-lts linux-headers linux-firmware acpi  grub efibootmgr firefox nautilus bluez bluez-utils



Genfstab -U /mnt >> /mnt/etc/fstab


vim /etc/locale.gen | locale-gen


useradd -m -G wheel -p /bin/bash user


passwd

passwd user

EDITOR=vim visudo 

git clone https://aur.archlinux.org/yay-bin.git | makepkg -si

yay -S gnome-terminal-transparency



grub-install --target=x86_64-efi --efi-directory=/boot --bootloader-id=
grub-mkconfig -o /boot/grub/grub.cfg

PROMPT='%B%{$fg[cyan]%}%(4~|%-1~/.../%2~|%~)%u%b >%{$fg[cyan]%}>%B%(?.%{$fg[cyan]%}.%{$fg[red]%})>%{$reset_color%}%b '



Grub Theme

https://www.gnome-look.org/p/2235245


Gnome Theme

https://github.com/devansharora18/dotfiles

