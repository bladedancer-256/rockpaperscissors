# rockpaperscissors
My code for the Arduino powering an interactive rock, paper, scissor robotic hand. 

There were two circuits connected wirelessly. The first was the robotic-hand circuit, made using motors attached to the Arduino board, string, and straws (and a lot of tape!) The second circuit comprised of 2 sensors attached to the forefinger and thumb of a glove to receive input about the move made from the movement the user wearing the glove. I programmed the speaker to emit 3 beeps when the button connected to the Arduino board is pressed by the user. After the beeps, both the robotic hand and the user makes a move, just like the actual rock-paper-scissor game with a human. The function robot() in the code picks an integer from 0-2, 0 corresponding to rock, 1 corresponding to paper, and 2 corresponding to scissors. The function user() then takes an input from the glove. (1,1) corresponding to rock, (0,1) corresponding to scissors, and (0,0) corresponding to paper. Then the function compare() compares (as per the name) the input by the user and the robot's movement generated by the Arduino to determine who won. The function playMusic() then plays one of three different tunes depending on the outcome relative to the user: win, lose, or tie.

