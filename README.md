# macbook-mtrack-settings
MacOS-feel MacBook trackpad settings using X11 and xf86-input-mtrack.

## Dependences

There's an X11 window server in your OS with [xf86-input-mtrack][xf86-input-mtrack] driver installed. For ArchLinux it's done by:

```bash
pacman -S xorg
pacaur -S xf86-input-mtrack     # it's from AUR
```

## How to apply?

```bash
cp *.conf /etc/X11/xorg.conf.d/
```

## How to fine tune my settings?

1. Pointer Acceleration. Checkout the pointer-accel.conf and [xorg.conf(5)] for thedocument.
2. Three Finger Selection/Dragging Pointer Acceleration. Checkout the mtrack.conf and modify the "SwipeSensitivity" option.
3. 4 finger Swipe Switching Workspace. That's depending on what window manager/desktop environment you're using. Just bind Button9 and Button8 for next and prev actions respectively.

[xorg.conf]: https://jlk.fjfi.cvut.cz/arch/manpages/man/xorg.conf.5
[xf86-input-mtrack]: https://github.com/BlueDragonX/xf86-input-mtrack
