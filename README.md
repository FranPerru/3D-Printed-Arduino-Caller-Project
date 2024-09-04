# 3D-Printed-Arduino-Caller-Project
*An Arduino-based caller with 3D printed parts and LED digits.*

*Project Overview*
This project involves creating a call panel for a system with 10 positions (spots), each represented by a button. The goal is to display the number of the position on a visual output when its corresponding button is pressed. The project utilizes two Arduino boards to manage the hardware components efficiently. One Arduino handles the button inputs, while the other controls a series of 14 LEDs arranged to display numbers from 00 to 99.

*Hardware Components*
2x Arduino Uno (or compatible boards)
10x Push Buttons for position inputs
14x LEDs to display position numbers
14x 220Ω Resistors for current limiting on LEDs
Jump wires and breadboards for prototyping
LCD Display (Optional) if an alternative display method is preferred
3D Printed Frame for housing the LEDs and buttons, with black PLA for the frame and transparent PLA for the LED holders

*Functionality*
Button Input: Each of the 10 buttons is associated with a specific position. When a button is pressed, it sends a signal to the Arduino controlling the LEDs.
LED Display: The second Arduino receives the signal and illuminates the corresponding LEDs to display the position number on the panel.
Communication: The two Arduinos communicate via serial communication, ensuring that button presses on the first Arduino result in the correct display on the second Arduino.

*Software*
The project includes Arduino sketches for both boards:

Arduino 1: Manages button inputs, reads which button is pressed, and sends this information to Arduino 2 via serial communication.
Arduino 2: Receives the button press information and activates the corresponding LEDs to display the position number.
Additional Features
Modular Design: The project is designed to be easily expandable. Additional positions can be added by scaling the number of buttons and corresponding LEDs.
Custom 3D-Printed Enclosure: The 3D-printed frame is designed to securely house the LEDs and buttons, providing a professional and organized look.
Optional LCD Display: The project can be modified to use an LCD display instead of LEDs, depending on the desired output method.
Usage
Initial Setup: Connect the buttons and LEDs to their respective Arduinos as described in the circuit diagrams provided.
Upload Code: Upload the corresponding Arduino sketches to each board.
Testing: After setting up the hardware and uploading the code, pressing any button should result in the display of the corresponding position number on the LED array.
Future Enhancements
Wireless Communication: Implementing wireless communication between the two Arduinos could make the system more flexible.
Advanced Display Options: Integrating more advanced displays, such as a dot-matrix LED display or a TFT screen, for more sophisticated number presentation.
Integration with Other Systems: Expand the system to interface with a computer or mobile app for remote control and monitoring.
