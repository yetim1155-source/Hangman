#Hackathon Hangman Game

A Terminal-based hangman game written in C. This project was originally built during a fast-paced class mini-hackathon to practice core programming logic, loops, and user input handling. 

#Post Hackathon fixes summary

1. Fixed the word-selection indexing with r-- so choices 1–10 correctly map to array indices 0–9.
2. Fixed the word-length calculation by starting len at 0 instead of 1.
3. Fixed check_guess() so an incorrect guess only counts as one wrong guess instead of adding points for every unmatched letter.
4. Replaced the messy points/looper system with a wrong_guesses counter that correctly allows 3 wrong guesses.
5. Added a separate check_win() function to determine when the entire word has been guessed.
6. Fixed winLose() so it only handles displaying whether the player won or lost.
7. Removed variables from winLose() that were not in its scope (word, len, guessRes).
8. Fixed minor code errors like print() to printf().
9. Fixed the function prototype for check_guess() to match the actual function.
10. Added found in check_guess() to indicate whether the guessed letter exists in the word.
11. Fixed the game loop so it continues until the player wins or reaches 3 incorrect guesses.
12. Added display of the current guess_output before each guess.
13. Fixed replay logic to accept both y and Y.
14. Removed unnecessary header files; only stdio.h was really needed.

#Key Takeaways

- Gained experience tracing and debugging logic post-event
- Learned the constraints of coming up with ideas and then quickly executing it under tight hackathon timeframes.
