# README
## Screenshot
![Screenshot](dmenu.png 'Screenshot')
## Dependency
1. [git](https://archlinux.org/packages/extra/x86_64/git/)
2. [make](https://archlinux.org/packages/core/x86_64/make/)
3. [libx11](https://archlinux.org/packages/extra/x86_64/libx11/)
4. [libxinerama](https://archlinux.org/packages/extra/x86_64/libxinerama/)
5. [libxft-bgra](https://aur.archlinux.org/packages/libxft-bgra)
## What's new?
### dmenu_run
This new script can handle history in `$XDG_CACHE_HOME` and will list command
you type most on the top when you run `dmenu_run`.

And when your command end with ';', the command will be started in a terminal.
(Actually, in `alacritty`. But you can change it to your favourite terminal)

P.S. I just simply combined those
[two](https://tools.suckless.org/dmenu/scripts/dmenu_run_with_command_history)
[scripts](https://tools.suckless.org/dmenu/scripts/dmenu_run_i) together.
### Flags added
* `-bw` *num*: dmenu appers with certain width of border.
* `-F`: dmenu turns off fuzzy match.
* `-c`: dmenu appears centered on the screen.
## Patches added / plan to add
Patch | Status |
---|---|
[center](https://tools.suckless.org/dmenu/patches/center/)  | Patched |
[fuzzymatch](https://tools.suckless.org/dmenu/patches/fuzzymatch/) | Patched|
[border](https://tools.suckless.org/dmenu/patches/border/) | Patched |
[mouse support](https://tools.suckless.org/dmenu/patches/mouse-support/) | Patched[^1] |
[gruvbox](https://tools.suckless.org/dmenu/patches/gruvbox/) | Patched |
[Allow color font](https://tools.suckless.org/dmenu/patches/allow-color-font/) | Patched[^2] |
[^1]:Left-click on item doesn't work. Quite werid.
[^2]:A patch of libxft is needed.
