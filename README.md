york-font
===

![york-font](./york-font.jpg?raw=true)

### What Is This?

A font derived from [Droid
Sans](https://en.wikipedia.org/wiki/Droid_(typeface)) compiled into
a single convenient `.ttf` file.

Specifically, York is created using the following process:

1. Obtain `DroidSans.ttf`.
2. Obtain `DroidSansFallbackFull.ttf`. This second `.ttf` file
   contains most of the non-Latin glyphs.
3. Open `DroidSansFallbackFull.ttf` in [FontForge](https://fontforge.org/en-US/)
   and change the Em size from `256` to `2048` to match
   the value in `DroidSans.ttf`.
4. Open `DroidSans.ttf` in FontForge, and merge the rescaled
   `DroidSansFallbackFull.ttf` file into it.
5. Adjust metadata to ensure that people don't mix this up with
   the real Droid Sans.
6. Save the result to `York.ttf`.

### Why?

There was a requirement for a font that could be rendered
at sizes down to 10pt without antialiasing and without
looking terrible, and covered a decent amount of the Unicode
[BMP](https://en.wikipedia.org/wiki/Plane_(Unicode)#Basic_Multilingual_Plane).

Droid Sans was the only font that really met these requirements.
DejaVu Sans was a close second, but has only 5119 glyphs compared to
the ~50000 glyphs in Droid Sans. Noto Sans has better glyph coverage
than Droid, but renders poorly at small sizes without antialiasing.
Additionally, IBM Plex Sans has good coverage, but also renders
unpleasantly at small sizes without antialiasing.

### License

https://spdx.org/licenses/Apache-2.0

