# rockpaperscissors
My code for the Arduino powering an interactive rock, paper, scissor robotic hand. 

There were two circuits connected wirelessly. The first was the robotic-hand circuit, made using motors attached to the Arduino board, string, and straws (and a lot of tape!) The second circuit comprised of 2 sensors attached to the forefinger and thumb of a glove to receive input about the move made from the movement the user wearing the glove. I programmed the speaker to emit 5 beeps when the button connected to the Arduino board is pressed by the user. 

After the beeps, both the robotic hand and the user makes a move, just like the actual rock-paper-scissor game with a human. 

The function getRobotChoice() in the code picks an integer from 1-1000, <333 corresponding to rock, >=333 & <666 corresponding to paper, and >=666 corresponding to scissors.

The function getUserChoice() then takes an input from the bend sensors. (1,1) corresponding to rock, (0,1) corresponding to scissors, and (0,0) corresponding to paper. 

Then the function compareChoice() compares the input by the user and the robot's movement generated by the Arduino to determine who won. 

