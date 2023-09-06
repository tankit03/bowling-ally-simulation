# Bowling Alley Simulation Program

## Overview

Welcome to the Bowling Alley Simulation Program! This software is designed to simulate a game of bowling for a single player. Before we dive into the program's usage, let's understand the rules and implementation requirements:

## Bowling Rules

- This program supports a single player.
- The game begins by prompting the player for their name and greeting them.
- There are 10 total frames in a game.
- Each frame allows the player up to 2 rolls (chances) to knock down a total of 10 pins.
- The player can knock down 0-10 pins with their first roll.
- With the second roll, the player can knock down 0 pins up to the number of pins remaining from the first roll.
- If the player knocks down all 10 pins in their first roll of a frame, it's a **strike (X)**, and they don't get a second roll in that frame.
- If the player knocks down all 10 pins in a frame using two rolls, it's a **spare (/)**.
- If the player knocks down 0 pins in a frame, it's called a **gutter (-) ball**.
- If a strike or spare occurs in the 10th frame, the player gets a **3rd roll** in that frame.

## Scoring Rules

- Frame score calculation:
  - An open frame (no strike or spare) score is the total pins knocked down with two rolls in the current frame.
  - A frame score with a strike is 10 plus the number of pins knocked down with the next two rolls. This can give a player 10-30 points for a frame with a strike.
  - A frame score with a spare is 10 plus the number of pins knocked down with the next roll. This can give a player 10-20 points for a frame with a spare.
  - Three consecutive strikes in frame 10 give 30 points.
- The player's **total score** is the sum of all 10 frame scores.

## Implementation Requirements

- The number of pins knocked down in each roll is determined by a random number:
  - First roll: 0 to 10
  - Second roll: 0 to (10 - first roll)
- An array represents pins knocked down with each roll for each frame, and this information is displayed after each roll.
- The program keeps track of the player's **total score** and displays it after each roll/frame.
- After each roll, the program prints the **game scoresheet**, including frame information and the total score for the player.
  - The frame information consists of the number of pins knocked down with each roll in each frame and the sum of the current and prior frame scores for each frame.
  - Strikes are denoted with an **X**.
  - Gutter balls are denoted with a **dash (-)**.
  - Spares are denoted with a **forward slash (/)**.
- After each frame, the program prints the **total frame scores** and a **total score**, if calculable.
- The game concludes by printing the **total score of the player** at the end of a game.
- The game allows for playing again with a different player at the end of a game, until the user decides to quit.
- The program handles all errors, such as incorrect inputs for bowling.

## Good Software Engineering Principles

- **Design your solution** before writing the program.
- Develop **test cases** before writing the program.
- Review conditionals, loops, functions, and arrays.
- Practice dynamic memory usage with pointers.
- Use functions to modularize code for increased readability and reduced repeated code.

## Enjoy the Bowling Game!

Now that you understand how the Bowling Alley Simulation Program works, have fun rolling those virtual balls and scoring strikes and spares. Enjoy your bowling experience!
