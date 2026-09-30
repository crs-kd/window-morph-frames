# Window morph frames

Frame sequence for the CR Smith Lorimer window scroll module, hosted here for
testing. Served over GitHub Pages so the module can be checked on a real
Unbounce page before the frames move to crsmith.co.uk.

Desktop composites two layers every frame. The window is only 45.5% of the
frame width, so scaling the whole picture up to give the welds the resolution a
screen can actually show would spend most of the memory on wallpaper and a sofa
that carry no detail. Instead:

    frames/bg/000.webp … 049.webp     the room, 800x450
    frames/win/000.webp … 049.webp    the window cropped at its own full
                                      resolution, 1500x1130, with the edge
                                      feathered in its alpha so the join
                                      between the soft background and the
                                      sharp inset falls on plain wallpaper
    frames/sm/000.webp … 024.webp     mobile, single layer, 900px
    frames/still/first.webp           both ends held, full 3840x2160
    frames/still/last.webp

The welds end up at 1252px against the 1310px a 1440 screen can show, for
0.38 GB of decoded bitmap.

Rendered from the Blender morph file. Not the source of truth for anything:
re-render, re-convert, re-upload.
