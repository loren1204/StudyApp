# StudyApp
//README.md file for Study Invaders Code: 
# Study Invaders

**Study Invaders** is a retro-inspired 2D educational shooter built with C++ and SFML. The player controls a spaceship and defeats enemies by correctly typing terms based on definitions. It’s a gamified flashcard experience, perfect for studying and learning interactively!

---

##Gameplay Overview

- Each enemy is tied to a definition from a flashcard file.
- The player must type the correct term letter-by-letter to fire bullets at the enemy.
- Enemies move toward the player. If they reach the player, a heart is lost.
- The game ends in a **Game Over** screen if all lives are lost.
- If all flashcards are answered correctly, a **YOU WIN** screen appears.

---

##Educational Goal

- Reinforce memory and recall through active gameplay.
- Supports custom flashcard lists for any subject.

---

##Features

- 15-round flashcard enemy system
- Bullet system based on correct letter input
- Random bullet color and enemy tracking
- Definition box with auto-wrapping text
- Pixel-art UI with **Game Over** and **You Win** screens
- Retry button and keyboard shortcuts
- Support for alphanumeric answers (letters + numbers)

---

##Project Structure

```bash
.
├── main.cpp                 # Main game logic
├── flashcard.h             # Flashcard class (holds question-answer pair)
├── flashcard.cpp
├── flashcardmanager.h      # Manages vector of flashcards and file loading
├── flashcardmanager.cpp
├── programming.txt         # Sample flashcard file (question:definition pairs)
├── assets/
│   ├── backgroundgame.png  # Background image
│   ├── alien.png           # Enemy sprite
│   ├── player.png          # Player spaceship sprite
│   ├── heart_resized.png   # Life icon (hearts)
│   ├── game_over.png       # Game Over screen
│   ├── you_win.png         # You Win screen
│   └── 8514FIX.ttf         # Pixel-style font

//README.md file for Flashcards Code
# Flashcard Viewer & Quiz App (SFML + C++)

A simple flashcard-based quiz application built using C++ and SFML. This app provides two modes: **Flashcard Mode** for studying and **Quiz Mode** for testing your knowledge interactively using keyboard input and a clean graphical interface.

---

##Controls

| Key           | Action                              |
|---------------|--------------------------------------|
| `Tab`         | Toggle between Flashcard and Quiz mode |
| `Space`       | Flip between Question/Answer (Flashcard mode) |
| `Left/Right`  | Navigate through flashcards (Flashcard mode) |
| `Enter`       | Submit answer (Quiz mode)            |
| `Backspace`   | Delete last character in input (Quiz mode) |
| Text Input    | Type your answer (Quiz mode only)    |

---

##How It Works

- **main.cpp**: Core logic that launches the SFML window and controls both study and quiz modes.
- **Flashcard Mode**: Displays question or answer text and allows flipping or navigating.
- **Quiz Mode**: Prompts for input, checks correctness, and displays instant feedback.
- Toggle between modes using the `Tab` key.

---

##Project Structure

```bash
.
├── main.cpp               # SFML GUI + Game Loop (Flashcard and Quiz logic)
├── flashcard.h            # Flashcard class declaration (Q&A data model)
├── flashcard.cpp          # Flashcard class definition
├── flashcardmanager.h     # Manages list of flashcards and quiz operations
├── flashcardmanager.cpp   # File loading, quiz logic, access to flashcard data
├── programming.txt        # Flashcard source file (Question/Answer format)
├── arial.ttf              # Font used in the GUI
