Naqvi Roll the Dice

A simple dice rolling game built with Python's Tkinter and Pillow libraries.

Key Features:

Graphical User Interface (GUI): Utilizes Tkinter for user-friendly interaction with the application.
Random Dice Rolls: Simulates dice rolls using random numbers and displays the corresponding image.
Customizable Appearance: Allows changing the label's font, color, and formatting for visual appeal.
Clear and Simple Code: Maintains readability and understanding through proper indentation and commenting.
Installation:

Python: Ensure you have Python installed on your system. You can download it from https://www.python.org/downloads/.
Pillow (PIL Fork): Install the Pillow library using pip: pip install Pillow
Running the Application:

Save the code: Save the code as a Python file (e.g., dice_game.py).
Execute the script: Open a terminal or command prompt, navigate to the directory where you saved the file, and run the following command: python dice_game.py
Explanation:

Imports: The code begins by importing necessary libraries, including tkinter for the GUI, Image and ImageTk from Pillow for image handling, and the random module.
Main Window: A tkinter.Tk() instance creates the main window and sets its title to "Naqvi Roll the Dice" using root.title(). The window size is adjusted with root.geometry().
Labels: Two labels are created using tkinter.Label():
l0: Displays the text "AliHassan's" with default settings using l0.pack().
l1: Customized with bolder, italicized Helvetica font (size 16), light green foreground, and dark green background using l1.pack().
Images: A list of image filenames for the dice faces (die1.png to die6.png) is stored in dice. The rolling_dice() function uses random.choice(dice) to pick a random file, opens it with Image.open(), and creates a PhotoImage object using ImageTk.PhotoImage() for display.
Dice Rolling Function:
rolling_dice(): This function is called when the "Roll the Dice" button is clicked. It:
Generates a random image from the dice list.
Updates the label1 image using label1.configure(image=image1).
Maintains a reference to the image using label1.image = image1.
Button: A button with the text "Roll the Dice" and blue foreground color is created using tkinter.Button(). It's linked to the rolling_dice() function using the command option and then displayed with button.pack().
Main Loop: The root.mainloop() call ensures that the window stays open and responds to user interactions.
Customization:

You can modify the label text, font, color, and other attributes as desired using the options provided by tkinter.Label().
You can replace the existing dice images with your own by ensuring they have the same file names and are placed in the same directory as this script.
Feel free to explore the documentation of Tkinter and Pillow for further customization possibilities.
