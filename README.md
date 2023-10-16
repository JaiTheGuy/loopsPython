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
- Should have some knowledge on some built-in Python functions and/or modules (ex: random, math & input).
- **IF USING IDE, should know the basics of Git when accessing and modifying files in the coding exercises (ex: committing, forking, push/pull requests).**

## Grade Level:
Recommended for high schoolers (9th-12th) with some basic knowledge on Python.

## Note On Participation:
> [!NOTE]
> There will be some questions, examples, and coding exercises throughout the lesson plan. You can optimize the content of these interaction pieces based on your classroom. It's highly recommended to go over the content of the interaction pieces as they help progress to the final project of the lesson.
> 
> You will see an (important sign) next to these pieces to encourage student participation during lecture for questions, peer coding and/or independent work


# Introduction To The Concept of Loops:
- We'll start with some real life applications of loops to get the students comfortable with the idea behind them.
- Emphasize that a **loop** is an action that occurs over and over and over again.
> [!IMPORTANT]
> Discuss with the class an example of a morning routine (ask the class the first couple of things they do in the morning)
- This exercise is to prove that when you have a morning routine, it is vital it remains constant and turns into a pattern everyday.

- Display the class with a real life application of a loop (something that keeps running):
  - International Space Station that continuously orbits the Earth **([GIF](https://github.com/JaiTheGuy/loopsPython/blob/main/loopsPythonVisuals/International_Space_Station_pillars%20(1).gif)).**
      - Discuss with the class that the coordinates are always moving therefore the ISS has a job to orbit continuously.
      - [JSON file that tracks the longitude/latitude coordinates of the ISS](http://api.open-notify.org/iss-now.json?callback=CALLBACK)
      - [NASA website of spotting the ISS geographically](https://spotthestation.nasa.gov/)
> [!IMPORTANT]
> Ask the class for more real life applications that can relate to a loop, even if there's a stop to it eventually.
> 
> Examples can include a car running until it needs gas or a candle burning until the wick burns below the wax to help them out.

## Examples of Loops in Coding:
- Explain the two pictures and the pseudo code that accompany with each one and how loops are typically integrated in coding applications such as shopping websites, phone applications and video games:
  
[IKEA Website Example](https://github.com/JaiTheGuy/loopsPython/blob/main/loopsPythonVisuals/ikea.png)
- For the following IKEA example, we see that there are 3 chairs being displayed.
- With the help of loops, they can iterate through any type of search result and display the following format.
```
# pseudocode for IKEA chair picture

for every chair in IKEA website:
	display pic of chair
	show name of chair
	type of furniture
	display price or price on sale
	stars out of 5/# of ratings
```

[Flappy Bird Example:](https://github.com/JaiTheGuy/loopsPython/blob/main/loopsPythonVisuals/aim_bird.gif)

> [!IMPORTANT]
> Before you show off the pseudocode of the Flappy Bird GIF, ask the class what specific actions are being looped throughout the game
> If it helps, give them this example and ask them to fill in the blanks

```
while playing flappy bird:
	__________________
	__________________
	if the bird goes through a pipe:
		_________________
	else:
		_________________
```
### Solution:
```
while playing flappy bird:
	move background of trees/skyline
	show off a new pipe
	if the bird goes through a pipe:
        	update the score to 1+
	else:
		lose the game and start over
```


# For Loops:
- Start to explain that there are 2 ways of looping in Python, the first one we'll be learning are **for loops**.
- [A GIF of Bart Simpson writing "HAVE A GREAT SUMMER, EVERYONE" on the board over and over again](https://github.com/JaiTheGuy/loopsPython/blob/main/loopsPythonVisuals/giphy%20(1).gif)
- Show off a GIF and explain how long it would take to write that specific statement 10 times, 100 times or even a million times.
- Emphasize it would be would be very difficult to do manually and show off this example to show off this point with the following code:
  
```python
print("HAVE A GREAT SUMMER, EVERYONE")
print("HAVE A GREAT SUMMER, EVERYONE")
print("HAVE A GREAT SUMMER, EVERYONE")
print("HAVE A GREAT SUMMER, EVERYONE")

# ...after many more print statements..

print("HAVE A GREAT SUMMER, EVERYONE")
```
- The solution to that is to write out for loop knowing the amount of times we want to print this statement out
- If we wanted to print "HAVE A GREAT SUMMER" 5 times using a loop, we'll write out the following:

```python

for i in range(5):
  print("HAVE A GREAT SUMMER, EVERYONE")

```

- Explain to the class which solution looks easier to write out in terms of how concise and minimal it is which can save a lot of time for coders.

## Syntax & For Loop Examples:
- The major case when using for loops is that we will know in advance how many times the loop will need to iterate through a collection.
- When we talk about collections, we are referring to some sort of data that we can extract from (examples include elements in lists or characters in strings).
- Iteration is a repeated performance where it executes the same set of instructions a given number of times or until a specified result is obtained.

Syntax:
```
for <temp variable> in <collection>:
  <executable code>
```

Break down each component to the following use case and/or definition:

- _**for**_ keyword = indicates the start of a for loop.
- _**temp variable**_ (temporary variable) = used to track the value of the element in the collection the loop is currently on. The temporary variable can be any name you'd like it to be but it's always encouraged to make a temp variable that relates to what you're doing.
- _**in**_ keyword = separates the temp variable from the collection used for iteration.
- _**collection**_ = the content that we're looping over with a colon afterwards.
- _**executable code**_ = the action to perform on each iteration of the loop.

Example:
```python
speech = ["Spanish", "French", "Italian", "English"]

for languages in speech:
  print(languages)

# Output:

Spanish
French
Italian
English
```
> [!IMPORTANT]
> Ask the class the following questions: What type of collection are we using for this loop that will be printed out here? 

```python
for i in "hello":
  print(i)

#
#
#
#
#
#
#
#
#
#
#
#


# Solution:

# The collection we're using is a String that is going to print out individual characters

# Output from the loop:
h
e
l
l
o

```

## Loops in Ranges:
- The same way we want to perform an action a certain amount of times in loops, it becomes most helpful when it comes to numbers.
- When we're not dealing with collections, we can iterate over a range of integers that exist.

Example #1: 
- Let's say we want to print out a range of numbers from 0 through 5.
- We will be using a temporary variable inside of a range and using the parenthesis after it to control the amount of times.
- The reason why we use 6 instead 5 is because that number is exclusive from that endpoint.


```python
for i in range(6):
  print(i)

 # Output:
0
1
2
3
4
5
```

Example #2: 
- We want to start off from a different number instead of zero.
- In order to start off with a non-zero number, we'll need two numbers in the range (the min and max).
- Let's use an example where we go from 10 through 15.

```python
for j in range(10,16):
  print(j)

# Output:
10
11
12
13
14
15
```

Example #3:
- Now that we know how to print out values from the min and max, let's know print out a pattern from the range.
- This will know require 3 numbers in the range that goes like this: `for k in range(start, stop, step)`
- With the following syntax, let's print out mulitple of 5's between 50 through 75.

```python
for k in range(50, 76, 5):
  print(k)

# Output:
50
55
60
65
70
75
```
> [!IMPORTANT]
> Let students either use [Replit](https://replit.com/) and copy the following patterns and Invite you to their link or [Fork this file](https://replit.com/) from the repo and create a pull request with your name and classname.
> Let's try getting the class to print out the following numerical patterns using for loops:
>
> Be mindful that the patterns will displayed horizonally but the output must be printed veritcally with the commas represnted as a new line for the value.
> The 3 ellipses are filler to save space but the values must be printed out in between as well.

```python
# Pattern 1:
# 21, 25, 29, ... 97
########### CODE BELOW HERE #########




# Pattern 2:
# -4, -2, 0, ... 3
########### CODE BELOW HERE #########






# Pattern 3:
# 3 mississippi, 2 mississippi, 1 mississippi
########### CODE BELOW HERE #########







# Pattern 4:
# Create a list of 5 emojis of your choice and print them using a for loop
# 😬😎😁👽🥳
########### CODE BELOW HERE #########









```
