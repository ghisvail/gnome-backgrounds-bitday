# gnome-backgrounds-bitday

      ____    ______  ______  ____    ______   __    __ 
     /\  _`\ /\__  _\/\__  _\/\  _`\ /\  _  \ /\ \  /\ \
     \ \ \L\ \/_/\ \/\/_/\ \/\ \ \/\ \ \ \L\ \\ `\`\\/'/
      \ \  _ <' \ \ \   \ \ \ \ \ \ \ \ \  __ \`\ `\ /' 
       \ \ \L\ \ \_\ \__ \ \ \ \ \ \_\ \ \ \/\ \ `\ \ \ 
        \ \____/ /\_____\ \ \_\ \ \____/\ \_\ \_\  \ \_\
         \/___/  \/_____/  \/_/  \/___/  \/_/\/_/   \/_/

[BitDay], a beautiful dynamic pixel wallpaper, packaged for the GNOME desktop.


## Installation

First, ensure [Meson] is available on your system.

Then, run the following commands:

```
meson --prefix=/usr builddir
ninja -C builddir install
```


## Configuration

The default timings for the dynamic wallpaper were taken from the
[BitDay-for-Windows] configuration. They can be adjusted either in file
`backgrounds/bitday-timed.xml.in` before installation, or in file
`/usr/share/backgrounds/bitday/bitday-timed.xml` post installation.


## Licensing

This project is licensed under the same [terms](./COPYING) as
[BitDay-for-Windows] where the images were originally sourced from.


[BitDay]: https://bitday.me/
[BitDay-for-Windows]: https://github.com/DannyCare/BitDay-for-Windows/
[Meson]: https://mesonbuild.com/Getting-meson.html
