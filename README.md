# Python-programmin-practice
# I started my python programming language practice with the assignment 1. I got this assignment from my instructor.

PROBLEM- 1
# Write a Python program to print your personal details on the output screen.
print ("Name- Akash Mathane")
print ("Phone no. - 7038588211")
print ("Residential address- Amravati")
print ("Email address- akash.p.mathane@gmail.com")

PROBLEM- 2
# Write a Program to accept two numbers and display their sum.
print ( 2 + 2)
print ( 200 + 2)
print ( 225 + 2)
print ( 230 + 2)
print ( 235 + 2)

PROBLEM- 3
# Write a Program to accept side of square and calculate area and perimeter of Square.

a = 5 # side of square is 5
area = a*a # formular of area 
perimeter = 4*a # formular of perimeter

print('area of square is', area)
print('Perimeter of the square is', perimeter)

PROBLEM- 4
# Write a Program to accept radius of circle and calculate area and circumference of Circle.

r = 5 # radius of circle is 5
area = math.pi * a * a # formular for area of circle 
perimeter = 2* math.pi * r # formular for perimeter of circle

print('area of square is', area)
print('Perimeter of the square is', perimeter)


PROBLEM- 5
# Write a Program to calculate simple interest.
# Note: accept required information from user.

p = int(input(" Tell me the initial principal balance "))
t = int(input(" Tell me the time you need "))
r = int(input(" Tell me the annual interest rate "))
simple_intrest = (p*t*r)/100 # P = initial principal balance , T = time (in years) , R = annual interest rate

print (" Simple intrest is ", simple_intrest)


PROBLEM- 6
# Write a Program to accept 3 numbers and display smallest and largest number.

a = int(input(" First number "))
b = int(input(" Second number "))
c = int(input(" Third number "))

def largest (a,b,c):
    if (a>b and a>c):
        print("The largest no. is ",a)
    elif (b>a and b>c):
        print("The largest no. is ", b)
    else:
        print("The largest no. is ", c)
    
def smallest(a,b,c):
    if (a<b and a<c):
         print("The smallest no. is ",a)
    elif (b<a and b<c):
         print("The smallest no. is ", b)
    else:
         print("The smallest no. is ", c)

largest (a,b,c)
smallest(a,b,c)

PROBLEM- 7
# Write a Program to accept two numbers, and one of the following operators +, -, *, /. Perform the given operation
# and display result.
a = int(input("write the first value for a "))
b = int(input("write the second value for b "))
print (a + b)
print ( a - b)
print ( a * b)
print ( a / b)

PROBLEM- 8

# Write a Program to accept a number and decide whether it is an odd or even number.

number = int(input("write the no. to check odd or even "))

if (number%2) == 0:
    print("your number is even number ")
else:
    print("your number is odd number")

PROBLEM- 9
# Write a Python program to get the Python version you are using.

print("Python version")
print (sys.version)
print("Version info.")
print (sys.version_info)

print("----------------")

import platform
print(platform.python_version())

PROBLEM- 10
# Write a Python program to display the examination schedule. (extract the date from exam_st_date)
# exam_st_date = (11, 12, 2018)
# Sample Output : The examination will start from : 11 / 12 / 2018

date = 11
month = 12
year = 2018

print("The examination will start from : ", date, month, year)

print("----------------")

exam_st_date = (11, 12, 2018)
print( "The examination will start from : %i / %i / %i" %exam_st_date)


PROBLEM- 11
# Write a Python program to check weather user inputted number is palindrome or not.

no = int(input("write no. here to check "))
rem = 0
rev = 0
org = no

while(no>0):
    rem = no%10
    rev = rev *10 + rem 
    no = no//10
         
print("original number = ",org)
print("reverse  number = ",rev)

if(org == rev):
    print("The given no. is palindrom")
else:
    print("Given number is not palindrom")
    
    
PROBLEM- 12
# Write a Python program to check weather user inputted number is prime or not.

no = int(input("write no. here to check "))
start = 2
end = no//2
status = 0
for x in range(start, end+1):
    if(no %  x == 0):
        status = 1
    
if(status == 1):
    print("Not prime number")
else:
    print("Prime number")


PROBLEM- 13
# Write a Python program to check weather user inputted number is Armstrong or not.
no = int(input("write no. here to check "))
rem = 0
rev = 0
org = no

while(no>0):
    rem = no%10
    rev = rev + rem ** 3
    no = no//10
         
print("original number = ",org)
print("reverse  number = ",rev)

if(org == rev):
    print("The given no. is Armstrong")
