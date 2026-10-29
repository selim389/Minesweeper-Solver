# Minesweeper-Solver
Minesweeper is a classic logic puzzle game that made its debut on Windows computers in 1990, and eventually became built into older computers in 1992. The game is played on a $m \times n$ grid of tiles. A number of mines are randomly set within the tiles. The objective of the game is to clear the board (or minefield) without detonating any mines. Tiles throughout the board are marked with numbers ranging from 1 to 8, telling you the number of mines that are adjacent to the tile. The game is complete once every mine has been determined, and all of the non-mine tiles have been uncovered (this results in a win), or if a mine is uncovered by the player (this results in a loss).

Utilizing various computer vision techniques, this project uses image preprocessing methods such as grayscale conversion and Canny edge detection, as well as grid scan and template matching to extract data from the Minesweeper board (numbers, flags, unmarked tiles). With this extracted data, Minesweeper logic will be applied in-order to determine the location of any known mines. Given that Minesweeper is considered to be an NP-Complete problem, we are unable to fully solve the board from a single image input.

# Breakdown
This section with show the input, as well as the output at every stage within this project. 

## Input
Here is an example input image of a $16 \times 16$ Minesweeper board, with a total of 40 mines.

![Example Input Image](https://raw.githubusercontent.com/selim389/Minesweeper-Solver/refs/heads/main/Test%20Image%206.png)

## Image Preprocessing
Here is the output given during the Image Preprocessing stage.

![Example Canny Edge Detection Output Image](https://raw.githubusercontent.com/selim389/Minesweeper-Solver/refs/heads/main/cannyedge.png)

## Data Extraction


## Logic Application & Output
Here is the final output, giving the solved $16 \times 16$ 2d array.

![Example Logic Application Output Image](https://raw.githubusercontent.com/selim389/Minesweeper-Solver/refs/heads/main/Logic%20Application%20Output.png)
