# My build of dmenu
Forked at Feb 14, 2022. Last patch from mainstream can be dated back to Mar 3,
2022 (some of them were patched manually). Maybe one day I will add some
patches from upstream repo.

## Screenshot
![Screenshot](screenshot.png 'Screenshot')
## Dependency
In order to build dmenu you need the Xlib header files.

And since this fork add extra unicode support, you also need Pango and Pangoxft
addtionally.

For arch users, you need packages below:
1. [git](https://archlinux.org/packages/extra/x86_64/git/)
2. [make](https://archlinux.org/packages/core/x86_64/make/)
3. [libx11](https://archlinux.org/packages/extra/x86_64/libx11/)
4. [libxinerama](https://archlinux.org/packages/extra/x86_64/libxinerama/)
5. [libxft](https://archlinux.org/packages/extra/x86_64/libxft/)
6. [pango](https://archlinux.org/packages/extra/x86_64/pango/)

## What's new?
### Multilanguage support
This fork enhances its usability for showing various kinds unicode characters.
Now my `dmenu` can correctly show letters from CKJ to even Hebrew rather
showing anonymous square.

### `dmenu_run`
When your command end with `;`, the command will be started in a terminal.
(Actually, in `$TERMINAL`. And you set the value in `.bash_profile` or
`.xporfile` or any other place.)

I have removed history function from `dmenu_run` to `dmenu_run_history`.

### Flags added
* `-bw` *num*: dmenu appers with certain width of border.
* `-F`: dmenu turns off fuzzy match.
* `-c`: dmenu appears centered on the screen.
## Patches added / plan to add
Patch | Status |
---|---|
[center](https://tools.suckless.org/dmenu/patches/center/)  | Patched |
[fuzzymatch](https://tools.suckless.org/dmenu/patches/fuzzymatch/) | Patched|
[fuzzyhighlight](https://tools.suckless.org/dmenu/patches/fuzzyhighlight/) | Patched|
[border](https://tools.suckless.org/dmenu/patches/border/) | Patched |
[mouse support](https://tools.suckless.org/dmenu/patches/mouse-support/) | Patched[^1] |
[gruvbox](https://tools.suckless.org/dmenu/patches/gruvbox/) | Patched |
[Allow color font](https://tools.suckless.org/dmenu/patches/allow-color-font/) | Patched[^2] |
[Unicode](https://github.com/akash-akya/dmenu-unicode)| Patched [^3]|

[^1]:Left-click on item doesn't work on my archlinux but works well on
  arco. Dependency problem maybe.

[^2]:A patch of libxft is needed.

[^3]:Not a patch in [suckless site](https://tools.suckless.org/dmenu/patches/)
  actually. It's a dmenu fork and I just stolen codes from its git commit.
