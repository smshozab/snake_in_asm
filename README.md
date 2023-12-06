<h1>Assembly Language Snake Game</h1>
**About the project**
This program is a personal project when I was learning 'computer organization and architecture' in the second year of my Management Mathematics and Computing bachelors degree. The idea behind of this program was the classic "Snake" game. This program was made using Microsoft Visual Studio 2017's 32bit MASM architecture in protected mode (no interrupts) and the Irvine32 library.

<h2>Features and Functions</h2>
**Game Speed Selection**
User may choose from three speed levels, level 1 to level 3, level 3 being the slowest.
Each of the speed levels have a 40ms difference.

**Random Generation of coin**
A coin is generated randomly at the start of every game or when the snake eats the previous coin.
A checking function is also created to make sure that the random coin doesnt generate on the coordinates of the snake.
A new coin is regenerated if the current one is generated at an invalid coordinate.

**Accepting keyboard input**
After the coin is generated, a loop will be initiated to detect for input and jump to specific functions according to the input.
If no key is entered, the program will keep looping and waiting for an input.
If the snake is moving and a valid input is not entered, the function will continuously loop and snake will continuous to move at the current direction.
If the user enters a new input that moves the snake in a different direction, the program will jump to a function that changes the function of the snake.

**Move Snake**
The head of the snake will be moved according to the user's last known input.
The body of the snake will be moved to the coordinate of the unit before it (eg: the 3rd unit of the body will move to the coordinates of the 2nd unit of the body)

**Coin Detection**
When the Snake moves, the coordinate of the head is compared with the coordinate of the coin to check whether the snake eats a coin

**Bonus Coin**
A bonus coin is created after every three coins eaten by snake, which increases the score by three.

**Eat Coin**
When a coin is eaten, a new unit is added to the snake to lengthen the snake.
The new tail is at the position of the old tail, a new tail is added according to the direction of the old tail

**Self Collision Detection**
When the Snake moves, the coordinate of the head is compared with the coordinate of the coin to check whether the snake collides with itself
Snake dies when it collides with itself
A function loops through the coordinates of the body of the snake and compares with the head position to check if they collide.
Wall Collision Detection
When the Snake moves, the coordinate of the head is compared with the coordinate of the coin to check whether the snake collides with the wall
Snake dies when it collides with the wall
A function compares the coordinates of the wall and the head to check if they collide

**Scoreboard**
When the game is over, a scoreboard is displayed to show the current score and high score of the user.
The user can also choose to exit the game or restart the game.

**Input Validation**
Input Validation is set to detect any invalid input and prompts the user to reenter the input if so.
Flowchart
Flowchart of this program can be downloaded here: snake game flowchart.pdf

**Controls**
Keys	Actions
w	Move up
a	Move left
s	Move down
d	Move right
x	Quits the game at any time
enter	Pause, (w,a,s,d to unpause)
(make sure that your capslock is disabled)

<h2>Output Screens</h2>
<img width="671" alt="image" src="https://github.com/smshozab/snake_in_asm/assets/29998010/6610c6f2-5aba-4ab4-a776-1e197010d87c">
<img width="674" alt="image" src="https://github.com/smshozab/snake_in_asm/assets/29998010/54e988d8-421d-437a-9863-0967d5c6a6f8">
<img width="675" alt="image" src="https://github.com/smshozab/snake_in_asm/assets/29998010/7e79238e-8061-4514-a028-5f306f10d724">
<img width="673" alt="image" src="https://github.com/smshozab/snake_in_asm/assets/29998010/c0dd5402-632a-4c08-8c9e-6fe58c0120a7">
