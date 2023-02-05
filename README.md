# About
Zero Two dance Plymouth theme is a funny theme that will enable your linux boot menu to show the funny Zero-Two Dance boot animation. </br>

![Desktop - 1](https://user-images.githubusercontent.com/101347202/216816149-c7b5f340-96d7-4e55-9f3f-243a6f861633.png)

The <b>progress bar</b> and the <b>OS name</b> is <b>not included</b>. You can modify the source files to achieve this. Follow Plymouth documention before modifying. Thank you!

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
# Plymouth
![Plymouth - logo](https://gitlab.freedesktop.org/plymouth/plymouth/-/raw/main/ply_header.svg)

Plymouth is an application that runs very early in the boot process (even before the root filesystem is mounted!) that provides a graphical boot animation while the boot process happens in the background.
It is designed to work on systems with DRM modesetting drivers. The idea is that early on in the boot process the native mode for the computer is set, plymouth uses that mode, and that mode stays throughout the entire boot process up to and after X starts. Ideally, the goal is to get rid of all flicker during startup.
For systems that don't have DRM mode settings drivers, plymouth falls back to text mode (it can also use a legacy /dev/fb interface).
In either text or graphics mode, the boot messages are completely occluded.  After the root file system is mounted read-write, the messages are dumped to /var/log/boot.log. Also, the user can see the messages at any time during boot up by hitting the escape key. <a href="https://gitlab.freedesktop.org/plymouth/plymouth">Learn more</a></br></br>
<i>Enjoy! ~ UwU ~</i>
