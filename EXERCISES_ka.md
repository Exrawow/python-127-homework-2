# სავარჯიშოები

შექმენით ეს ფაილები თქვენს საკუთარ საქაღალდეში:
`submissions/<თქვენი-github-username>/`.

## exercise_1.py — ჩემს შესახებ, input-იდან

`input()`-ის გამოყენებით გამოითხოვეთ მომხმარებლისგან სახელი, ასაკი და
ქალაქი, შემდეგ დაბეჭდეთ წინადადება f-string-ის გამოყენებით. ასაკი
გადაიყვანეთ `int`-ში და დაბეჭდეთ, რამდენი წლის გახდება 5 წელიწადში.

მაგალითი გაშვებისას:
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

## exercise_2.py — შეასწორეთ შეცდომა

ეს კოდი აგდებს `TypeError`-ს. დააკოპირეთ `exercise_2.py`-ში და
შეასწორეთ ტიპის გადაყვანის (casting) გამოყენებით, რომ იმუშაოს
შეცდომის გარეშე.

```python
age = input("How old are you?\n")
print("Next year you will be " + (age + 1))  # ბაგი: გამოასწორეთ ეს ხაზი
```

მოსალოდნელი შედეგი (input-ისთვის `25`):
```
How old are you?
25
Next year you will be 26
```

## exercise_3.py — გაასუფთავეთ input

გამოითხოვეთ მომხმარებლის სრული სახელი `input()`-ით. გაითვალისწინეთ,
რომ შესაძლოა ჩაწეროს ზედმეტი space-ები ან არასწორი ასოები, მაგ.
`"  ada LOVELACE  "`. გაასუფთავეთ `.strip()`-ით და `.title()`-ით,
შემდეგ დაბეჭდეთ გასუფთავებული სახელი და მისი სიგრძე `len()`-ით.

მაგალითი გაშვებისას (input არის `"  ada LOVELACE  "`):
```
Enter your full name:
  ada LOVELACE  
Cleaned name: Ada Lovelace
Length: 12
```

## exercise_4.py — Truthy თუ falsy

თხოვეთ მომხმარებელს დაბეჭდოს რამე (შესაძლოა უბრალოდ დააჭიროს
Enter-ს, არაფრის ჩაწერის გარეშე). დაბეჭდეთ, არის თუ არა `bool(...)`
მისი ჩანაწერის `True` თუ `False`. შემდეგ, ცალკე, დაბეჭდეთ `bool("0")`
და კომენტარში ახსენეთ, რატომ არ არის ის `False`.

მაგალითი გაშვებისას (მომხმარებელი უბრალოდ აჭერს Enter-ს):
```
Type something (or press Enter for nothing):

bool of your input: False
bool("0"): True
```

## exercise_5.py — ბონუსი: ფასი დღგ-ით

თხოვეთ მომხმარებელს ფასი `input()`-ით, გადაიყვანეთ `float`-ში.
`VAT_RATE = 0.18` კონსტანტის გამოყენებით, გამოთვალეთ ფასი დღგ-ის
ჩათვლით და დაბეჭდეთ 2 ათწილადის სიზუსტით `round(...)`-ის
გამოყენებით.

მაგალითი გაშვებისას (input არის `100`):
```
Enter a price:
100
Total with VAT: 118.0
```
