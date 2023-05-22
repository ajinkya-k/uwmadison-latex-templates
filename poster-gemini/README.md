# Poster Template using UW--Madison Colors and Branding

This folder contains a poster template based on the [Gemini](https://github.com/anishathalye/gemini/) beamerposter theme.

It uses fonts, colors, and logos from the University of Wisconsin--Madison [Brand and Visual Identity](https://brand.wisc.edu/)

**NOTE:** This template required `LuaLaTeX` or `XeLaTeX` for compilation.

To convert the poster to `.tiff` use [ghostscript](https://ghostscript.com/) as follows:

```bash
gswin64c \
    -sDEVICE=tiff64nc -sCompression=lzw \
    -dBATCH -dNOPAUSE  \
    -sOutputFile=poster.tiff \
    -r600 poster.pdf
```

In the above command:

 - `-sDEVICE=tiff64nc`: selects the graphics device as `tiff` with the CMYK colorscheme
 - `-dBATCH -dNOPAUSE`: uses the ghostscript program in non-interactive mode
 - `-sOutputFile=poster.tiff`: chooses `poster.tiff` as the output file name
 - `-r600`: means ghostscript will use a dpi of 600 points per inch to create the `tiff` image

Replace `gswin64c` with the appropriate `ghostscript` executable on your system.
