# Double-six-dice-game-
import random



def roll_dice():

    return random.randint(1, 6), random.randint(1, 6)



def play_game():

    print("Welcome to the Double Six Dice Game!")

    

    while True:

        input("Press Enter to roll the dice...")

        die1, die2 = roll_dice()

        print(f"You rolled: {die1} and {die2}")

        

        if die1 == 6 and die2 == 6:

            print("Congratulations! You rolled double sixes! You win!")

            break

        else:

            print("Sorry, you didn't roll double sixes. Try again!")



if __name__ == "__main__":

    play_game()
