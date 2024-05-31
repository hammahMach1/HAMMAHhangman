Hammah's Hangman Game

Introduction

This is a simple console-based implementation of the classic Hangman game written in Python. The player guesses letters to try to reveal a hidden word within a limited number of tries.

Features

Random word selection from a predefined list.
ASCII art to represent the hangman at different stages.
Tracks guessed letters and words.
Allows for repeated play until the user chooses to exit.
Getting Started

Prerequisites
Python 3.x installed on your system.
Running the Game
Clone the repository or download the hangman.py file.
Open a terminal or command prompt.
Navigate to the directory containing hangman.py.
Run the game using the following command:
sh
Copy code 
python hangman.py

python hangman.py
How to Play
The game will randomly select a word from a predefined list.
You will be prompted to guess a letter or the entire word.
If you guess a correct letter, it will be revealed in the word.
If you guess an incorrect letter, you lose a try, and part of the hangman figure will be drawn.
You have a total of 6 tries to guess the word correctly.
If you guess the word before running out of tries, you win. Otherwise, you lose, and the word is revealed.
Code Overview

get_word()
Selects and returns a random word from a predefined list of words.
display_hangman(tries)
Returns a string representing the current state of the hangman based on the number of tries left.
play(word)
The main game logic. Handles user input, checks guesses, updates the display, and manages the game state.
main()
Initializes the game by selecting a word and calling the play() function. Also handles replaying the game based on user input.
Example

sh
Copy code
Let's play Hangman!

   --------
   |      |
   |      
   |    
   |      
   |     
   -

_ _ _ _ _ _ _

Please guess a letter or word: p
Good job, p is in the word!

   --------
   |      |
   |      
   |    
   |      
   |     
   -

p _ _ _ _ _ _

Please guess a letter or word: z
z is not in the word.

   --------
   |      |
   |      O
   |    
   |      
   |     
   -

p _ _ _ _ _ _

...

Let's play Hangman!

   --------
   |      |
   |      
   |    
   |      
   |     
   -

_ _ _ _ _ _ _

Please guess a letter or word: p
Good job, p is in the word!

   --------
   |      |
   |      
   |    
   |      
   |     
   -

p _ _ _ _ _ _

Please guess a letter or word: z
z is not in the word.

   --------
   |      |
   |      O
   |    
   |      
   |     
   -

p _ _ _ _ _ _

...
Contributing

Contributions are welcome! If you have suggestions for improvements or new features, feel free to open an issue or submit a pull request.

License

This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgements

ASCII art for the hangman was inspired by various online examples.
Enjoy playing Hangman!
