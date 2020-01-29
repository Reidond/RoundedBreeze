## Rounded Breeze

A Breeze kdecoration fork for KWin. Features rounded corners and a single pixel border for contrast (like on macOS).

## Screenshot

![preview](https://raw.githubusercontent.com/zephyyy/RoundedBreeze/master/preview.png)

Also [Imgur](https://imgur.com/a/EV7lF3B).

## Dependencies

There are some dependencies you'll need to install. Some people suggested using the following commands:

### Ubuntu, KDE Neon

```shell
sudo apt install git g++ extra-cmake-modules cmake gettext libkf5config-dev libkdecorations2-dev libqt5x11extras5-dev qtdeclarative5-dev libkf5guiaddons-dev libkf5configwidgets-dev libkf5windowsystem-dev libkf5coreaddons-dev libfftw3-dev
```

### Arch Linux, Manjaro, Antergos

```shell
sudo pacman -S kdecoration qt5-declarative qt5-x11extras kcoreaddons kguiaddons kconfigwidgets kwindowsystem fftw cmake extra-cmake-modules
```

### OpenSUSE

```shell
sudo zypper install git extra-cmake-modules libkdecoration2-devel kcoreaddons-devel kguiaddons-devel kconfig-devel kwindowsystem-devel ki18n-devel kconfigwidgets-devel libQt5DBus-devel libqt5-qtx11extras-devel fftw3-devel
```

## Installation

In order to install the theme and add it to your decorations do the following:

```shell
git clone https://github.com/Reidond/RoundedBreeze
cd RoundedBreeze
mkdir build
cd build
cmake .. -DCMAKE_INSTALL_PREFIX=/usr -DCMAKE_BUILD_TYPE=Release -DKDE_INSTALL_LIBDIR=lib -DBUILD_TESTING=OFF -DKDE_INSTALL_USE_QT_SYS_PATHS=ON
sudo make install
kwin_x11 --replace &
```

That is it! Your new decoration theme should appear in
_Settings &rarr; Application Style &rarr; Window Decorations_.

## Other

Use with [ShapeCorners](https://sourceforge.net/projects/shapecorners) to be able able to round any window.
