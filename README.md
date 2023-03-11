adwaita-solarized-qt
====================

adwaita-solarized-qt is a fork of [adwaita-qt][adw-qt] with a focus on the
[solarized][solarized] color scheme.

It is recommended to be used together with the GTK3 and GTK4 styles from
[adw-gtk3][adw-gtk3] and the [solarized][adw-colors-solarized] colors from
[adw-colors][adw-colors]. For GTK2 there is no perfect option, but my
discontinued [numix-solarized][numix-solarized] is an okay stand-in until GTK2
dies or an adw-gtk2 theme is made.

[solarized]: https://ethanschoonover.com/solarized/
[adw-qt]: https://github.com/FedoraQt/adwaita-qt
[adw-gtk3]: https://github.com/lassekongo83/adw-gtk3
[adw-colors]: https://github.com/lassekongo83/adw-colors
[adw-colors-solarized]: https://github.com/lassekongo83/adw-colors/blob/main/themes/solarized/gtk.css
[numix-solarized]: https://github.com/Ferdi265/numix-solarized-gtk-theme

Original README below:

adwaita-qt
==========

A native style to bend Qt5/Qt6 applications to look like they belong into GNOME Shell.

This style provides all four variants of GTK Adwaita theme:

* Adwaita
![Widget Factory](data/screenshots/widgets-adwaita.png)

* Adwaita-dark
![Widget Factory](data/screenshots/widgets-adwaita-dark.png)

* HighContrast
![Widget Factory](data/screenshots/widgets-highcontrast.png)

* HighContrastInverse
![Widget Factory](data/screenshots/widgets-highcontrastinverse.png)

## How to compile

The project uses the standard CMake buildsystem.

So for example, the whole compilation process could look like this:

```
mkdir build
cd build
cmake -DCMAKE_INSTALL_PREFIX:PATH=/usr [-DUSE_QT6] ..
make
make install
```

## Usage

After install, you'll be able to either set the theme as your default via your DE's tools (like `systemsettings` or `qt-config`) or start your qt applications with the `-style adwaita` parameter.
