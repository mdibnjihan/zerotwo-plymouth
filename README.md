# About
Zero Two dance Plymouth theme is a funny theme that will enable your linux boot menu to show the funny Zero-Two Dance boot animation. </br>
![Desktop - 1](https://user-images.githubusercontent.com/101347202/216816149-c7b5f340-96d7-4e55-9f3f-243a6f861633.png)

# Installation

+ For **debian**(Ubuntu, Kubuntu) based distros-
```bash
# make sure you have the packages for plymouth
sudo apt install plymouth
# after downloading or cloning themes, copy the selected theme in plymouth theme dir
sudo cp -r zerotwo /usr/share/plymouth/themes/
# install the new theme (zerotwo, in this case)
sudo update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/zerotwo/zerotwo.plymouth 100
# select the theme to apply
sudo update-alternatives --config default.plymouth
#(select the number for installed theme, zerotwo in this case)
# update initramfs
sudo update-initramfs -u
``` 

Enjoy! UwU
