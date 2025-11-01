# 🎯 Mini Project: Number Guessing Game

*Project Author:* Damilola Amusan
*Peer Reviewer:* Olubukola Abraham  
*Track:* Beginner (No Prior Experience)

---

## 💡 Project Description

This mini project demonstrates the use of programming basics — variables, loops, and decision control — to create a simple number guessing game.  
The program chooses a random number between 1 and 10, and the user keeps guessing until they get it right.

---

## 🧩 Algorithm (Pseudocode)

Algorithm: Number Guessing Game

1. Start the program  
2. Generate a random number between 1 and 10 and store it as the secret number  
3. Ask the user to guess the number  
4. WHILE the guess is not equal to the secret number  
   - IF the guess is lower than the secret number, print “Too low! Try again.”  
   - ELSE IF the guess is higher than the secret number, print “Too high! Try again.”  
   - Ask the user to guess again  
5. IF the guess equals the secret number, print “🎉 Congratulations! You guessed it right!”  
6. End the program

---

## 🔄 Collaboration Workflow

1. Create a new GitHub repository named *number-guessing-game*.  
2. Push this README file to your repo.  
3. Add your peer as a *collaborator*.  
4. Wait for your peer to review and make improvements via a *pull request*.  
5. Review their pull request → Approve or request changes → Merge if satisfied.

---

## 💻 Optional: Python Implementation (for practice)

```python
import random

secret_number = random.randint(1, 10)
guess = None

print("Welcome to the Number Guessing Game!")

while guess != secret_number:
    try:
        guess = int(input("Guess a number between 1 and 10: "))
        if guess < secret_number:
            print("Too low! Try again.")
        elif guess > secret_number:
            print("Too high! Try again.")
        else:
            print("🎉 Congratulations! You guessed it right!")
    except ValueError:
        print("Please enter a valid number.")

### There you have it! Your number guessing game is ready
