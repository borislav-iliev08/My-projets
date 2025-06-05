# My projets
This is my projects from beginning in my career as software engeneering
# 🔐 Login Simulation (Python Project)
A simple Python project that simulates a user login system.  
It includes user registration, username verification, password checking with limited attempts, and clear user feedback.

---

##  What I used
- Python code with functions
- Basic logic for user authentication
- Using loops and conditionals
- Creating clean, readable code

------
## Code

username=input("You will register with this username:")

password=input('Set strong password adn remember it :')

attempts = 3

print("======\Entering in the system/======")

new_user=input("Please enter your saved username:")

while new_user != username:
    print(f'{new_user} do not match !')
    new_user = input()
    if new_user == username:
        print('This user was fount ,now type password!')

new_pass = input("Enter your password here:")

while new_pass != password:
        print(f'This password is wrong! You have {attempts} attempts left! ')
        attempts-=1
        if attempts==-1:
            print(f'Please try again later! ')
            break
        new_pass = input('Password:')
        elif new_pass == password:
            print(f'Welcome back {username}!')
            break







----------------
---------------
----------------
------------------
-------------------

#  Mini game(Guess the number)
Easy Python project where the system create random number from range and you need to guess it ,the game dont stop till you type "Stop".
---------
##  What I used
- Python code with functions
- Basic logic for user authentication
- Using loops and conditionals
- Creating clean, readable code
 ----------

## Code

import random
print(f"Hello this is 'Guess the number' if you want to stop playing type 'Stop'")
print('==============')
number=input("Please enter you're guess here: ")
while number!='Stop':
   random_numb=random.randint(1,20+1)
   int_num=int(number)
   if int_num==random_numb:
    print(f'Exellent you guessed it right!')
    break

   else:
    print(f'Wrong try again!The right number was {random_numb}')
    number = input("Please enter you're guess here: ")
    continue
    if number=='Stop':
        print(f'Have a grat day!Come back soon!')
