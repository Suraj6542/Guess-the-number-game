# Guess-the-number-game
#This python code is basically a game like guess the number
import random

print("Guess the number between 1 and 100")

random_number = random.randint(1, 100)
guess = None

while guess != random_number:
    guess = int(input("Your guess: "))
    if guess > random_number:
        print("Too high. Try again.")
    elif guess < random_number:
        print("Too low. Try again.")
    else:
        print("You got it! The number was", random_number)
