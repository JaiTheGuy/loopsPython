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

## Note On Particaption:
> [!NOTE]
> There will be some questions, examples, and coding exercises thorughout the lesson plan. You can optimize the content of these interaction pieces based on your classroom. It's highly recommended to go over the content of the interaction pieces as they help progress to the final project of the lesson.
> 
> You will see an (important sign) next to these pieces to encourage student particaption during lecture for questions, peer coding and/or independent work


# Introduction To Loops:
- We'll start with some real life applications of loops to get the students comfortable with the idea behind them.
- Emphasize that a **loop** is an action that occurs over and over and over again.
> [!IMPORTANT]
> Discuss with the class an example of a morning routine (ask the class the first couple of things they do in the morning)
- This exercise is to prove that when you have a morning routine, it is vital it remains constant and turns into a pattern everyday.

- Display the class with a real life application of a loop (something that keeps running):
  - International Space Station that continuously orbits the Earth **([GIF](https://github.com/JaiTheGuy/loopsPython/blob/main/loopsPythonVisuals/International_Space_Station_pillars%20(1).gif)).**
      - Discuss with the class that the cooridnates are always moving therefore the ISS has a job to orbit continuously.
      - [JSON file that tracks the longitude/latitude cooridates of the ISS](http://api.open-notify.org/iss-now.json?callback=CALLBACK)
      - [NASA website of spotting the ISS geographically](https://spotthestation.nasa.gov/)
> [!IMPORTANT]
> Ask the class for more real life applications that can relate to a loop, even if there's a stop to it eventually.
> 
> Examples can include a car running until it needs gas or a candle burning until the wick burns below the wax to help them out.

## Examples of Loops in Coding:
- Explain the two pictures and the psuedo code that accompany with each one and how loops are tpyically integrated in coding applcations such as shopping websites, phone applications and video games:
  
[IKEA Website Example](https://github.com/JaiTheGuy/loopsPython/blob/main/loopsPythonVisuals/ikea.png)
```
# pseudocode for IKEA chair picture

for every chair in IKEA website:
	display pic of chair
	show name of chair
	type of furniture
	display price or price on sale
	stars out of 5/# of ratings
```
 

# Lesson Outline:
- Start to explain that there are 2 ways of looping in Python
- Quick gif of Bart Simpson writing on the board over and over again
- Explain how long it would take to write a sepcific statement 1000 times, would be very diffifcult to do manually
- The solution to that is to write out for loop
- Figure of code of print("hello world") vs a loop which takes less time and is more efficient
- Explain to the class which solution looks easier to write out in terms of how concise and minimal it is, and can save a lot of time for coders

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




        

