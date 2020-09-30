# xorg-server-1.20.8_source_configuration
ubuntu 20.04 , focal , linux , xorg-server

$$ sudo tar xvpf xorg_include.tar.xz -C /

$$ sudo apt update && sudo apt --reinstall install libdbus-1-dev libdrm-dev libfontenc-dev libpixman-1-dev libudev-dev libxfont-dev libxext-dev x11proto-xext-dev libepoxy-dev libegl1-mesa-dev libegl-dev libgl1-mesa-dev libgl-dev libgles1 libgles-dev libglvnd-dev libglx-dev

$$ tar xvpf xorg-server-1.20.8.tar.xz -C /tmp

$$ cd /tmp/xorg-server-1.20.8

$$ make -j4

$$ sudo make install


