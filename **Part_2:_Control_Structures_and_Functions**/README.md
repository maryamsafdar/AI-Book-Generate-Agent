<p><strong>Chapter 5: Control Structures and Functions</strong></p>

<p><strong>5.1 Introduction</strong></p>

<p>In the previous chapters, we have learned the basics of programming, including variables, data types, and operators. However, to write more complex and efficient programs, we need to learn about control structures and functions. Control structures allow us to control the flow of our program's execution, while functions enable us to reuse code and organize our programs in a more modular way. In this chapter, we will explore the different types of control structures and functions in programming.</p>

<p><strong>5.2 Conditional Statements</strong></p>

<p>Conditional statements are used to execute different blocks of code based on certain conditions. The most common type of conditional statement is the if-else statement.</p>

<h4>If-Else Statement</h4>

<p>The if-else statement is used to execute a block of code if a certain condition is true. If the condition is false, the code in the else block is executed.</p>

<p><code>python
x = 5
if x &gt; 10:
    print("x is greater than 10")
else:
    print("x is less than or equal to 10")
</code></p>

<p>In this example, the condition <code>x &gt; 10</code> is false, so the code in the else block is executed.</p>

<h4>If-Elif-Else Statement</h4>

<p>The if-elif-else statement is used to check multiple conditions and execute different blocks of code based on those conditions.</p>

<p><code>python
x = 5
if x &gt; 10:
    print("x is greater than 10")
elif x == 5:
    print("x is equal to 5")
else:
    print("x is less than 5")
</code></p>

<p>In this example, the condition <code>x &gt; 10</code> is false, but the condition <code>x == 5</code> is true, so the code in the elif block is executed.</p>

<h4>Nested If-Else Statements</h4>

<p>Nested if-else statements are used to check multiple conditions and execute different blocks of code based on those conditions.</p>

<p><code>python
x = 5
y = 10
if x &gt; 5:
    if y &gt; 10:
        print("x is greater than 5 and y is greater than 10")
    else:
        print("x is greater than 5 but y is less than or equal to 10")
else:
    print("x is less than or equal to 5")
</code></p>

<p>In this example, the condition <code>x &gt; 5</code> is false, so the code in the else block is executed.</p>

<p><strong>5.3 Loops</strong></p>

<p>Loops are used to execute a block of code repeatedly for a specified number of times. There are two types of loops: for loops and while loops.</p>

<h4>For Loops</h4>

<p>For loops are used to execute a block of code for a specified number of times.</p>

<p><code>python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
</code></p>

<p>In this example, the code in the for loop is executed three times, once for each fruit in the list.</p>

<h4>While Loops</h4>

<p>While loops are used to execute a block of code as long as a certain condition is true.</p>

<p><code>python
x = 0
while x &lt; 5:
    print(x)
    x += 1
</code></p>

<p>In this example, the code in the while loop is executed five times, until the condition <code>x &lt; 5</code> is false.</p>

<p><strong>5.4 Functions</strong></p>

<p>Functions are used to reuse code and organize our programs in a more modular way. A function is a block of code that can be called multiple times from different parts of our program.</p>

<h4>Defining a Function</h4>

<p>A function is defined using the <code>def</code> keyword followed by the name of the function and a list of parameters in parentheses.</p>

<p><code>python
def greet(name):
    print("Hello, " + name + "!")
</code></p>

<p>In this example, the function <code>greet</code> takes one parameter <code>name</code> and prints a greeting message.</p>

<h4>Calling a Function</h4>

<p>A function is called by using the name of the function followed by a list of arguments in parentheses.</p>

<p><code>python
greet("John")
</code></p>

<p>In this example, the function <code>greet</code> is called with the argument <code>"John"</code>, and the greeting message is printed.</p>

<h4>Function Arguments</h4>

<p>Functions can take multiple arguments, and arguments can have default values.</p>

<p><code>python
def greet(name, age=30):
    print("Hello, " + name + "! You are " + str(age) + " years old.")
</code></p>

<p>In this example, the function <code>greet</code> takes two arguments <code>name</code> and <code>age</code>, and the argument <code>age</code> has a default value of 30.</p>

<h4>Return Values</h4>

<p>Functions can return values using the <code>return</code> statement.</p>

<p><code>python
def add(x, y):
    return x + y
</code></p>

<p>In this example, the function <code>add</code> takes two arguments <code>x</code> and <code>y</code> and returns their sum.</p>

<p><strong>5.5 Conclusion</strong></p>

<p>In this chapter, we have learned about control structures and functions in programming. We have seen how to use conditional statements, loops, and functions to write more complex and efficient programs. We have also learned how to define and call functions, and how to use function arguments and return values. In the next chapter, we will learn about data structures and file input/output.</p>
