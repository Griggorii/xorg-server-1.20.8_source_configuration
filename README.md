# xorg-server-1.20.8_source_configuration
ubuntu 20.04 , focal , linux , xorg-server

Не для новичков что бы не натворить лишнего бардака в системе после может не завестись система и надо все дорабатывать как пример как я разрабатывал в течений пяти лет операционную систему https://www.youtube.com/watch?v=GBAtFq2aD8E по этому работа очень сложная и любая выкладка таких наработок заняла бы миллионы человеко часов по этому тут я уже предоставляю почти готовую систему как та на которой еще не с паразитировали и нету черных рамок вокруг белых виджетов http://chng.it/WDfJZLPgZZ проблемы установки тут https://youtu.be/MVhZ_QZGxaQSource full https://github.com/Griggorii/xorg-server-1.20.8/releases/tag/xorg-serverDump ubuntu 20.04 objective libsxorg-server-1.20.8.tar.xz inpack /tmp$ sudo mv /usr/include/pciaccess.h /usr/include/xorg/ && sudo rm /usr/include/pciaccess.hOnly real technologies, not any fictional parasitic distributions all it corporation support real technology investments and donate VISA 4817 7601 8112 4706 thanks

$ cd ~/

$ git clone https://github.com/Griggorii/xorg-server-1.20.8_source_configuration.git

$ cd xorg-server-1.20.8_source_configuration

$ sudo tar xvpf xorg_include.tar.xz -C /

$ sudo tar xvpf include_xorg_update.tar.xz -C /

$ sudo apt update && sudo apt --reinstall install libaudit-dev libbsd-dev libdbus-1-dev libdmx-dev libdrm-dev libegl1-mesa-dev libepoxy-dev libgbm-dev libgcrypt-dev libgl1-mesa-dev libpciaccess-dev libpixman-1-dev libselinux1-dev libsystemd-dev libudev-dev libunwind-dev libwayland-dev libx11-dev libx11-xcb-dev libxau-dev libxaw7-dev libxcb-glx0-dev libxcb-icccm4-dev libxcb-image0-dev libxcb-keysyms1-dev libxcb-randr0-dev libxcb-render-util0-dev libxcb-render0-dev libxcb-shape0-dev libxcb-shm0-dev libxcb-util0-dev libxcb-xf86dri0-dev libxcb-xkb-dev libxcb-xv0-dev libxcb1-dev libxdmcp-dev libxext-dev libxfixes-dev libxfont-dev libxi-dev libxinerama-dev libxkbfile-dev libxmu-dev libxmuu-dev libxpm-dev libxrender-dev libxres-dev libxshmfence-dev libxt-dev libxtst-dev libxv-dev lsb-release mesa-common-dev nettle-dev wayland-protocols x11-xkb-utils x11proto-dev xauth xfonts-utils xkb-data xtrans-dev xutils-dev libxcb-xinput-dev libtirpc-dev libfontenc-dev x11proto-xext-dev libglvnd-dev libxkbfile-dev make ninja-build meson xserver-xspice libspice-protocol-dev xorg-sgml-doctools x11proto-dev x11proto-core-dev libxdmcp-dev xtrans-dev libpthread-stubs0-dev libxcb1-dev x11proto-xext-dev libxdamage-dev libgl-dev icu-devtools libdatrie-dev libthai-dev libpango1.0-dev librsvg2-dev libx11-xcb-dev libxcb-glx0-dev libxcb-randr0-dev libxcb-shape0-dev libxcb-xfixes0-dev libxcb-sync-dev libxcb-present-dev libxfixes-dev libxkbfile-dev libdrm-dev libxshmfence-dev libfribidi-dev libpng-dev libsepol1-dev libx11-dev libxcb-dri3-dev libffi-dev libxcb-shm0-dev libgraphite2-dev libxcb-dri2-0-dev libexpat1-dev uuid-dev libxext-dev x11proto-xf86vidmode-dev libgif-dev libxrender-dev libicu-dev libblkid-dev libpcre2-dev libselinux1-dev libpcre3-dev libxxf86vm-dev libjpeg-dev libwayland-dev libfreetype6-dev mesa-common-dev libmount-dev libfontconfig1-dev libxfont-dev libglvnd-dev libglib2.0-dev libgl1-mesa-dev libcairo2-dev libxft-dev libegl1-mesa-dev libharfbuzz-dev libglvnd-core-dev libepoxy-dev libgdk-pixbuf2.0-dev libbsd-dev libpciaccess-dev libgcrypt20-dev libgpg-error-dev nettle-dev libsystemd-dev xmlto libcap-ng-dev libdmx1 libxcb-xf86dri0 libxmu-headers libaudit-dev libcap-ng-dev libdmx-dev libdmx1 libxaw7-dev libxcb-icccm4-dev libxcb-image0-dev libxcb-keysyms1-dev libxcb-render-util0-dev libxcb-util0-dev libxcb-xf86dri0 libxcb-xf86dri0-dev libxcb-xinput-dev libxcb-xkb-dev libxcb-xv0-dev libxmu-dev libxmu-headers libxmuu-dev libxpm-dev libxres-dev libxt-dev libxv-dev xutils-dev -y

