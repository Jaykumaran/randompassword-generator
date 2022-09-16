#PY PASS GENERATOR
import random


small_letters=['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z']
capital_letters=['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
numbers=['0', '1', '2' , '3', '4','5','6','7','8','9']
symbols=['!', '@', '#', '$', '%' , '&', '*','(','~']
print("Welcome to PyPassword Generator")
no_of_small_letters=int(input(f"How many small letters would you like in your password? : \n "))
no_of_capital_letters=int(input(f"How many capital letters would you like in your password? : \n "))
no_of_symbols=int(input(f"how many symbols would you like? to have in passwords? :  \n"))

no_of_numbers=int(input(f"how many numbers would you like to have in pass? \n"))


#hard level
password_list=[]

for char in range(1, no_of_capital_letters+1):

  password_list+= random.choice(capital_letters)
  
for char in range(1, no_of_small_letters+1):

  password_list+= random.choice(small_letters)
for char in range(1, no_of_numbers+1):

  password_list+= random.choice(numbers)
for char in range(1, no_of_symbols+1):

  password_list+= random.choice(symbols)
print(password_list)
random.shuffle(password_list)
print(password_list)
random_password=""
for char in password_list:
  random_password+=char
print(f"your password is :{random_password}")


output sample:


Welcome to PyPassword Generator
How many small letters would you like in your password? : 
 2
How many capital letters would you like in your password? : 
 4
how many symbols would you like? to have in passwords? :  
5
how many numbers would you like to have in pass? 
7
['O', 'B', 'V', 'L', 'h', 'l', '8', '8', '4', '0', '5', '0', '0', '(', '$', '#', '#', '~']
['4', 'B', '(', '8', 'h', 'l', '0', '8', 'L', '0', 'O', '$', '~', '0', '5', 'V', '#', '#']
your password is :4B(8hl08L0O$~05V##
 




