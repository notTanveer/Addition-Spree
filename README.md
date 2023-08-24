# Addition Spree

## Overview
This is a simple math game built with React that prompts the user to add two randomly generated numbers. The user types their answer into an input field and presses enter to submit. If they answer correctly, a new set of numbers is generated and their score is incremented. If they answer incorrectly, their score is decremented. The game ends when the user reaches a score of 10.

## Technologies Used
- React - For building the UI and managing state
- Bootstrap - For basic styling
- Babel - To transpile JSX to vanilla JavaScript

## Components
The app consists of a single `App` component that manages the entire game state and logic.

## State
The component's state contains:
- `num1` - The first randomly generated number
- `num2` - The second randomly generated number
- `response` - The user's answer input
- `score` - The user's current score

## Logic
- When a key is pressed in the input field, the `inputKeyPress` handler checks if it is "Enter".
- If so, it parses the input to a number and compares it to the expected answer.
- If correct, new random numbers are generated and score incremented.
- If wrong, the input is cleared and score decremented.
- The `updateResponse` handler updates the `response` state on each change of the input.
- When the score reaches 10, a winning message is displayed.

## Rendering
The component conditionally renders:
- The math problem and input field if the game is still active
- A winning message once the user has won
This allows the game to end once a winning condition is met.

## Assets
The component loads Bootstrap from a CDN for basic styling and Babel for JSX processing.
