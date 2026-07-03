# numbe-guessing-game-python
Python number guessing game using loops, conditions, and the random module.
print("This is a number guessing game\ncomputer will assign a random number from 0 to 99 and you need to find that number!")
import random
computer=random.choice(range(100))
count=0
while True:
    num=int(input("Guess the number:"))
    if(num>=100 or num<0):
        print("guess only between 0 to 99")
    else:
        if(computer==num):
            count=count+1
            print(f"You guess the number in {count} attempts")
            break
        elif(num>computer):
            print("lower")
            count=count+1
        else:
            print("higher")
            count=count+1
        

