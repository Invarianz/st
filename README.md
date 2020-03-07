# Vanilla st with some sugar sprinkles
Clone of the simple terminal (st) in version 0.8.2 by [suckless.org](https://suckless.org) with terminal colors inspired by the default terminal in [vscode](https://github.com/microsoft/vscode) and DejaVu Sans Mono Font.

## Pre applied patches
Patches will be automatically applied from the `patches/` folder when make is invoked.

There are three patches applied:
- anysize (terminal will seamlessly fit with tiling window managers)
- keyboard scrollback via `Shift-PgUp/PgDn` with extra long history (20.000 lines)
- colors and font patch

## Installation
```
git clone https://github.com/Invarianz/st
cd st
sudo make install
 ```
 
For the people interested in breaking speed limits one can invoke; (e.g. in a bash shell)
```
export CFLAGS="-march=native -O3" && make
```
For this very close to vanilla build `libX11` and `libXft` are required.
