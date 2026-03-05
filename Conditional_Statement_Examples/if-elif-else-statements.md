## 1. Write a program to check if a number is positive, negative, or zero.

```python
num=float(input("Enter the number"))
if num > 0:
    print("Number is Positive")
elif num < 0:
    print("Number is Negetive")
else:
    print("Number is Zero")
```

Output:-
```text
Enter the number 12
Number is Positive
```
```text
Enter the number 0
Number is Zero
```
```text
Enter the number -12
Number is Negetive
```

---

## 2. Write a program to find the largest among two numbers.

```python
num1,num2=input("Enter the both the numbers with comma between them").split(",")
if float(num1)>float(num2):
    print(f"{num1} is greater")
elif float(num1)<float(num2):
    print(f"{num2} is greater")
else:
    print("Both the numbers are equal")
```

Output:-
```text
Enter the both the numbers with comma between them 12,1
12 is greater
```
```text
Enter the both the numbers with comma between them 12,12
Both the numbers are equal
```

---

## 3. Write a program to find the largest among three numbers.

Program 1:-
```python
num1,num2,num3=input("Enter any three the numbers with comma between them").split(",")
num1,num2,num3=int(num1),int(num2),int(num3)
if num1>num2:
    if num1>num3:
        print(f"{num1} is greatest")
    else:
        print(f"{num3} is greatest")
    
elif num2>num1:
    if num2>num3:
        print(f"{num2} is greatest")
    else:
        print(f"{num3} is greatest")
else:
    print(f"{num3} is greatest")
```

Program 2:-
```python
num1,num2,num3=input("Enter any three the numbers with comma between them").split(",")
num1,num2,num3=int(num1),int(num2),int(num3)

if (num1 > num2) and (num1 > num3):
    print(f"{num1} is greatest")
elif (num2 > num1) and (num2 > num3):
    print(f"{num2} is greatest")
else:
    print(f"{num3} is greatest")
```

Program 3:-
```python
num1,num2,num3=input("Enter any three the numbers with comma between them").split(",")
num1,num2,num3=int(num1),int(num2),int(num3)
temp=num1

if num2 > temp:
    temp = num2
if num3 > temp:
    temp = num3
print(f"{temp} is greatest")
```

Output:-
```text
Enter any three the numbers with comma between them 12,23,1
23 is greater
```

---

## 4. Write a program to assign grades based on marks:

## - 90–100: A

## - 75–89: B

## - 50–74: C

## - Below 50: Fail

Program 1:-
```python
marks = input("Enter the marks")
grade = ""
if int(marks) in range (1,101):
    if int(marks) >= 90:
        grade = "A"
    elif int(marks) >= 75:
        grade = "B"
    elif int(marks) >= 50:
        grade = "C"
    else:
        grade = "Fail"
    print(f"The grade is {grade}")
else:
    print("The marks should be between 1 to 100")
```

Program 2:-
```python
marks = int(input("Enter the marks"))
grade = ""
if marks not in range (1,101):
    print("The marks should be between 1 to 100")
else:
    if marks>=90 and marks<=100:
        grade = "A"
    elif marks>=75 and marks<= 89:
        grade = "B"
    elif marks>=50  and marks<=74:
        grade = "C"
    else:
        grade = "Fail"
    print(f"The grade is {grade}")
```

Program 3:-
```python
marks = input("Enter the marks")
grade = "Fail"
if int(marks) < 1 or int(marks) > 100:
    print("The marks should be between 1 to 100")
else:
    if 90 <= int(marks) <= 100:
        grade = "A"
    elif 75 <= int(marks) <= 89:
        grade = "B"
    elif 50 <= int(marks) <= 74:
        grade = "C"
    else:
        grade = "Fail"
    print(f"The grade is {grade}")
```

Program 4:-
```python
    marks = int(input("Enter the marks"))
    grade = "Fail"
    
    if marks in range (1,101):
        if marks in range(90,101):
            grade = "A"
        elif marks in range(75,90):
            grade = "B"
        elif marks in range(50,75):
            grade = "C"
        else:
            grade = "Fail"
        print(f"The grade is {grade}")
    else:
        print("The maximum marks a student can get is 100")
```

Output:-

```text
Enter the marks 10
The grade is Fail
```
```text
Enter the marks 99
The grade is A
```
```text
Enter the marks 89
The grade is Fail
```
```text
Enter the marks 10
The grade is B
```
```text
Enter the marks 79
The grade is C
```
```text
Enter the marks 120
The maximum marks a student can get is 100
```

