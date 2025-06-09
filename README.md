Light Scrolling Program
Overview
The Light Scrolling Program is a Python-based simulation where you control the state of a series of lights and input triggers. The program includes functionalities to turn on lights sequentially, turn all lights on or off simultaneously, and perform a reverse light scroll. This project is intended for educational purposes and can be used for understanding basic object-oriented programming (OOP) concepts, as well as time-based operations in Python.

Features
Light Class: Represents a single light with an on/off state.

Input Class: Simulates user inputs, each of which can trigger different actions.

Light Scrolling: Turns lights on sequentially with a 1-second delay between each light.

All Lights On/Off: Turns all lights on or off at the same time.

Reverse Light Scrolling: Turns on lights in reverse order, one by one, with a 1-second delay between each.

Input-Driven Actions: Allows the user to trigger different light sequences using input commands (I1, I2, I3) and can stop the program with the "Exit" command.

Setup
To use this program, ensure you have Python installed on your machine (Python 3.x is recommended).

Installation
Clone the repository (or download the script directly):

bash
Copy
git clone https://github.com/yourusername/light-scrolling-program.git
Navigate to the directory where the script is located.

Run the script:

bash
Copy
python light_scrolling_program.py
Or, if you're using an IDE, open the script and run it.

Dependencies
This project uses the built-in Python time module to control delays between light actions. No additional dependencies are required.

Usage
Once the program is started, the user will be prompted to choose between three inputs, which trigger different light actions:

Input 1 (I1): This triggers the Light Scroll action, where lights turn on one by one in sequence with a 1-second delay between each.

Input 2 (I2): This triggers the All Lights On action, where all lights are turned on simultaneously.

Input 3 (I3): This triggers the Light Scroll Reverse action, where lights turn on in reverse order with a 1-second delay between each.

The user can also type "Exit" to stop the program.

Code Explanation
1. Light Class
This class represents a single light. It has the following attributes and methods:

name: The name of the light (e.g., "L_1", "L_2").

is_on: Boolean attribute to track whether the light is on or off (default is False).

turn_on(): Turns the light on and prints a message.

turn_off(): Turns the light off and prints a message.

2. Input Class
This class simulates user inputs (I1, I2, I3). Each input can trigger specific actions:

name: The name of the input (e.g., "I1", "I2").

is_on: Boolean attribute to track whether the input is on or off.

turn_on(): Activates the input and prints a message.

turn_off(): Deactivates the input and prints a message.

3. Light Actions
Light_Scroll(): Turns on each light sequentially with a 1-second delay between each.

All_Lights_On(): Turns all the lights on at once.

All_Lights_Off(): Turns all the lights off at once.

Light_Scroll_Reverse(): Turns on each light sequentially in reverse order with a 1-second delay.

4. Program Flow
The program continuously prompts the user for input. Based on the input, one of the corresponding light actions is triggered. The program runs in an infinite loop, awaiting further user input, until the user types "Exit".

Contributing
Feel free to fork this project, make improvements, and create a pull request. Contributions are welcome to add new features, improve existing functionalities, or optimize the code.

Some Ideas for Improvement:
Add logging or visual representation of light states.

Add more input options for different light patterns or user controls.

Implement a GUI to control the lights visually.
