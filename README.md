﻿# Magic 8-Ball

Welcome to the **Magic 8-Ball** project! This is a simple Swift program that simulates a Magic 8-Ball, providing random answers to a user's question. The program utilizes basic control flow, including the `switch` statement, to randomly select a response from a predefined set of answers.

## Project Overview

This project is a fun implementation of a Magic 8-Ball game, where the user inputs a question and receives a randomized answer. The program generates a random number between 1 and 9, and based on that number, the Magic 8-Ball provides an answer.

## Code Structure

The code is organized into the following key sections:

1. **Player Name and Question:**
   - The `playerName` variable stores the name of the player.
   - The `playerQuestion` variable stores the question asked by the player.

   ```swift
   let playerName = "Ben"
   let playerQuestion = "Will there be any more snowfall in New York for winter 2024? ❄️"

2. **Random Number Generation:**

- The `randomNumber` variable generates a random integer between 1 and 9, which is used to determine the Magic 8-Ball's answer.

   ```swift
   let randomNumber = Int.random(in: 1...9)

3. **Switch Statement for Answer Selection:**
    -  The `switch` statement evaluates the `randomNumber` and assigns a corresponding answer to the `eightBall` variable.

   ```swift
   switch randomNumber {
     case 1: eightBall = "Yes - definitely"
     case 2: eightBall = "It is decidedly so"
     case 3: eightBall = "Without a doubt"
     case 4: eightBall = "Reply hazy, try again"
     case 5: eightBall = "Ask again later"
     case 6: eightBall = "Better not tell you now"
     case 7: eightBall = "My sources say no"
     case 8: eightBall = "Outlook not so good"
     case 9: eightBall = "Very doubtful"
     default: eightBall = "Error"
   }
4. **Output:**
-  The program prints the player's question and the Magic 8-Ball's answer to the console.

   ```swift
   print("\(playerName)'s Question: \(playerQuestion)")
   print("Magic 8 Ball's answer: \(eightBall)")
   
## Challenge

The code includes a challenge to improve the output format when the `playerName` is empty. The solution leverages the ternary conditional operator to adjust the print statement based on whether the `playerName` is provided.

   ```swift
   playerName.isEmpty ? print("Question: \(playerQuestion)") : print("\(playerName) asks: \(playerQuestion)")
```
## Usage

To run the program, simply execute the Swift code in your preferred Swift environment. The program will:
1. Display the player's name and question.
2. Generate a random answer from the Magic 8-Ball.
3. Print the answer to the console.

## Conclusion

This project is a simple and entertaining way to explore the basics of Swift programming, including variables, control flow, and string interpolation. Feel free to modify the code to add more answers, customize the output, or enhance the game's functionality!

Enjoy your journey with the Magic 9-Ball!
