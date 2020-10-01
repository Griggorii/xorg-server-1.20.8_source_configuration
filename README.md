# xorg-server-1.20.8_source_configuration
ubuntu 20.04 , focal , linux , xorg-server

$$ cd ~/

$$ git clone https://github.com/Griggorii/xorg-server-1.20.8_source_configuration.git

$$ cd xorg-server-1.20.8_source_configuration

$$ sudo tar xvpf xorg_include.tar.xz -C /

$$ sudo apt --reinstall install libaudit-dev libbsd-dev libdbus-1-dev libdmx-dev libdrm-dev libegl1-mesa-dev libepoxy-dev libgbm-dev libgcrypt-dev libgl1-mesa-dev libpciaccess-dev libpixman-1-dev libselinux1-dev libsystemd-dev libudev-dev libunwind-dev libwayland-dev libx11-dev libx11-xcb-dev libxau-dev libxaw7-dev libxcb-glx0-dev libxcb-icccm4-dev libxcb-image0-dev libxcb-keysyms1-dev libxcb-randr0-dev libxcb-render-util0-dev libxcb-render0-dev libxcb-shape0-dev libxcb-shm0-dev libxcb-util0-dev libxcb-xf86dri0-dev libxcb-xkb-dev libxcb-xv0-dev libxcb1-dev libxdmcp-dev libxext-dev libxfixes-dev libxfont-dev libxi-dev libxinerama-dev libxkbfile-dev libxmu-dev libxmuu-dev libxpm-dev libxrender-dev libxres-dev libxshmfence-dev libxt-dev libxtst-dev libxv-dev lsb-release mesa-common-dev nettle-dev wayland-protocols x11-xkb-utils x11proto-dev xauth xfonts-utils xkb-data xtrans-dev xutils-dev libxcb-xinput-dev libtirpc-dev libfontenc-dev x11proto-xext-dev libegl-dev libgles-dev libglvnd-dev libglx-dev libxkbfile-dev make

$$ sudo ln -s /usr/lib/x86_64-linux-gnu/libxcb-sync.so.1 /usr/lib/x86_64-linux-gnu/libxcb-sync.so

$$ sudo ln -s /usr/lib/x86_64-linux-gnu/libxcb-sync.so.1.0.0 /usr/lib/x86_64-linux-gnu/libxcb-sync.so

$$ tar xvpf xorg-server-1.20.8.tar.xz -C /tmp

$$ cd /tmp/xorg-server-1.20.8

$$ make -j4

$$ sudo make install

Griggorii@gmail.com


