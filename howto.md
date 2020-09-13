Create this file with: 
sudo nano /usr/share/X11/xorg.conf.d/10-nvidia-brightness.conf

Write in the file:

Section "Device"
    Identifier     "Device0"
    Driver         "nvidia"
    VendorName     "NVIDIA Corporation"
    BoardName      "GeForce RTX 2060 Mobile"
    Option         "RegistryDwords" "EnableBrightnessControl=1"
EndSection
