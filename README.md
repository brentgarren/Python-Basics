# Python-Basics and yes we going really basic

-### This is an example of print() Which output a line of code<br>
-### Text preceded with a # are comments and are ignored when running scripts<br>
Comments are written by the programmer in this case Me to allow future programmers YOU to understand what the script is supposed to do<br>

print("Hello World")<br>

Anything within the ( ) would be outputed in this case Hello World<br>
when printing a string ( ) we need to include the " "

--------------------------------------

# Mathematical Operators
<pre>
OPERATOR | SYMBOL | EXAMPLE <br>

ADDITION       |  +  | 1 + 1 = 2 <br>
SUBTRACTION    |  -  | 5 - 1 = 4 <br>
MULTIPLICATION |  *  | 10 * 10 = 100 <br>
DIVISION       |  /  | 10 / 2 = 5 <br>
MODULUS        |  %  | 10 % 2 = 0 <br>
EXPONENTIAL    |  ** | 5**2  = 25 (52) <br>

Greater Than   | >   | 
Less Than      | <   |
Equal to       | ==  |
Not Equal to   | !=  |
Greater than or equal to  | >= |
Less than or equal | <= |
</pre><br>

--------------------------------------

# Variables

Variables allow you to store and update data in a computer program. You have a variable name and store data to that name.<br>
<pre>Example: 
  | Fruit = Apple |
  | Leaves = 15 |
</pre>

In the example above, we have 2 variables. The variable name "fruit" stores the string (words) ice cream, while another variable called "leaves" stores a number (2000).

Variables are powerful as you can change them throughout your program. The following example sets the age variable to 30, then we increase this age variable by 1, making the final variable data 31.

<pre>
Age = 30
Age = age + 1
Print(age)
</pre>

<h3>Data Types</h3>
<pre>
String - Used for combinations of characters, such as letters or symbols
Integer - Whole Numbers
Float - Numbers that contain decimals or fractions
Boolean - Used for data that is restricted as either true or false
List - Series of different data types stored in a collection

</pre><br>
![image](https://user-images.githubusercontent.com/105601437/218305201-feee43b9-f392-4f49-a67a-72460c8aa7db.png)
<br>

# Boolen Operators
<pre>
Both conditions must be true for the statement to be true | AND |
Only one condition of the statement needs to be true | OR |
If a condition is the opposite of an argument	| NOT |
<br>
a = 1
if a == 1 or a > 10:
     print("a is either 1 or above 10")
     <br>
name = "bob" hungry = True
if name == "bob" and hungry == True:
     print("bob is hungry")
elif name == "bob" and not hungry:
     print("Bob is not hungry")
else: # If all other if conditions are not met
     print("Not sure who this is or if they are hungry") 
</pre>
<br>
# <h3>Loops</h3>

<pre>
There are 2 types of Loops - | For | and | while | 
<h4> While Loops</h4>
We can have the loop run indefinitely or (similar to an if statement) determine how many times the loop should run based on a condition.
  Example
  i = 1
while i <= 10:
     print(i)
     i = i + 1
<br>
This while loop will run 10 times, outputting the value of the i variable each time it iterates (loops). Let's break this down:

The i variable is set to 1
The while statement specifies where the start of the loop should begin
Every time it loops, it will start at the top (outputting the value of i)
Then it goes to the next line in the loop, which increases the value of i by 1
Then (as there is no more code for the program to execute), it goes to the top of the loop, starting the process over again
The program will keep on looping until the value of the i variable is greater than 10<br>

<h4> For Loops</h4>
A for loop is used to iterate over a sequence such as a list. Lists are used to store multiple items in a single variable, and are created using square brackets

websites = ["facebook.com", "google.com", "amazon.com"]
for site in websites:
     print(site)
     
This for loop shown in the code block above, will run 3 times, outputting each website in the list. Let's break this down:

The list variable called websites is storing 3 elements
The loop iterates through each element, printing out the element
The program stops looping when it's been through each element in the loop

In Python, we can also iterate through a range of numbers using the range function. Below is some example Python code that will print the numbers from 0 to 4. In programming, 0 is often the starting number, so counting to 5 is 0 to 4 (but has 5 numbers: 0, 1, 2, 3, and 4)

for i in range(5):
     print(i)
</pre><br>

-------------------------------------

<h1>Introduction to Funcations</h1>
<pre>
 A function is a block of code that can be called at different places in your program.

You could have a function to work out a calculation such as the distance between two points on a map or output formatted text based on certain conditions. Having functions removes repetitive code, as the function's purpose can be used multiple times throughout a program.
<br>
def sayHello(name):
     print("Hello " + name + "! Nice to meet you.")
sayHello("ben") # Output is: Hello Ben! Nice to meet you
<br>

</pre>
