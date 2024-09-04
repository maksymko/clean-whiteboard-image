# Clear Whiteboard Image

GIMP Script-Fu script for cleaning the whiteboard images.  This version is
intended to be used non-interactively, in batch mode.  Currently processes only
one image.

## Install

Copy to the GIMP's `script-fu` directory, in my case it's
`~/.config/GIMP/2.10/scripts`. Obviously will vary depending on the version.

```shell
DEST=~/.config/GIMP/2.10/scripts
cp clean-whiteboard-photo.scm ${DEST}
```

Can also use `gimptool` if you have it:

```shell
gimptool --install-script clean-whiteboard-photo.scm
```

## Use from the Command Line

WARNING: This overwrites the original file !!!

```shell
FILENAME=IMG_1111.jpg
gimp -c -i -b '(clean-whiteboard-photo "IMG_1111.jpg")' -b '(gimp-quit 0)'
```