---

## 5. Write a program to check whether a character is a vowel, consonant, or not an alphabet.

Program 1:-
```python
letter=input("Enter the character")

if letter.lower() == 'a' or letter.lower() == 'e' or letter.lower() == 'i' or letter.lower() == 'o' or letter.lower() == 'u':
    print(f"{letter} is a vowel")
elif letter.lower() == 'b' or letter.lower() == 'c' or letter.lower() == 'd' or letter.lower() == 'f' or letter.lower() == 'g' or letter.lower() == 'h' or letter.lower() == 'j' or letter.lower() == 'k' or letter.lower() == 'l' or letter.lower() == 'm' or letter.lower() == 'n' or letter.lower() == 'p' or letter.lower() == 'q' or letter.lower() == 'r' or letter.lower() == 's' or letter.lower() == 't' or letter.lower() == 'v' or letter.lower() == 'w' or letter.lower() == 'x' or letter.lower() == 'y' or letter.lower() == 'z':
    print(f"{letter} is a consonant")
else:
    print(f"{letter} is not an alphabet")
```

Program 2:-
```python
letter=input("Enter the character")
vowels = "aeiou"
consonants = "bcdfghjklmnpqrstvwxyz"

if letter.lower() in vowels:
    print(f"{letter} is a vowel")
elif letter.lower() in consonants:
    print(f"{letter} is a consonant")
else:
    print(f"{letter} is not an alphabet")
```

Output:-

```text
Enter the character Q
Q is a consonant
```
```text
Enter the character w
w is a consonant
```
```text
Enter the character #
# is not an alphabe
```
```text
Enter the character A
A is a vowel
```
```text
Enter the character i
i is a vowel
```

---

## 6. Write a program to calculate electricity bill based on units consumed:

## 0–100 units: ₹5/unit

## 101–200 units: ₹7/unit

## Above 200 units: ₹10/unit

Program 1:-
```python
units=int(input("Enter the number of units consumed"))
bill=0
if units>= 0 and units <=100:
    bill= 5*units
elif units>= 101 and units <=200:
    bill= 7*units
else:
    bill= 10*units
print(f"Total electricity bill is Rs.{bill}")
```
Program 2:-
```python
units=int(input("Enter the number of units consumed"))
bill=0
if units <=100:
    bill= 5*units
elif units <=200:
    bill= 7*units
else:
    bill= 10*units
print(f"Total electricity bill is Rs.{bill}")
```

Output:-
```text
Enter the number of units consumed 300
Total electricity bill is Rs.3000
```
```text
Enter the number of units consumed 90
Total electricity bill is Rs.450
```
```text
Enter the number of units consumed 120
Total electricity bill is Rs.840
```

---

## 7. Write a program to determine the day of the week based on a number (1–7).

```python
week_number = int(input("Enter the number"))
week=""
if week_number == 1:
    week="Sunday"
elif week_number == 2:
    week="Monday"
elif week_number == 3:
    week="Tuesday"
elif week_number == 4:
    week="Wednesday"
elif week_number == 5:
    week="Thursday"
elif week_number == 6:
    week="Friday"
else:
    week="Saturday"
print(f"{week}")
```
Output:-
```text
Enter the number 4
Wednesday
```

---

## 8. Write a program to check if a year is a leap year using full logic (divisible by 4, 100, and 400 rules).

```python
year = int(input("Enter the year"))
leap_year = False
if year % 4 == 0 and year % 100 != 0:
    leap_year = True
elif year % 100 == 0 and year % 400 == 0:
    leap_year = True
else:
    leap_year = False

if leap_year:
    print("It is leap Year")
else:
    print("It is not leap year")
```
Output:-
```text
Enter the year 2022
It is not leap year
```
```text
Enter the year 1900
It is not leap year
```
```text
Enter the year 2000
It is leap Year
```
```text
Enter the year 2024
It is leap Year
```

---

## 9. Write a program to determine whether a number is one-digit, two-digit, or three-digit.

```python
number = input("Enter the number")
digit=0
if len(number)<=3:
    if len(number) == 3:
        if number.startswith("00"):
            digit=1
        elif number.startswith("0"):
            digit=2
        else:
            digit=3
    elif len(number) == 2:
        if number.startswith("0"):
            digit=1
        else:
            digit=2
    else:
        digit=1
    print(f"It is {digit}-digit number")
else:
    print("It is more than 3 digit number")
```

