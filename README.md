#rock,paper,scissors game
import random

while True:
    choices= ["rock","paper","scissors"]
    computer= random.choice(choices)

    player=None
    while player not in choices:
    
    palyer=input("Enter your choice ").lower()
     
    if player==computer:
            print("computer:",computer)
            print("player:",player)
            print("Tie!")
    
    elif player=="rock":
        if computer=="scissors":
             print("computer:",computer)
             print("player:",player)
             print("you win!")
        if computer=="paper":
             print("computer:",computer)
             print("player:",player)
             print("you lose!")  
    
    elif player=="scissors" :
        if computer=="rock":
            print("computer:",computer)
            print("player:",player)
            print("you lose!")  
        if computer=="paper":
            print("computer:",computer)
            print("player:",player)
            print("you win!")  
            
    elif player=="paper" :
        if computer=="rock":
            print("computer:",computer)
            print("player:",player)
            print("you win!")  
        if computer=="scissors":
            print("computer:",computer)
            print("player:",player)
            print("you lose!")  
    
    playAgain=input("play again? (yes/no): ").lower()
    if playAgain != "yes":
         break
print("Bye!")
