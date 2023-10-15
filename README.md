# Loops in Python Workshop 

## Duration:
Approximately 60 minutes.

## Objectives:
- Understand the concept behind the use of loops in computer programming.
- Distinguish the differences between for loops and while loops.
- Practice applying loops into Python-based coding exercises and projects.
- Recognize loop errors/bugs and apply debugging techniques to fix them.

## Materials (Needed For Teacher & Students):
- Access to computer & WiFi.
- Github Account.
- Replit Account OR an IDE with Python installed.
- **IF REMOTE, Zoom or Google Meet account.**

## Prerequisites: 
- Should have a solid foundation in the following topics in Python: Variables, Data Types (ex: ints & strings), Conditional Logic (with boolean/logical operators) & Lists.
- Should have a some knowledge on some built-in Python functions and/or modules (ex: random, math & input).
- **IF USING IDE, should know the basics of Git when accessing and modifying files in the coding exercises (ex: commiting, forking, push/pull requests).**

## Grade Level:
Recommended for high schoolers (9th-12th) with some basic knowledge on Python.


# Introduction To Loops:
- We'll start with some real life applications of loops to get the students comfortable with the idea behind them.
- Discuss with the class an example of a morning routine (ask the class the first couple of things they do in the morning)
- This exercise is to prove that when you have a morning routine, it is vital it remains constant and turns into a pattern everyday.

- Display the class real life exmaples of a loop includes:
  - International Space Station that continuously orbits the Earth.
      - Example of the ISS constantly moving: http://api.open-notify.org/iss-now.json?callback=CALLBACK
      - Example from NASA website: https://spotthestation.nasa.gov/

## Examples of Loops in Coding:
- Explain the two pictures and the psuedo code that accompany with each one:
  - Flappy Bird Example:
  - IKEA Website Example:
 

# Lesson Outline:
- Start to explain that there are 2 ways of looping in Python
- Quick gif of Bart Simpson writing on the board over and over again
- Explain how long it would take to write a sepcific statement 1000 times, would be very diffifcult to do manually
- The solution to that is to write out for loop
- Figure of code of print("hello world") vs a loop which takes less time and is more efficient
- Explain to the class which solution looks easier to write out in terms of how concise and minimal it is, and can save a lot of time for coders

!(https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExczZzYXRpZnYzbmVqc3p3ZjF6bHA4bjE0Y3ZkeGdqc2g3Zm0xMGdzZyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/l2JdUB3sRLn5HmSY0/giphy.gif)

## For Loops
- First type of loop to explain are for loops
- we will know in advance how many times the loop will need to iterate because we will be working on a collection

- Syntax:
`for <temporary variable> in <collection>:
  <action>`

Let’s break down each of these components:

A for keyword indicates the start of a for loop.
A <temporary variable> that is used to represent the value of the element in the collection the loop is currently on.
An in keyword separates the temporary variable from the collection used for iteration.
A <collection> to loop over. In our examples, we will be using a list.
An <action> to do anything on each iteration of the loop.

Example: explain the comparisons between this example and this one
```
sport_games = ["football", "hockey", "baseball", "cricket"]
for game1 in sport_games:
  print(game1)
```

What will be printed out here? 
```
Word = “hello”
For i in word:
	print(i)
```

What type of collection are we using? *String*




        

