# St (Suckless Terminal)

My custom terminal build based on (lukesmith's build only for ligatures) with some additional patches like newterm, rightclick paste, desktop entry,sixel, live-reload xresources, anygeometry etc!.

## Patches:

- Ligatures
- sixel (check sixel branch)
- scrollback
- Clipboard
- Alpha(Transparency)
- Boxdraw
- patch_column ( doesnt cut text while resizing)
- font2
- right click paste
- st desktop entry
- newterm
- anygeometry
- xresources
- sync patch ( Better draw timing to reduce flicker/tearing and improve animation smoothness )
- live reload ( change colors/fonts on the fly )
  and more...


## Xresources live-reload

```
 #make an alias for this command

alias load="kill -USR1 $(pidof st)"
alias  use="xrdb merge"

command : use Xresourcesfile && load
```

## Install

`cd st && make && sudo make install`


## Keybindings

```
alt + n                 open a new terminal with same cwd ( current working directory )
alt + c                 Copy
alt + v                 Paste
alt + down              scroll down
alt + up                scroll up
alt + shift + k         Zoom in
alt + shift + j         Zoom out
alt + comma             Zoom in
alt + .                 Zoom out
alt + g                 Reset Zoom
alt + s                 Increase Transparency
alt + a                 Decrease Transparency
copy anything and right click on the terminal ( will paste the copied thing )
```
you can change all of these in config.h

