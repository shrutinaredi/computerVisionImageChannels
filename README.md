Overview:
---------
This homework consists of two programming walkthroughs that introduce basic Python image processing concepts.

Walkthrough 1: Vincent van Gogh Collage
----------------------------------------
- Creates a 2x2 collage showing the original Van Gogh image and its red, green, and blue color channels
- Output file: collage.png

Implementation details:
- Used numpy array indexing to extract individual color channels
- Created blank images with np.zeros_like() and filled individual channels
- Used np.concatenate() to combine images horizontally and vertically

Walkthrough 2: I ❤️ NY Logo Overlay
------------------------------------
- Superimposes a red "I ❤️ NY" logo onto a Manhattan scene
- Output file: output_nyc.png

Implementation details:
- Converted the logo to grayscale using color.rgb2gray()
- Created binary mask using threshold value of 0.5
- Used np.pad() to match image dimensions
- Applied red color [255, 0, 0] to masked regions

Parameters/Constants:
--------------------
Walkthrough 2:
- threshold = 0.5 (for converting grayscale to binary mask)
  This value was chosen as a reasonable midpoint that effectively separates
  the logo foreground from its background.

Packages Used:
--------------
- numpy: Array operations and mathematical functions
- matplotlib.pyplot: Image display and visualization
- skimage.io: Image loading (io.imread) and saving (io.imsave)
- skimage.color: Color space conversion (rgb2gray)
- skimage.transform: Image resizing (rescale)

All packages used are within the allowed guidelines for this assignment.

Files Included:
---------------
1. hw1_walkthrough1.py - Completed code for Walkthrough 1
2. hw1_walkthrough2.py - Completed code for Walkthrough 2
3. signAcademicPolicy.py - Academic honesty policy (with student info)
4. runHw1.py - Main test framework
5. collage.png - Output from Walkthrough 1
6. output_nyc.png - Output from Walkthrough 2
7. Vincent_van_Gogh.png - Input image for Walkthrough 1
8. I_Love_New_York.png - Input logo for Walkthrough 2
9. nyc.png - Input background for Walkthrough 2
10. README.txt - This file