else:
    print("Given number is not Armstrong")

PROBLEM- 14
# Write a program which will find all such numbers which are divisible by 7 but are not a multiple of 5, between 2000
# and 3200 (both included).

li = []
for i in range(2000,3200):
    if i%7 == 0 and i%5 != 0:
        li.append(str(i))
        
print(','.join(li))


PROBLEM- 15

# Write a program, which can compute the factorial of a given numbers.
# Suppose the following input is supplied to the program:
# 8
# Then, the output should be:
# 40320

no = 8
fact = 1

for i in range(1, no+1):
    fact = fact * i
    print("The factorial of",no,"is",fact)
    



    

PROBLEM- 16
# Write a Python program to test whether a passed letter is a vowel or not

letters = input("Enter the letter here: ")

if letters in ('a','e','i','o','u'):
    print("Your letter is vowel")
else:
    print("Your letter is not vowel")

PROBLEM- 17
# Modify above program to accept name and number. Display name for given number of times

name = input("Enter the name here: ")
vowel = 0
for i in name:
    if (i == 'a' or i == 'e' or i == 'i' or i == 'o' or i == 'u'):
        vowel = vowel + 1
        print("total numbers of vowels are", vowel)




PROBLEM- 18

# Write an Program to accept two numbers from user and display all numbers between those numbers
# Example: If user enters 3 and 9 program should display numbers 3,4,5,6,7,8 and 9

no = 2

for i in range(3,10):
    no = no + 1
    print(no)
    


PROBLEM- 19

# Write a Program to display following pattern 
# Modify above program to accept a number (between 1 to 9) from user and display above pattern accordingly.
# 1
# 22
# 333
# 4444
# 55555
# 666666
# 7777777
# 88888888
# 999999999


n = int(input("Enter number of rows: "))

for i in range(1,n+1):
    for j in range(1, i+1):
        print(i, end="")
    print()
    
print("------------------")

n = int(input("Enter number of rows: "))

for i in range(10):
    print(str(i) * i)


PROBLEM- 20
# pattern programs

n = int(input("Enter number of rows: "))

for row in range(n,0,-1):
    for col in range(1, row + 1):
        print(col,end = "")
    print()
    
print("------------------")

n = int(input("Enter number of rows: "))

for i in range(n,0,-1):
    for col in range(1, i + 1):
        print(i,end = "")
    print()


PROBLEM- 21
# Write an Program to display following pattern
# 111111111
# 22222222
# 3333333
# 444444
# 55555
# 6666
# 777
# 88
# 9


n = int(input("Enter number of rows: "))
b = 0

for i in range(n, 0, -1):
    b += 1
    for j in range(1, i + 1):
        print(b, end=' ')
    print()

PROBLEM- 22
# Write a Program to display following pattern
# ********
# *******
# ******
# ****
# ***
# **
# *

n = int(input("Write number here to print stars "))


for i in range(n,0,-1):
    for j in range(1, i + 1):
        print("*", end=' ')
    print()

PROBLEM- 23
# Write a Program to display following pattern
# Note: There are nine * in last line
#     *
#    ***
#   *****
#  *******
# *********

n = int(input("Write number here to print stars "))

for i in range(0,n):
    for j in range(0,n-i-1):
        print(end = " ")
    for j in range(0,i+1):
        print("*", end = " ")
    print()


PROBLEM- 24
# 24 Write a Program to display following pattern

n = int(input("Write number here to print stars "))

for i in range(0,n):
    for j in range(0,i):
        print("*", end = " ")
    print()

PROBLEM- 25
# 25 Write an Program to display following pattern


PROBLEM- 26
# Write a Program to display numbers 10 to 1 in reverse order.
# Note: Output should be 10, 9, 8, 7, ….., 2, 1

n = int(input("write the numer here to start reverse order: "))

while(n>=1):
    print(n, end = " ")
    n = n - 1
    
PROBLEM- 27
# Write a Program to accept number and display its table.
# Note: If user enters 7 output should be as follows

n = int(input('writr a number here to start a table: '))


for i in range(1,11):
    print(n, "x", i, "=", n*i )


PROBLEM- 28
# Write a Python program to print the following string in a specific format (see the output).
# Sample String= "Twinkle, twinkle, little star, How I wonder what you are! Up above the world so high, Like a
# diamond in the sky. Twinkle, twinkle, little star, How I wonder what you are!"

print("Twinkle, twinkle, little star,\n\t How I wonder what you are!\nUp above the world so high,\n\t\tLike a diamond in the sky.\nTwinkle, twinkle, little star,\n\tHow I wonder what you are!" )


