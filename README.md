# number-guessing-game
import random
winning_num = random.randint(1,100)
guess = int(input("Guess a number between 1 and 100: "))
while guess != winning_num:
    guess = int(input("Guess a number between 1 and 100: "))

    if guess > winning_num:
        print("Try lower!")
    elif guess < winning_num:
        print("Try higher!")
    elif guess == winning_num:
        print("You guessed right!")
        break
