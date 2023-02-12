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
There are some key components we can note from this function:

The def keyword indicates the beginning of a function. The function is followed by a name that the programmer defines (and is a function parameter). In our example, it's sayHello.
Following the function name is a pair of parenthesis () that holds input values, data that we can pass into the function. In our example, it's a name.
A colon : marks the end of the function header.

In the function, notice the indentation. Similar to if statements, anything after the colons that is indented is considered part of the function.

A function can also return a result, see the code block below:
<pre>
  def calcCost(item):
     if(item == "sweets"):
          return 3.99
     elif (item == "oranges"):
          return 1.99
     else:
          return 0.99

spent = 10
spent = spent + calcCost("sweets")
print("You have spent:" + str(spent))
</pre>
</pre>
<br>

![image](https://user-images.githubusercontent.com/105601437/218307292-3f5db291-0eee-4204-b360-710f9483a8cb.png)

--------------------------------------

<h3>Files</h3>
<pre>
it's common to write a script and import or export it from a file; whether that be as a way to store the output of your script or to import a list of 100's of websites from a file to enumerate.

f = open("file_name", "r")
print(f.read())

To open the file, we use the built-in open() function, and the "r" parameter stands for "read" and is used as we're reading the contents of the file. The variable has a read() method for reading the contents of the file. You can also use the readlines() method and loop over each line in the file; useful if you have a list where each item is on a new line. In the example above, the file is in the same folder as the Python script; if it were elsewhere, you would need to specify the full path of the file.

You can also create and write files. If you're writing to an existing file, you open the file first and use the "a" in the open function after the filename call (which stands for append). If you're writing to a new file, you use "w" (write) instead of "a". See the examples below for clarity:

f = open("demofile1.txt", "a") # Append to an existing file
f.write("The file will include more text..")
f.close()

f = open("demofile2.txt", "w") # Creating and writing to a new file
f.write("demofile2 file created, with this content in!")
f.close()

Notice we use the close() method after writing to a file; this closes the file so no more writing to the file (within the program) can occur.
</pre>

--------------------------------

Imports
<pre>
In Python, we can import libraries, which are a collection of files that contain functions. Think of importing a library as importing functions you can use that have been already written for you. For example, there is a "date" library that gives you access to hundreds of different functions for anything date and time-related.

import datetime
current_time = datetime.datetime.now()
print(current_time)

We import other libraries using the import keyword. Then in Python, we use that import's library name to reference its functions. In the example above, we import datetime, then access the .now() method by calling library_name.method_name(). Copy and paste the example above into the code editor.

Here are some popular libraries you may find useful in scripting as a pentester:

Request - simple HTTP library.
Scapy - send, sniff, dissect and forge network packets -https://scapy.readthedocs.io/en/latest/introduction.html
Pwntools - a CTF & exploit development library. - https://docs.pwntools.com/en/stable/

Many of these libraries are already built into the programming language; however, libraries written by other programmers not already installed in your machine can be installed using an application called pip, which is Python's package manager. Let's say you want to install the "scapy" library (which allows you to craft your own packets in code and send them to other machines); you install it first by running the command | pip install scapy |, after which in your program you can now import the scapy library.

</pre>