PROBLEM- 29
# Write a Program to display 10 numbers that are divisible by 5 and 7

a = int(input("Enter start number:"))
 
b = int(input("Enter last number:"))

for i in range(a,b):
    if ((i%5==0) and (i%7==0)):
        print(i)
        

    
PROBLEM- 30
# Write a program to calculate time reached to given destination. Accept following details from the user.

Name_of_destination = input("Name of destination: ")
Distance_to_destination = int(input("Distance to destination: "))
Speed_per_Kilometre = int(input("Speed per Kilometre: "))
No_of_breaks_in_journey = int(input("No of breaks in journey: "))
Time_per_break = int(input("Time per break: "))




# 31
a = [1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89]

for i in a:
    if(i<5):
        print(i, end=" ")
print()        
#Instead of printing the elements one by one, make a new list that has all the elements less than 5 from
#this list in it and print out this new list.
a = [1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89]
b = []
for i in a:
    if i < 5:
        b.append(i)
print(b)

#Write this in one line of Python. 
a = [1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89]
b = []
[b.append(i) for i in a if i < 5]
print(b)



#Ask the user for a number and return a list that contains only elements from 
#the original list a that are smaller than that number given by the user.
a = [1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89]
b = []
user_input = int(input('Select a number: \n'))
[b.append(i) for i in a if i < user_input]
print(b)


PROBLEM- 32
# 32 Ask the user for a string and print out whether this string is a palindrome or not. (A palindrome is a string that reads
# the same forwards and backwards.)

string = input("Type your string here to check ")

if (string == string[::-1]):
    print("string is palindrom",string)
else:
    print("string is not palindrom")
    

PROBLEM- 33
# Ask user to enter 10 elements in the list and find minimum and maximum of from the list.

list = [100,200,300,400,500,600,700,800,900]

print("minimum no. is ", min(list))
print("maximum no. is ", max(list))
print("Index no. is ", list.index(700))

PROBLEM- 34
# 34 Write a program to replace minimum element from the list by
#     “maximum element+1” and display the result.

list = [2, 4, 6, 8, 10, 12, 14, 16,1, 3, 5, 7, 9, 11, 13, 15, 17, 19, 21, 23, 25]


        

PROBLEM- 35
# 35 Ask user to enter 10 elements in the list and find even and odd from the list.

list = [2, 4, 6, 8, 10, 12, 14, 16,1, 3, 5, 7, 9, 11, 13, 15, 17, 19, 21, 23, 25]

for x in (list):
    if (x%2 == 0):
        print("even no. is ",x)
    elif(x%2 != 0):
        print("odd no. is", x)

PROBLEM- 36
# Ask user to enter 10 elements in the list and find prime number from the list.

no = int(input("Enter, how many elements you want: "))
li = []
start = 2
end = no//2
status = 0

for i in range (no):
    elements = input("Enter here:" )
    li.append(elements)
    
for x in range(start, end+1):
    rem = no % x
    if(rem == 0):
        status = 1
        
    
    
if(status == 0):
    print("{} Not prime number".format(no))
else:
    print("{} Prime number".format(no))
    
                

             
PROBLEM- 37
# Ask user to enter 10 elements in the and find all Armstrong numbers from the list.

no = int(input("write no. here to check "))
li = []
rem = 0
rev = 0
org = no

for i in range (no):
    elements = input("Enter here:" )
    li.append(elements)
    
while(no > 0):
    rem = no%10
    rev = rev + rem ** 3
    no = no//10
         
if(org == rev):
    print("The given no. is Armstrong")
else:
    print("Given number is not Armstrong")      



PROBLEM- 38
# 38 Write a program to create 3 list and restrict the user to insert only prime number in first_list, only palindrome number
# in second_list, only Armstrong number in third_list.

list_1 = int(input("For list_1: "))
list_2 = int(input("For list_2: "))
list_3 = int(input("For list_3: "))

for a in range (list_1):
    elements = input("Enter here:" )
    li.append(elements)
    while True:
        
               


for b in range (list_2):
    elements = input("Enter here:" )
    li.append(elements)

for c in range (list_3):
    elements = input("Enter here:" )
    li.append(elements)


PROBLEM- 39
# 39 With a given integral number n, write a program to generate a dictionary that contains (i, i*i) such that is an integral
# number between 1 and n (both included). and then the program should print the dictionary.

number = int(input("Type a number: "))

numberDict = {}
for i in range(1, number+1):
    numberDict[i] = i*i

print(numberDict)



