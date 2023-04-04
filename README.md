# CodeClause_color_detection
This code is an implementation of a color detection algorithm in Python using the OpenCV library.
It allows the user to click on any pixel in an image and then displays the name of the color of that pixel,as well as the RGB values of that pixel.
The program reads an image from a file, sets up a mouse callback function to detect double-click events, and creates a window to display the image. 
It also reads a CSV file containing color information, such as color name, hex code, and RGB values.
The get_color_name() function calculates the minimum distance between the RGB values of the selected pixel and the colors listed in the CSV file to determine the most similar color.
The draw_function() function is called when the user double-clicks on a pixel, and it sets the clicked flag to true, records the pixel's RGB values, and ends the function.
The main loop of the program runs continuously until the user hits the 'esc' key. 
If the user has clicked on a pixel, the program updates the rectangle and text displays to show the selected color's name and RGB values. 
If the sum of RGB values is greater than or equal to 600, the text will be displayed in black color. 
Finally, the program waits for the user to hit the 'esc' key before closing the window and terminating the program.
