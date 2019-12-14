# Guessing-Number-Game-in-python
import random

number = random.randint(1,9)
guess = 0
count = 0
while guess != number and guess != exit:
    guess = input("Enter the number that you want to guess: ")
    
    if guess == exit:
        break
        
    guess = int(guess)
    count += 1
    
    if guess < number:
        print("Too low!")
    elif guess > number:
        print("Too high!")
    else:
        print("Congrats!You have guessed the right number!")
        print("This took you only {} times".format(count))
