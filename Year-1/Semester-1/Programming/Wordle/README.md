# Wordle — Kotlin

A simplified, console-based version of Wordle developed for the **first practical assignment** in the **Programming** course at **Instituto Superior de Engenharia de Lisboa (ISEL)**.

**Academic year:** 2026/2027  
**Degree:** Computer Science and Engineering  
**Year / semester:** 1st year / 1st semester  
**Language:** Kotlin

## Objective

The program randomly selects a secret five-letter word. The player has up to **six attempts** to guess it. After each guess, the program displays feedback for every letter.

| Symbol | Meaning |
| --- | --- |
| `+` | The letter is correct and in the correct position. |
| `#` | The letter occurs in the secret word but is in a different position and has not already been counted. |
| `_` | The letter is absent or has no remaining unmatched occurrence. |

The game ends when the entire word is guessed or all attempts have been used.

## Implemented functions

The assignment provided the `main` function and word list and required the implementation of four functions:

- `readGuess(length: Int)`: reads a guess, converts it to uppercase, and checks its length and characters.
- `getResult(secret: String, guess: String)`: returns the per-letter feedback, taking repeated letters into account.
- `allCorrect(result: String)`: checks whether all five letters are in their correct positions.
- `noRepeats(s: String)`: checks whether a word contains repeated characters. This helper is included but is not used by the current word-selection line.

## Source file

- [`Jogowordle.kt`](Jogowordle.kt) — Kotlin source code for the console game.

## Run

Open `Jogowordle.kt` in a Kotlin-compatible development environment and run the `main` function.

Alternatively, with the Kotlin command-line compiler installed:

```bash
kotlinc Jogowordle.kt -include-runtime -d wordle.jar
java -jar wordle.jar
```

## Academic context

This project was developed as an academic programming exercise. The assignment supplied the initial program structure and asked students to complete the game logic in the four functions listed above.
