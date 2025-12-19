# Pygame Unit Testing – Space Invader Game

## Student Information

* **Name:** Phuntsho Dema
* **Programme:** Bachelor of Business Intelligence (BBI)
* **Section:** B
* **Student ID:** 03230228

---

## Project Title

**Unit Testing Core Game Functionalities Using Python (Pygame)**

---

## Project Description

This project focuses on testing the core functionalities of a simple **Space Invader–style game** developed using the **Pygame** library. The testing is implemented using Python’s built-in **unittest** framework. The goal is to verify that essential game mechanics work correctly before integrating them into the full game.

The program emphasizes **test-driven development (TDD)** principles by validating individual components such as player movement, collision detection, scoring, and game-over conditions.

---

## Key Functionalities Tested

The following core game features are identified and tested:

* Player movement
* Collision detection between bullets and invaders
* Score updating mechanism
* Game over condition
* Basic game state validation

---

## Libraries Used

* **pygame** – for game environment simulation
* **unittest** – for writing and running unit tests
* **random** – for generating random invader positions
* **math** – for collision distance calculation

---

## Test Case Structure

The test cases are written inside the `TestGame` class, which inherits from `unittest.TestCase`.

### 1. Test Setup (`setUp` Method)

The `setUp()` method initializes:

* Pygame screen
* Player position and movement variables
* Bullet position and state
* Invader positions and movement values
* Initial score

This method runs **before every test**, ensuring a fresh and consistent test environment.

---

## Test Case Explanations

### 1. Player Movement Test

This test simulates a left arrow key press and verifies that the player’s X-position decreases accordingly.

**Purpose:** Ensure player movement responds correctly to keyboard input.

---

### 2. Collision Detection Function

A helper function calculates the distance between a bullet and an invader using the Euclidean distance formula.

**Purpose:** Determine whether a collision occurs when the distance is within a defined threshold.

---

### 3. Collision Detection Test

This test verifies:

* Collision is detected when the bullet is near an invader
* No collision is detected when the invader is far away

**Purpose:** Validate accuracy of the collision detection logic.

---

### 4. Scoring Test

This test checks whether the score increases when a collision occurs and remains unchanged when there is no collision.

**Purpose:** Ensure score updates only under valid collision conditions.

---

### 5. Game Over Condition Test

This test simulates a game-over scenario by forcing an invader beyond the player boundary.

**Purpose:** Confirm that the game correctly identifies and triggers the game-over state.

---

## How to Run the Tests

1. Ensure Python and Pygame are installed
2. Save the file as `test_game.py`
3. Run the following command in the terminal:

```bash
python test_game.py
```

---

## Learning Outcomes

Through this project, the following skills were developed:

* Writing unit tests using Python
* Testing game logic without full gameplay execution
* Using Pygame in a controlled testing environment
* Applying mathematical logic for collision detection
* Understanding test-driven development concepts

---

## Conclusion

This project demonstrates how unit testing can be applied to game development to verify essential mechanics before full-scale implementation. By testing individual components independently, the reliability and stability of the game logic can be significantly improved.

---

## References

* Python Documentation – `unittest` module
* Pygame Official Documentation
* Stack Overflow – Game testing and collision detection examples
