# dice
import random
print("This game to guess a number from the dice and then the dice is thrown. If you guesss the same number as outcome on the dice u won .If not ulose")
b,s=1,0
while b==1:
    a=int(input("enter a number between 1 to 6:"))
    x=random.randint(1,6)
    if 1<=a<=6:
        if a==x:
            print("CONGRATS! YOU WON.")
            s+=10
            print("Score=",s)
        else:
            print("Better Luck Next Time! Computer generated number is",x)
            s-=5
            print("Score=",s)
    else:
        print("Enter a number between 1 to 6")
    b=int(input("want to play more enter 1 and for exist enter 0:"))
