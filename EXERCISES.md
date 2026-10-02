# Exercises

Create these files inside your own folder:
`submissions/<your-github-username>/`.

## exercise_1.py — About me, from input

Ask the user for their name, age, and city using `input()`, then print a
sentence about them using an f-string. Cast the age to `int` and print
what their age will be in 5 years.

Example run:
```
What is your name?
Ada
How old are you?
25
What city do you live in?
Tbilisi
My name is Ada, I am 25 years old, and I live in Tbilisi.
In 5 years I will be 30.
```

## exercise_2.py — Fix the bug

This code raises a `TypeError`. Copy it into `exercise_2.py`, then fix it
using type casting so it runs without error.

```python
age = input("How old are you?\n")
print("Next year you will be " + (age + 1))  # BUG: fix this line
```

Expected output (for an input of `25`):
```
How old are you?
25
Next year you will be 26
```

## exercise_3.py — Clean the input

Ask the user for their full name with `input()`. Assume they might type
extra spaces or the wrong case, e.g. `"  ada LOVELACE  "`. Clean it up
with `.strip()` and `.title()`, then print the cleaned name and its
length with `len()`.

Example run (input is `"  ada LOVELACE  "`):
```
Enter your full name:
  ada LOVELACE  
Cleaned name: Ada Lovelace
Length: 12
```

## exercise_4.py — Truthy or falsy

Ask the user to type something (they may just press Enter without typing
anything). Print whether `bool(...)` of what they typed is `True` or
`False`. Then, separately, print `bool("0")` and explain with a comment
why it is not `False`.

Example run (user just presses Enter):
```
Type something (or press Enter for nothing):

bool of your input: False
bool("0"): True
```

## exercise_5.py — Bonus: price with VAT

Ask the user to enter a price with `input()`, cast it to `float`. Using
a constant `VAT_RATE = 0.18`, compute the total price with VAT included
and print it rounded to 2 decimal places with `round(...)`.

Example run (input is `100`):
```
Enter a price:
100
Total with VAT: 118.0
```
