#Rock paper scissor game
import random
i=0
win=0
equal=0
lose=0
remain=9
print("Rock paper scissor game \nNumber of choice are 10")
while i<10:
    computer=random.choice(["rock","paper","scissor"])
    in_put=str(input("rock,paper,scissor write select any one? \n"))
    if computer=="rock" and in_put=="paper":
        print("you win")
        print(f"remain:{remain}")
        remain=remain-1
        win=win+1
        i=i+1
    elif computer=="rock" and in_put=="scissor":
        print("you lose")
        print(f"remain:{remain}")
        remain = remain - 1
        lose=lose+1
        i=i+1
    elif computer=="paper" and in_put=="rock":
        print("you lose")
        print(f"remain:{remain}")
        remain = remain - 1
        lose=lose+1
        i=i+1
    elif computer=="paper" and in_put=="scissor":
        print("you win")
        print(f"remain:{remain}")
        remain = remain - 1
        win=win+1
        i=i+1
    elif computer=="scissor" and in_put=="rock":
        print("you win")
        print(f"remain:{remain}")
        remain = remain - 1
        win=win+1
        i=i+1
    elif computer=="scissor" and in_put=="paper":
        print("you lose")
        print(f"remain:{remain}")
        remain = remain - 1
        lose=lose+1
        i=i+1
    elif computer==in_put:
        print("you equal")
        print(f"remain:{remain}")
        remain = remain - 1
        equal=equal+1
        i=i+1
    else:
        print("wrong input please try again !")
print("Game over")
print(f"Result:- Win:{win}, Equal:{equal}, Lose:{lose}")