Output:-
```text
Enter the number 122
It is 3-digit number
```
```text
Enter the number 122
It is 3-digit number
```
```text
Enter the number 12
It is 2-digit number
```
```text
Enter the number 1
It is 1-digit number
```
```text
Enter the number 001
It is 1-digit number
```
```text
Enter the number 022
It is 2-digit number
```

---

## 10. Write a program to categorize a person based on age:

## Child (<13)

## Teen (13–19)

## Adult (20–59)

## Senior (60+)

```python
age = int(input("Enter the age"))
person=""
if age < 13:
    person = "child"
elif age <= 19:
    person = "Teen"
elif age <= 59:
    person = "Adult"
else:
    person = "Senior"
print(f"The person is {person}")
```

Output:-
```text
Enter the age 8
The person is child
```
```text
Enter the age 18
The person is Teen
```
```text
Enter the age 48
The person is Adult
```
```text
Enter the age 80
The person is Senior
```

---

## 11. Write a program to check if a number is divisible by both 2 and 3.
```python
number = int(input("Enter the number"))
if number % 2 == 0 and number % 3 == 0:
    print(f"The number {number} is divisible by both 2 and 3")
else:
    print(f"The number {number} is not divisible by both 2 and 3")
```

Output:-
```text
Enter the number 12
The number 12 is divisible by both 2 and 3
```
```text
Enter the number 11
The number 11 is not divisible by both 2 and 3
```

---

## 12 Write a program to check if a number lies between 50 and 100.

Program 1:-
```python
number = int(input("Enter the number"))

if number > 50 and number < 100:
    print(f"The {number} lies between 50 and 100")
else:
    print(f"The {number} does not lie between 50 and 100")
```

Program 2:-
```python
number = int(input("Enter the number"))

if number in range(51,101):
    print(f"The {number} lies between 50 and 100")
else:
    print(f"The {number} does not lie between 50 and 100")
```

Program 3:-
```python
number = int(input("Enter the number"))

if 50 < number < 100 :
    print(f"The {number} lies between 50 and 100")
else:
    print(f"The {number} does not lie between 50 and 100")
```

Output:-
```text
Enter the number 78
The 78 lies between 50 and 100
```
```text
Enter the number 1
The 1 does not lie between 50 and 100
```

---

## 13. Write a program to check if a triangle is valid (sum of angles = 180).
```python
a,b,c=input("Enter the angles of the triangle").split(",")

if int(a)+int(b)+int(c) == 180:
    print("The triangle is valid")
else:
    print("The triangle is invalid")

```

Output:-
```text
Enter the angles of the triangle 90,90,10
The triangle is invalid
```
```text
Enter the angles of the triangle 90,45,45
The triangle is valid
```

---

## 14. Write a program to determine the type of triangle based on sides (equilateral, isosceles, scalene).

```python
a,b,c=input("Enter the sides of the triangle").split(",")
if a==b==c:
    print("The triangle is equilateral")
elif (a==b) or (b==c) or (a==c):
    print("The triangle is isosceles")
else:
    print("The triangle is scalene")
```

Output:-
```text
Enter the sides of the triangle 2,2,3
The triangle is isosceles
```
```text
Enter the sides of the triangle 2,2,2
The triangle is equilateral
```
```text
Enter the sides of the triangle 1,2,3
The triangle is scalene
```

---

## 15. Write a program to calculate discount based on purchase amount:

## -Above ₹5000 → 20%

## - Above ₹2000 → 10%

## - Otherwise → No discount

```python
amount=float(input("Enter the purchase amount"))
total=0
if amount > 5000:
    total = amount - (amount * 0.20)
elif amount > 2000:
    total = amount - (amount * 0.10)
else:
    total = amount
print(f"You have to pay a total of Rs.{total}")
```

Output:-
```text
Enter the purchase amount 5050.25
You have to pay a total of Rs.4040.2
```
```text
Enter the purchase amount 2010
You have to pay a total of Rs.1809.0
```
```text
Enter the purchase amount 1000
You have to pay a total of Rs.1000.0
```

---

## 16. Write a program to determine whether a number is a three-digit palindrome.

```python
number = input("Enter the number")

if len(number) == 3:
    if int(number) // 100 == int(number) % 10:
        print("The number is palindrome")
    else:
        print("The number is not palindrome")
else:
    print("Please enter 3 digit number")
```

Output:-
```text
Enter the number 555
The number is palindrome
```
```text
Enter the number 515
The number is palindrome
```
```text
Enter the number 215
The number is not palindrome
```
