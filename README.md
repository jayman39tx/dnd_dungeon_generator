# dnd_dungeon_generator
Generates a hand-drawn-style DnD map file of a dungeon grid-map segment, with several options.

The hand-drawn effect is created with the use of a Delaunay Triangle grid, with random soft stippling.

Options available at the GUI input:

Output Image dots-per-unit ("dpi", for example): Defaults to 300, but can be set to 150, 144, 72, etc.

Image width in units ("mm" or "inches", for example): Defaults to 5, but can be set to any number. This is multiplied by the dots-per-unit value to get the total number of pixels wide of the final image.

Image height in unites ("mm" or "inches", for example): Defaults to 5, but can be set to any number. This is multiplied by the dots-per-unit value to get the total number of pixels high of the final image.

Image Folder: Select a folder to contain the resulting image file generated from this script.

Image Type/Extension: Defaults to "PNG". You can select one of six image types: PNG, GIF, JPG, PCX, TIF, or BMP

Image File Basename (without extension): defaults to "generated_map_xxxx", where "xxxx" is four random lower-case letters. You can change this to output a specific filename in the Image Folder selected.

Include Hexagon lines: Defaults to draw lines. This draws multiple 2-inch wide hexagons across the map segment, to assist with scale and in-game movement.

Include Hexagon dots: Defaults to draw dots. This draws multiple sets of black dots in hexagon patterns in the same pattern and scale as the Hexagon lines.

X and Y size of the grid: defaults to 3x3, but can be up to 7x7

The primary option window will automatically proceed to the grid randomization stage with a secondary GUI after 30 seconds.

Secondary GUI:

The program generates a grid as described in the grid size at the bottom of the first GUI.
The program randomly populates the grid with either "F" or "W" in each space, representing "Floor" or "Wall", respectively.
In this secondary GUI, you have 30 seconds to make any changes desired to the floor/wall layout of this dungeon grid.
After 30 seconds, or when the "OK" button is clicked, the program will proceed to generate a random dungeon segment image with the given specifications.
