<img width="1280" alt="readme-banner" src="https://github.com/user-attachments/assets/35332e92-44cb-425b-9dff-27bcf1023c6c">

# [Finger wars] 🎯


## Basic Details
### Team Name: [STRIKE]


### Team Members
- Team Lead: [Adarsh A] - [NSS COLLEGE OF ENGINEERING]
- Member 2: [Amruthavarshan P H] - [NSS COLLEGE OF ENGINEERING]
- Member 3: [Arunkrishna P U] - [NSS COLLEGE OF ENGINEERING]

### Project Description
[This project is a two-player "Finger Wars" game using an Arduino, where players compete by wiggling the fingers to move an LED towards opposite side. The first player to push the LED to their opposite end wins, with game status displayed on an LCD.]

### The Problem (that doesn't exist)
[This project humorously solves the "problem" of deciding who's faster by creating a fun finger flicking game with an LED race, perfect for friendly competition.]

### The Solution (that nobody asked for)
[A thrilling LED race game that lets two players mash buttons to claim victory, turning quick reflexes into ultimate bragging rights—because who really needed another way to settle friendly rivalries?]

## Technical Details
### Technologies/Components Used
For Software:
- [Languages used:C/C++ (Arduino IDE)]
- [Frameworks used: Arduino Framework]
- [Libraries used: LiquidCrystal_I2C for the LCD display]
- [Tools used: Arduino IDE for code development and debugging]

For Hardware:
- [Arduino uno, LEDs, IR sensor, Buzzer,  connecting wire]
- [Microcontroller:
   Arduino Uno: 5V, 16 MHz, 14 digital I/O pins
  
- IR Sensors:
  - Quantity: 2
  - Voltage: 3.3V-5V
  - Range: 2-30 cm
  - Output: Digital (HIGH/LOW)
    
- LEDs:
  - Quantity: 7
  - Voltage: 2-3V
  - Current: ~20mA per LED
    
- Buzzer:
  - Voltage: 5V
  - Programmable tone frequencies
    
- LCD Display:
  - 16x2 I2C module
  - Address: Typically 0x27 or 0x3F
    
- Power Supply:
  - USB or 9V battery
    
- Connections:
  - LEDs: Pins 4-10
  - IR Sensors: Pins 2, 3
  - Buzzer: Pin 11
    
- LCD:
   VCC - 5V, GND - GND, SDA - A4, SCL - A5

Game Mechanics:

Players press their buttons to move a central LED left or right along a row.
Player 1 moves the LED right, and Player 2 moves it left.
The goal is to push the LED to the opponent’s end to win. 
When the LED reaches the far right, Player 1 wins; if it reaches the far left, Player 2 wins. 
The game then displays a winning message and plays a victory sound.

### Implementation
For Software:
# Installation
[commands]

# Run
[commands]

### Project Documentation
For Software:

# Screenshots (Add at least 3)
![Screenshot1](Add screenshot 1 here w![e111f725-28f1-417e-bdeb-39c91b8d421a](https://github.com/user-attachments/assets/bf724560-ddf0-4c65-849f-7715a58585a7)
ith proper name)
*Add caption explaining what this shows*

![Screenshot2](Add screenshot 2 here with ![bc19bba0-8225-4b9b-bc0c-6cc14c6371b9](https://github.com/user-attachments/assets/7235b86a-50b3-4e0e-a096-b6c16f0bb47c)
proper name)
*Add caption explaining what this shows*

![Screenshot3](Add screenshot 3 here with proper name![26d287c1-6fd7-46fb-83e9-c5f6d01cacd0](https://github.com/user-attachments/assets/ae793ae5-6368-4fbd-9306-3918a38326a1))
*Add caption explaining what this shows*


# Diagrams

![Workflow](![09f88809-3e1c-4507-8d43-8879a3c3b0ef](https://github.com/user-attachments/assets/60b25892-a073-4481-ada4-ba8d712e469c))
*Add caption explaining your workflow*

For Hardware:

# Schematic & Circuit
![Circuit](![Screenshot 2024-11-02 222235](https://github.com/user-attachments/assets/fcd238f1-876e-4dd4-8f68-e4806466d02e)
r-attachments/assets/a071a0cd-b80c-4c2c-aad2-c7bebe6abaf9))
*Connect the LCD (I2C 16x2) by wiring SDA to A4 and SCL to A5 on the Arduino Uno, and power it by connecting VCC to 5V and GND to GND.
For the IR sensors, connect IR Sensor 1 (Player 1) to Digital Pin 2 and IR Sensor 2 (Player 2) to Digital Pin 3.
To set up the LEDs as position indicators, connect each one to Digital Pins 4 through 10 in order.
Finally, connect the buzzer by wiring the positive terminal to Digital Pin 11 and the negative terminal to GND.*

![Schematic](![Neat Inari-Wolt (1)](https://github.com/user-attachments/assets/a071a0cd-b80c-4c2c-aad2-c7bebe6abaf9))
*AFinger Wars is an engaging two-player game that utilizes an Arduino microcontroller along with various electronic components to create a competitive experience. At the heart of the game is an I2C LCD that displays vital information, including game messages and the current position of the LED. A row of LEDs, connected to digital output pins, forms the game field, while two IR sensors play a crucial role in player interaction. IR sensors detect the players' hand movements without direct contact, allowing for a more dynamic and hygienic gameplay experience. As players wave their hands over the sensors, the LED shifts toward their opponent's end of the row. The game begins with the LED centered, and players compete to move it to the edges, striving for victory. When the LED reaches either end, the game announces the winner on the LCD and plays a celebratory sound through the buzzer. This innovative use of IR sensors enhances the responsiveness and engagement of the game, providing a modern twist to the classic concept of competition.*

# Build Photos
![Components](Add photo of your components here)
*Arduino board, I2C LCD, 8 LEDs, 2 IR sensors, buzzer, resistors, breadboard, jumper wires.
*

![Build](Add photos of build ![67183cf4-bac6-4937-971d-faabf5f112dc](https://github.com/user-attachments/assets/c9775056-a2b8-4897-95a0-2415e6f9410b)
process here)
*LCD Connection: Connect SDA to A4 and SCL to A5 on the Arduino. Connect VCC to 5V and GND to GND. Confirm the I2C address in the code (commonly 0x27).
IR Sensors: Connect IR Sensor 1’s signal pin to Digital Pin 2 (Player 1) and IR Sensor 2’s signal pin to Digital Pin 3 (Player 2). Power each sensor by connecting VCC to 5V and GND to GND.
LEDs: Connect Digital Pins 4–10 to each LED (left to right) with the negative pin of each LED connected to GND through a 220Ω resistor.
Buzzer: Connect positive to Digital Pin 11 and negative to GND.
Upload Code: Paste and upload the code in Arduino IDE, setting the correct board and port.
run the Game: When powered on, the LCD displays the game title, and a start tune plays. Use the IR sensors to move the LED left or right. Reaching the ends triggers a win message and sound for the respective player.*

![Final](Add photo of final product here![bc19bba0-8225-4b9b-bc0c-6cc14c6371b9](https://github.com/user-attachments/assets/e30015f9-a80f-4a05-bb10-38aba111c7c3))
* 1. Game Initialization
Power-Up Sequence: When the game is powered on, the Arduino microcontroller initializes all components. It sets the LCD to display a welcoming message, such as “Welcome to Finger Wars!”, establishing the game's theme.
Sound Effect: To enhance the initial experience, a retro start tune is played through the buzzer, adding an audio cue that signals the game is ready to begin.
2. Game Start
Initial Setup: The LED array starts with the LED positioned at the center. This central starting point visually indicates that the game is balanced, with both players having equal opportunities to win.
Player Readiness: Players are prompted to get ready, and the game awaits their hand movements over the IR sensors to initiate the gameplay.
3. Player Interaction
IR Sensor Activation: Each IR sensor is positioned to detect hand movements:
Player 1's Control: When Player 1 waves their hand over their designated IR sensor, the sensor detects the movement, signaling the Arduino to execute a command to move the LED one position to the right.
Player 2's Control: Similarly, Player 2 can wave their hand over their IR sensor, prompting the LED to move one position to the left.
Real-Time Feedback: After each movement, the current position of the LED is updated and displayed on the LCD, allowing players to see their progress and strategize their next move.
4. Winning Condition
Position Check: The Arduino continuously monitors the position of the LED. It compares the LED’s position against predetermined thresholds:
If the LED moves to the far-right end of the array, the Arduino registers that Player 1 has won.
If the LED reaches the far-left end, Player 2 is declared the winner.
Victory Announcement: Upon determining a winner, the game updates the LCD to announce “Player 1 Wins!” or “Player 2 Wins!” Additionally, the buzzer plays a celebratory sound effect, enhancing the excitement of winning.
5. End of Game
Game Termination: Once a player wins, the game ceases to respond to further inputs from the IR sensors, effectively ending that round of competition.
Restart Option: Players can reset the game by powering it off and then on again or implement a button for resetting within the code, allowing for multiple rounds of play without needing to reconfigure the setup.
6. User Experience
Engaging Gameplay: The game’s design focuses on creating an immersive experience. Players actively engage with the game through physical movement, promoting interaction and competition.
Visual and Auditory Feedback: The combination of LED indicators, real-time updates on the LCD, and sound effects from the buzzer ensures players receive immediate feedback on their actions, enhancing their sense of involvement and enjoyment.
Hygienic Interaction: The use of IR sensors allows for touchless gameplay, making the game more appealing in social settings, particularly in light of hygiene concerns.
The final build of Finger Wars effectively integrates various electronic components to create a fun and interactive game. Its innovative use of IR sensors for player interaction, combined with visual and auditory feedback, provides a modern twist to classic competitive games. The game not only serves as a source of entertainment but also demonstrates the principles of electronics and programming, making it an engaging project for both creators and players alike*
### Project Demo
# Video
[[Add your demo video link here](https://youtu.be/y0UUmDJTGRA?si=vT_ZeLQmOUt4Zwol)]
*The video shows which components we used and how the final output turned out*
# Additional Demos
[Add any extra demo materials/links]

## Team Contributions
- [Amruthavarshan P H]: [ideator,schrematic,video editing,Coding]
- [Adarsh A]: [circuit,coding,debugging,team leader,work flow diagram]
- [Arunkrishna P U]: [coding,connections,components,wrtings,planning ]
---
Made with ❤️ at TinkerHub Useless Projects 

![Static Badge](https://img.shields.io/badge/TinkerHub-24?color=%23000000&link=https%3A%2F%2Fwww.tinkerhub.org%2F)
![Static Badge](https://img.shields.io/badge/UselessProject--24-24?link=https%3A%2F%2Fwww.tinkerhub.org%2Fevents%2FQ2Q1TQKX6Q%2FUseless%2520Projects)



