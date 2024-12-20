# flow-control-loops

---

### Lab 1: Guess the Number

**Word Problem:**  
Create a number-guessing game where the computer picks a random number between 1 and 10, and the user has 3 attempts to guess the number.

**Instructions:**  
1. Use `random.randint(1, 10)` to generate a random number.
2. Create a loop that allows the user to guess the number up to 3 times.
3. After each guess, tell the user whether their guess is too high, too low, or correct.
4. If the user guesses the number or runs out of attempts, print an appropriate message.

**Concepts Used:**  
- `input()`, `while` loop, `if-else` statement, `import random`, flow control
import random

secret_number = random.randint(1, 10)

attempts = 3

for attempt in range(attempts):
    guess = int(input(f"Attempt {attempt + 1}/{attempts}: Guess the number (between 1 and 10): "))
    
    if guess == secret_number:
        print("Congratulations! You've guessed the correct number.")
        break
    elif guess < secret_number:
        print("Your guess is too low.")
    else:
        print("Your guess is too high.")

    if attempt == attempts - 1:
        print(f"Sorry, you've used all your attempts. The correct number was {secret_number}.")

---

### Lab 2: Countdown Timer

**Word Problem:**  
Write a countdown timer that counts down from a number the user inputs to 1. The countdown should print each number.

**Instructions:**  
1. Ask the user to input a number to start the countdown.
2. Use a `while` loop to decrement the number.
3. Print the countdown until it reaches 1.

**Concepts Used:**  
- `input()`, `while` loop, `print()`
number = int(input("Enter a Number to start the countdown: "))

while number >= 1:
  print(number)
  number -= 1

---

### Lab 3: Sum of Numbers

**Word Problem:**  
Write a program that asks the user for a number and calculates the sum of all numbers from 1 to that number.

**Instructions:**  
1. Ask the user to input a number.
2. Use a `for` loop to sum the numbers from 1 to the user’s input number.
3. Print the total sum.

**Concepts Used:**  
- `input()`, `for` loop, summing
number = int(input("Enter a number: "))

total_sum = 0

for i in range(1, number + 1):
  total_sum += i

print(f"the sume of all numbers from 1 to {number} is: {total_sum}")

---