$ sudo apt --reinstall install libpciaccess-dev -y

$ sudo libegl-dev libgles-dev libglx-dev libgles-dev libglx-dev libegl-dev libopengl-dev libjpeg-turbo8-dev libjpeg8-dev libxcb-util-dev

$ sudo ln -s /usr/lib/x86_64-linux-gnu/libxcb-sync.so.1 /usr/lib/x86_64-linux-gnu/libxcb-sync.so

$ sudo ln -s /usr/lib/x86_64-linux-gnu/libxcb-sync.so.1.0.0 /usr/lib/x86_64-linux-gnu/libxcb-sync.so

$ sudo mv /usr/include/pciaccess.h /usr/include/xorg/ && sudo rm /usr/include/pciaccess.h

$ sudo ln -s /usr/bin/x86_64-linux-gnu-ar /usr/bin/ar

$ tar xvpf xorg-server-1.20.8.tar.xz -C /tmp

$ tar xvpf build_stable.tar.xz  -C /tmp/xorg-server-1.20.8

$ cd /tmp/xorg-server-1.20.8

$ make -j4

Problem build make error reconfigure command $ ./configure --prefix=/usr --exec_prefix=/usr

$ sudo make install

$ sudo strip -s '/lib/xorg/Xorg' '/lib/xorg/Xorg.wrap' /lib/xorg/modules/* /lib/xorg/modules/drivers/* /lib/xorg/modules/extensions/* /lib/xorg/modules/input/*

 2)

$ cd /tmp/xorg-server-1.20.8/build

$ sudo mkdir /root

$ ninja install

Ninja fix problem libc-<version> command $ /usr/bin/meson --internal regenerate && ninja install

$ sudo strip -s '/lib/xorg/Xorg' '/lib/xorg/Xorg.wrap' /lib/xorg/modules/* /lib/xorg/modules/drivers/* /lib/xorg/modules/extensions/* /lib/xorg/modules/input/*

Dev remove:

$ sudo apt purge xserver-xspice libspice-protocol-dev xorg-sgml-doctools x11proto-dev x11proto-core-dev libxdmcp-dev xtrans-dev libpthread-stubs0-dev libxcb1-dev x11proto-xext-dev libxdamage-dev libgles-dev libglx-dev libgl-dev libegl-dev libopengl-dev icu-devtools libdatrie-dev libthai-dev libpango1.0-dev librsvg2-dev libx11-xcb-dev libxcb-glx0-dev libxcb-randr0-dev libxcb-shape0-dev libxcb-xfixes0-dev libxcb-sync-dev libxcb-present-dev libxfixes-dev libxkbfile-dev libjpeg-turbo8-dev libdrm-dev libxshmfence-dev libfribidi-dev libpng-dev libsepol1-dev libx11-dev libxcb-dri3-dev libffi-dev libxcb-shm0-dev libgraphite2-dev libxcb-dri2-0-dev libexpat1-dev uuid-dev libxext-dev x11proto-xf86vidmode-dev libgif-dev libjpeg8-dev libxrender-dev libicu-dev libblkid-dev libpcre2-dev libselinux1-dev libpcre3-dev libxxf86vm-dev libjpeg-dev libwayland-dev libfreetype6-dev mesa-common-dev libmount-dev libfontconfig1-dev libxfont-dev libglvnd-dev libglib2.0-dev libgl1-mesa-dev libcairo2-dev libxft-dev libegl1-mesa-dev libharfbuzz-dev libglvnd-core-dev libepoxy-dev libgdk-pixbuf2.0-dev libbsd-dev libpciaccess-dev libgcrypt20-dev libgpg-error-dev nettle-dev libsystemd-dev xmlto dblatex dblatex-doc docbook-xml docbook-xsl fonts-gfs-baskerville fonts-gfs-porson libalgorithm-c3-perl libapache-pom-java libb-hooks-endofscope-perl libb-hooks-op-check-perl libclass-c3-perl libclass-c3-xs-perl libclass-data-inheritable-perl libclass-method-modifiers-perl libclass-xsaccessor-perl libcommons-logging-java libcommons-parent-java libdata-optlist-perl libdevel-callchecker-perl libdevel-caller-perl libdevel-globaldestruction-perl libdevel-lexalias-perl libdevel-stacktrace-perl libdist-checkconflicts-perl libdynaloader-functions-perl libemail-date-format-perl libeval-closure-perl libexception-class-perl libfile-homedir-perl libfile-which-perl libfontbox-java libipc-shareable-perl liblog-dispatch-perl liblog-log4perl-perl libmail-sendmail-perl libmime-charset-perl libmime-lite-perl libmime-types-perl libmodule-implementation-perl libmodule-runtime-perl libmro-compat-perl libnamespace-autoclean-perl libnamespace-clean-perl libpackage-stash-perl libpackage-stash-xs-perl libpadwalker-perl libparams-classify-perl libparams-util-perl libparams-validationcompiler-perl libpdfbox-java libreadonly-perl libref-util-perl libref-util-xs-perl librole-tiny-perl libsombok3 libspecio-perl libsub-exporter-perl libsub-exporter-progressive-perl libsub-identify-perl libsub-install-perl libsub-name-perl libsub-quote-perl libsys-hostname-long-perl libunicode-linebreak-perl libvariable-magic-perl libxstring-perl libyaml-tiny-perl preview-latex-style sgml-data t1utils texlive texlive-base texlive-bibtex-extra texlive-binaries texlive-extra-utils texlive-fonts-recommended texlive-lang-greek texlive-latex-base texlive-latex-extra texlive-latex-recommended texlive-pictures texlive-plain-generic texlive-science tipa xml-core xmlto xsltproc -y
 
$ sudo apt purge libcap-ng-dev libdmx1 libxcb-util-dev libxcb-xf86dri0 libxmu-headers libaudit-dev libcap-ng-dev libdmx-dev libdmx1 libxaw7-dev libxcb-icccm4-dev libxcb-image0-dev libxcb-keysyms1-dev libxcb-render-util0-dev libxcb-util-dev libxcb-util0-dev libxcb-xf86dri0 libxcb-xf86dri0-dev libxcb-xinput-dev libxcb-xkb-dev libxcb-xv0-dev libxmu-dev libxmu-headers libxmuu-dev libxpm-dev libxres-dev libxt-dev libxv-dev xutils-dev libsystemd-dev xmlto -y

$ sudo apt autoremove -y

# xorg-server-1.20.8 , waylandxorg-server , xorg-server-1.20.8 , objective , replace find include <pciaccess.h> to <xorg/pciaccess.h> , danger x11 session priority only wayland

Test translate EN: https://translate.google.com/translate?hl=&sl=en&tl=en&u=https%3A%2F%2Fgithub.com%2FGriggorii%2Fxorg-server-1.20.8_source_configuration

На данный момент по скольку у меня модифицированный дистрибутив то войти после установки можно будет только в сессию wayland видимо это связано что мне надоел инклюд pciaccess.h в общих инклюдах и я его переопределил в xorg , а предположительно после всяких различных разработок приходится пересобирать и mesa драйвер , а он еще не пересобран , но это не точно и какие то другие de отличные от org.gnome могут заработать например xfce я могу где то ошибаться позднее проверю на обычной операционной системе без модификации пока вот так https://github.com/Griggorii/xorg-server-1.20.8/blob/main/Not_XWAYLAND_LINUX_0S.20.04.png <-(может сделаем третью сессию для убунты без X? X11 , XWayland , Wayland) все дело в том что в моем модифицированном дистрибутиве есть по мимо /lib/x86_64-linux-gnu/pkgconfig есть еще и /lib/pkgconfig что позволяет получить еще одну очищенную или подсахаренную генерацию которою нельзя получить другим образом и только взять у меня и выдать за свою в корпорации и получить многомиллионный грант соответственно за меня лучше конечно что бы не было смещений брать ubuntu 21.04 и в ней перекомпилировать objective код и тогда это не заденет иксовую сессию с помощью модифицированного в 20.04 pkg дев инструмента для этого с помощью zsync я (с паразитировал с помощью своего готового образа) свой собственный образ https://github.com/Griggorii/ubuntu-21.04-hirsute-desktop-amd64-griggorii-zsync.isoПочему я делаю акцент на то что бы корпорации ит вели моим счет наработкам дело в том что я вырастил самую удачную архитектуру за пять лет и лучшие портажи которые теперь можно перекинуть на любую другую архитектуру включая телефоны , планшеты , телевизоры и будет лучшая производительность , но в случае сговора ит я не стал инвестируемым и нет я не планировал стать Билл Гейтсом или Торвальдсом я работал именно на качество и естественно цель моя как видите по результатам была не только заработать , но и дать лучшие наработки для портажей я даже не понимаю почему сам гугл пользуясь такими мощными наработками не поднял меня на его партнерки и все такое ведь если бы я запатентовал портажи то пришлось мне платить очень много , а мне хватит и допустим миллиона долларов за весь пакет наработок включая chromium os 77 как только это все это реализуется и корпорации перестанут играть в дурачка вида (я у корпорации пупер девелопер за 399ка) и кто понял о чем я то мир получит 1.20.4 xorg gold золотой за счет того что в нем изначально не было тиринга генерации я уже сделал.

Griggorii@gmail.com пишем сюда если хотите поддерживать технологии переноса дампа и поддержать от крупных компании по производству видео техники где вендорам нужны видео драивера будь то вы от фирмы lenovo , samsung , sony и других вендоров я открыл уже достаточно много техно фишек , но мне демонетезировали даже видео канал на ютубе методом административного государственного давления . По этому я могу принять крипто валютами что бы этим не благодарным тем более ничего не досталось даже как с самозанятого ведь они спонсируют только всяких рогозинов и других. Вы долны помнить тот диалог где звучало следующее в стране плохие дороги , а зачем вам машина раз дороги плохие , мужику надо было парировать типа , а зачем вам мозг если вы им думать не умеете ? А , зачем вам лекарства вы все равно скоро умрете ? А , зачем вам протезы вы все равно инвалид на машине ? А , зачем вам квартира вы все равно нищий и все в таком духе я не понимаю как туда еще атомную бомбу не запустили в этот россадник ? А , потом бы позвонили и спросили нужны ли им будут деньги через +15 минут если они через 10 все рвно будут мертвы. Все скоро подорожает так что знайте и думайте нужен ли этот бесполезный монолит в качестве кремля который уже является типом пирамиды мавроди и получают только возле пирамиды , но не понимают они пока все не разделяться на отдельные страны что бы доход был не только у пирамиды которая производит только звуки , а цены подлетят потому что когда на что то цена взлетает то это идет по цепочке т.е те кто наценил цены в стране ни чего не выйграют по скольку то что он ранее брал по пять рублей будет теперь стоить 10 , а кто же цены контролирует наверное некий орган ЦБ он же и повышает цену на услуги при том это происходит в стране где рубль не растет по отношению к валютам , а еще и бесконечно падает пробивая не то что бы некую глубину , а уже и дно соответственно и зарплату не прибавят в течении как минимум пяти лет.


