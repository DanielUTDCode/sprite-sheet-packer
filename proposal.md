# Sprite Sheet Packer

## Repository
[Public GitHub repository](https://github.com/DanielUTDCode/sprite-sheet-packer)

## Description
I want to make a Python tool that takes a folder of PNG animation frames and packs them into one transparent sprite sheet. This would save me from having to arrange each frame by hand when I make sprites for a game.

## Features
- **Load frames in order**
  - I’ll find the PNG files in a folder and sort them by filename. Names like `frame_01.png` and `frame_02.png` will keep the frames in order.
- **Arrange frames into a grid**
  - I’ll use Pillow to create a transparent canvas and a loop to place each frame. The user can choose the number of columns, and the program will calculate how many rows it needs.
- **Handle different frame sizes**
  - I’ll use the largest frame width and height to set the cell size, then center each frame in its cell without stretching it.
- **Export a usable image**
  - I’ll save the finished sheet as a transparent PNG and print the frame count, grid size, and output filename.

## Challenges
- Figure out how to turn each frame’s index into a row, column, and pixel position.
- Preserve transparency when placing frames onto the sheet.
- Handle empty folders, invalid column counts, and frames that aren’t all the same size.

## Outcomes

**Ideal Outcome:** The tool exports a clean sprite sheet from PNG frames of different sizes, with a user-selected column count. I’d include a sample set of frames and a short README so another student can try it.

**Minimal Viable Outcome:** The tool takes a folder of same-size PNGs and exports them in filename order to a transparent grid with a fixed number of columns.

## Milestones

- Week 1
  1. Set up the repository and make a small set of numbered PNG frames.
  2. Load the frames in order and export a basic grid.

- Week 2
  1. Add configurable columns and center frames of different sizes.
  2. Test transparency, incomplete rows, and invalid inputs.

- Final Week
  1. Fix any remaining issues and export a sample sprite sheet.
  2. Write the README and prepare the demo.
