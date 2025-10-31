# SETUP


## Partitions

|Partition| Mount Point | Size | Purpose|
|--|--|--|--|
|/boot/efi|FAT32|512 MB|EFI System Partition (ESP): Mandatory for modern UEFI booting|
|/|ext4|80 GB - 100 GB|Root: Contains the OS, all your programs, and system files|
|/home|ext4|Remaining Space (~400 GB)|Home: Your personal files, documents, downloads, and app settings|

## INSTALL ESSENCIALS

```sh
sudo apt update && sudo apt upgrade -y
```

Flatpak/Flathub

https://flatpak.org/setup/Ubuntu

Using flatpak install hidamari to use animated wallapaper

Install AppImageLaucher

> To handle app images instalation, once installed download the app and double click. select Integrate and run

> To change manually some configs ~/.local/share/applications/

```sh
sudo apt-get install libfuse2
```

https://github.com/TheAssassin/AppImageLauncher/releases


### Dev Essencials
```sh
sudo apt install build-essential
```
docker

https://docs.docker.com/desktop/setup/install/linux/ubuntu/
```sh
sudo apt install git
```
### Game Essencials
```sh
sudo apt install steam
```

### Gnome look Essencials

```sh
sudo apt install gnome-tweaks \
sudo apt install gnome-shell-extension-manager
```

Enable user theme in Extension

Install  
https://github.com/vinceliuice/Orchis-theme  
https://github.com/vinceliuice/Tela-icon-theme


transparent dock
```sh
gsettings set org.gnome.shell.extensions.dash-to-dock transparency-mode 'FIXED' \
gsettings set org.gnome.shell.extensions.dash-to-dock background-opacity 0.0
```

center dock icons

```sh
gsettings set org.gnome.shell.extensions.dash-to-dock extend-height false
```
