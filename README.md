# Number---Guessing---Game
import random

secret_number = random.randint(1, 100)
attempts = 7

print("Welcome to Number Guessing Game!")
print("Guess a number between 1 and 100")

for i in range(attempts):
    guess = int(input("Enter your guess: "))

    if guess == secret_number:
        print("Congratulations! You guessed the number.")
        break
    elif guess < secret_number:
        print("Too Low!")
    else:
        print("Too High!")

    print("Attempts left:", attempts - i - 1)

else:
    print("Game Over!")
    print("The correct number was:", secret_number)
