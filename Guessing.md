```mermaid
flowchart TD
Intro([Welcome to the Guessing Game!]) --> NumberGen([Generates a Number 1-10])
NumberGen --> Input([Choose a number between 1-10])
Input-- If input number is above selected number ---A([Too High!])
A --> Input
Input-- If input number is below selected number ---B([Too Low!])
B--> Input
Input--If input number is below 1 or above 10 ---C([Number should be between 1 and 10])
Input-- If input is not a number ---C([Please enter a number between 1 and 10])
C --> Input
Input-- If input number is equal to selected number ---E([You guessed correctly!])
```

Game begins with an introduction and generates a random number between 1 and 10.<br/>
Asks the user for an input.<br/>
If input is not the selected number it will tell whether the guess was too high or too low.<br/>
If the input was beyond the 1-10 range or was not a number it will ask.<br/>
If the input was correctly the selected number, it will tell that you guessed correctly.<br/>
In all results except success it will ask you again for an input to play until you guess the number.<br/>
