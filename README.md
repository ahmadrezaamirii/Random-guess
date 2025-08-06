# Random-guess
---
### a game that cooden about a Random guess . the computer select a number between 1 to 100 and we must guess that and when the guess is correct, we win the game .
***
At the first , Library:
````
import random
````

Use the functions:
Get input =>
````
def get_guess():
    ans = int(input("Whats your Guess? "))
    return ans

````
The fuction of calculate and get hints:

````
def win(computer_num , guess) :
    return computer_num == guess

def answer(computer , user) :
    if computer > user :
        return "My number is larger"
    if computer < user :
        return "My number is smaller"
    return "goood job! you won :) "
````
ask about play agian? :
````
def finish(number , count):
    answer = input("Do you want play again? (Y/N) ") 
    if answer.upper() == 'YES':
        return True
    else :
        return False


````



````
continue_playing = True
while (continue_playing):
    computer_num = random.randint (1 , 100)
    guess = 0
    count = 0
    
    while (not win(computer_num , guess)):
        guess = get_guess()
        count += 1
        print(answer(computer_num , guess))
        
    continue_playing = finish(computer_num , guess)
````
****
[My GitHub profile](https://github.com/ahmadrezaamirii)

[My LinkedIn](https://www.linkedin.com/in/ahmadreza-amiri-46936b1b2/)