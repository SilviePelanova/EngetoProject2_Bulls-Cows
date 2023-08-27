# **Bulls & cows**

## About
Bulls&cows is a game based on guessing a secret number. The program will generate the secret number and the player guesses it. Then the program counts the number of matches. The aim of the game is to guess all the matching digits in the least number of attempts. 

## Used modules
The program uses module random to generate random number and module time and datetime to count elapse time in format hh:mm:ss.

## How the program works
The program will generate an unknown random number in the format:
 + 4-digit number
 + do not start with 0 
 + digits occur just once 
 
 Then the program prompts the player to insert a number. Once the number is entered the program launch the time counter, evaluate the format of the number and count the number of matching digits, bulls&cows. If wrong number format used, program returns message with invalid input and prompt player to enter new number. Once the correct number is entered, the program launches loop counter.
 If the matching digit is in the right position the program will count bull/bulls. If the matching digit is in a different position the program will count cow/cows. The bull/bulls are counted first. Then the program will prompt the player to insert new guess until the player guesses the number. When the game ends the program will return a message with number of guesses, status how well the player played the game based on the number of guesses and elapsed time in a format hh:mm:ss. The loops are counted only for a valid input until the end of the game. Time counter ends when the player guessed the secret number.

_Example with secret number => 1369_
![The course of the game, counting bulls and cows](https://github.com/SilviePelanova/sp-repo/blob/main/Engeto_Project_2/image-bulls%26cows.png)

## How to play

### Launch the game
The game can be launched on any tool allowing run py. script.

### Rules
The inserted number must be in the given format:
+ 4-digit number (e.g., e345 contains letter e => invalid input)
+ do not start with 0 (e.g., 0123 starts with 0 => invalid input)
+ digits must not be repeated (e.g., number 2342 contains digit 2 on the first and last position => invalid input) Only the number in the right format is evaluated to count bulls and cows.

Once the program prompts you to insert a number, insert the number by writing it. In case you receive a message with an invalid input, enter a number in valid format. In case of valid input program will return message with number of matching digits, bulls&cows. 
+ Bull/bulls => you guessed matching digits on right position
+ Cow/cows => you guessed matching digits not on the right position. 

Then the program will prompt you to enter another guess. If you reach 4 bulls (all digits are matching on the right position), you guessed the secret number and the game ends.

