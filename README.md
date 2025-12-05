# 🎮 C# Console Mini-Game Challenge

![Gameplay Preview](./screenshot.png)
*(Upload an image of your game here, e.g., screenshot.png)*

## 📝 Description

This project is a console application developed as part of a programming "Challenge Project." The goal is to build a functional mini-game that manages character movement, object consumption (food), and player state changes based on in-game actions.

The game demonstrates the use of C# methods to organize logic, handle user input, and manage the game state within a console environment.

## ✨ Key Features

The project implements the following core game mechanics:

- **Collision Detection:** logic determines if the player's coordinates match the food's coordinates (consumption).
- **Dynamic Status System:**
    - The player's appearance changes to match the food consumed using the `states` and `foods` arrays.
- **Status Effects:**
    - **Freeze:** Certain food types temporarily freeze the player's movement.
    - **Speed Boost:** Other food types allow the player to move faster (optional feature logic).
- **Procedural Regeneration:** Uses the `Random` class to redisplay food in a new, valid location after consumption.
- **Input Validation:** The game terminates execution if an unsupported key (non-directional) is pressed.
- **Responsive Stability:** Contains logic to terminate the game immediately if the terminal window is resized, preventing rendering crashes.

## 🏗️ Code Structure

The application logic is organized into clean, reusable methods and specific data structures:

### Variables & Data
- **Coordinates:** Tracks `(x, y)` positions for both the Player and the Food.
- **Console Layout:** Variables to monitor Terminal height and width.
- **Assets:**
    - `states`: An array defining valid player appearances.
    - `foods`: An array defining available food types.
- **State Trackers:** Variables to store the current index of the player's appearance and the food being displayed.

### Helper Methods
- `TerminalResized()`: Compares current console size against initial values to detect changes.
- `ShowFood()`: Generates random coordinates and displays a random food string.
- `ChangePlayer()`: Updates the player's string representation based on the food index.
- `FreezePlayer()`: Implements a delay to pause movement.
- `Move()`: Calculates the new player position based on directional key input.
- `InitializeGame()`: Sets up the initial terminal size and variables.

## 🚀 Learning Objectives

This project was created to demonstrate proficiency in:
* Using **Visual Studio Code** to develop .NET console applications.
* Implementing logical workflows using **C# Methods** with required and optional parameters.
* Understanding and modifying existing code design.
* Using control structures (`switch`, `if-else`, `for` loops).
* Manipulating console coordinates and using the `Random` class.

## 🛠️ Technologies Used

* **Language:** C#
* **Framework:** .NET
* **IDE:** Visual Studio Code

## 💻 How to Run

1.  Clone this repository.
2.  Open the folder in Visual Studio Code.
3.  Open the integrated terminal.
4.  Run the command:
    ```bash
    dotnet run
    ```

## 📧 Contact

If you have any questions about the code or suggestions for improvement, feel free to reach out:

📩 **Email:** mariusc0023@gmail.com

---
*This project is for educational purposes to test C# procedural programming skills.*