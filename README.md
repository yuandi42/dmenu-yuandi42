# README
## Screenshot
![Screenshot]{dmenu.png "Screenshot"}
## Dependency
1. [git](https://archlinux.org/packages/extra/x86_64/git/)
2. [make](https://archlinux.org/packages/core/x86_64/make/)
3. [libx11](https://archlinux.org/packages/extra/x86_64/libx11/)
4. [libxinerama](https://archlinux.org/packages/extra/x86_64/libxinerama/)
5. [libxft-bgra](https://aur.archlinux.org/packages/libxft-bgra)
## Options added
    -bw " num": dmenu appers with certain width of border.
    -F: dmenu turns off fuzzy match.
    -c: dmenu appears centered on the screen.
## Patches added / plan to add
Patch | Status |
---|---|
[center](https://tools.suckless.org/dmenu/patches/center/)  | Patched |
[fuzzymatch](https://tools.suckless.org/dmenu/patches/fuzzymatch/) | Patched|
[border](https://tools.suckless.org/dmenu/patches/border/) | Patched |
[mouse support](https://tools.suckless.org/dmenu/patches/mouse-support/) | Patched[^1] |
[xresources-alt](https://tools.suckless.org/dmenu/patches/xresources-alt/) | Unpatched[^2] |
[alpha](https://tools.suckless.org/dmenu/patches/alpha/)| Unpatched[^3] |
[gruvbox](https://tools.suckless.org/dmenu/patches/gruvbox/) | Patched |
[Allow color font](https://tools.suckless.org/dmenu/patches/allow-color-font/) | Patched[^4] |
[^1]:Left-click on item doesn't work. Quite werid.
[^2]:Seems not working correctly. Dispatched.
[^3]:Took really long time to mannauly patching, and got a strange error during
  make install, sorry and bye.
[^4]:A patch of libxft is needed.
