# Number Gussing Game 
## Thinking like a programmer

One of the hardest things to learn in programming is not the syntax you need to learn, but how to apply it to solve real-world problems. You need to start thinking like a programmer — this generally involves looking at descriptions of what your program needs to do, working out what code features are needed to achieve those things, and how to make them work together.

### Q: Let's imagine your boss has given you the following brief for creating this game:

I want you to create a simple "guess the number" type game. It should choose a random number between 1 and 100, then challenge the player to guess the number in 10 turns. After each turn, the player should be told if they are right or wrong, and if they are wrong, whether the guess was too low or too high. It should also tell the player what numbers they previously guessed. The game will end once the player guesses correctly, or once they run out of turns. When the game ends, the player should be given an option to start playing again.

### Upon looking at this brief, the first thing we can do is to start breaking it down into simple actionable tasks, in as much of a programmer mindset as possible:

Generate a random number between 1 and 100.

Record the turn number the player is on. Start it on 1.

Provide the player with a way to guess what the number is.

Once a guess has been submitted first record it somewhere so the user can see their previous guesses.

Next, check whether it is the correct number.

If it is correct:

Display congratulations message.
Stop the player from being able to enter more guesses (this would mess the game up).
Display control allowing the player to restart the game.

If it is wrong and the player has turns left:

Tell the player they are wrong and whether their guess was too high or too low.
Allow them to enter another guess.
Increment the turn number by 1.

If it is wrong and the player has no turns left:

Tell the player it is game over.

Stop the player from being able to enter more guesses (this would mess the game up).
Display control allowing the player to restart the game.

Once the game restarts, make sure the game logic and UI are completely reset, then go back to step 1.


