# zerotwo-plymouth
Zero Two dance Plymouth theme is a funny theme that will enable your linux boot menu to show the funny Zero-Two Dance boot animation. </br>

#How to install? </br>

<code>sudo apt install plymouth</code>
<b>Note:</b> Plymouth requires pre-implementation from the distribution itself. Refer to developer documentation for Plymouth. <a href="https://gitlab.freedesktop.org/plymouth/plymouth">Plymouth GitLab</a></br>
<code>sudo cp -r /<DIRECTORY_NAME>/zerotwo/ /usr/share/plymouth/themes/</code></br>
<code>sudo update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/zerotwo/zerotwo.plymouth 100</code></br>
<code>sudo update-alternatives --config /usr/share/plymouth/themes/plymouth.default</code></br>
Enter the number according to your installation.
<code>sudo update-initramfs -u</code>

Enjoy! UwU

