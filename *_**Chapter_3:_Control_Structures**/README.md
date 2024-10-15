<p><strong>Chapter 3: Control Structures</strong></p>

<p>Control structures are the backbone of any programming language, allowing developers to control the flow of their code and make decisions based on specific conditions. In this chapter, we will delve into the world of control structures, exploring the different types, their syntax, and how to use them effectively in your code.</p>

<p><strong>3.1 Conditional Statements</strong></p>

<p>Conditional statements are used to execute a block of code based on a specific condition. The most common type of conditional statement is the if-else statement.</p>

<h4>3.1.1 If-Else Statements</h4>

<p>An if-else statement consists of three parts: the condition, the if block, and the else block. The condition is evaluated, and if it is true, the code in the if block is executed. If the condition is false, the code in the else block is executed.</p>

<p><code>python
x = 5
if x &gt; 10:
    print("x is greater than 10")
else:
    print("x is less than or equal to 10")
</code></p>

<p>In this example, the condition <code>x &gt; 10</code> is evaluated, and since it is false, the code in the else block is executed, printing "x is less than or equal to 10" to the console.</p>

<h4>3.1.2 If-Elif-Else Statements</h4>

<p>If-elif-else statements are used when there are multiple conditions to be evaluated. The elif block is executed if the initial condition is false and the elif condition is true.</p>

<p><code>python
x = 5
if x &gt; 10:
    print("x is greater than 10")
elif x == 5:
    print("x is equal to 5")
else:
    print("x is less than 5")
</code></p>

<p>In this example, the condition <code>x &gt; 10</code> is evaluated, and since it is false, the elif condition <code>x == 5</code> is evaluated. Since this condition is true, the code in the elif block is executed, printing "x is equal to 5" to the console.</p>

<h4>3.1.3 Nested If-Else Statements</h4>

<p>Nested if-else statements are used when there are multiple conditions to be evaluated within an if or else block.</p>

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

<p>In this example, the condition <code>x &gt; 5</code> is evaluated, and since it is false, the code in the else block is executed. However, within the else block, there is another if-else statement that evaluates the condition <code>y &gt; 10</code>. Since this condition is true, the code in the if block is executed, printing "x is less than or equal to 5" to the console.</p>

<p><strong>3.2 Loops</strong></p>

<p>Loops are used to execute a block of code repeatedly based on a specific condition. There are two types of loops: for loops and while loops.</p>

<h4>3.2.1 For Loops</h4>

<p>For loops are used to iterate over a sequence of values, such as a list or a string.</p>

<p><code>python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
</code></p>

<p>In this example, the for loop iterates over the list of fruits, printing each fruit to the console.</p>

<h4>3.2.2 While Loops</h4>

<p>While loops are used to execute a block of code as long as a specific condition is true.</p>

<p><code>python
x = 0
while x &lt; 5:
    print(x)
    x += 1
</code></p>

<p>In this example, the while loop executes the code block as long as the condition <code>x &lt; 5</code> is true. The variable <code>x</code> is incremented by 1 in each iteration, and the loop continues until <code>x</code> is no longer less than 5.</p>

<p><strong>3.3 Break and Continue Statements</strong></p>

<p>Break and continue statements are used to control the flow of loops.</p>

<h4>3.3.1 Break Statements</h4>

<p>Break statements are used to exit a loop prematurely.</p>

<p><code>python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    if fruit == "banana":
        break
    print(fruit)
</code></p>

<p>In this example, the for loop iterates over the list of fruits, but when it encounters the fruit "banana", the break statement is executed, and the loop exits prematurely.</p>

<h4>3.3.2 Continue Statements</h4>

<p>Continue statements are used to skip the current iteration of a loop and move on to the next iteration.</p>

<p><code>python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    if fruit == "banana":
        continue
    print(fruit)
</code></p>

<p>In this example, the for loop iterates over the list of fruits, but when it encounters the fruit "banana", the continue statement is executed, and the loop skips the current iteration and moves on to the next iteration.</p>

<p><strong>3.4 Conclusion</strong></p>

<p>Control structures are a fundamental part of programming, allowing developers to control the flow of their code and make decisions based on specific conditions. In this chapter, we explored the different types of control structures, including conditional statements, loops, and break and continue statements. By mastering these concepts, developers can write more efficient and effective code.</p>

<p><strong>Exercise</strong></p>

<ol>
<li>Write a program that uses an if-else statement to determine whether a number is even or odd.</li>
<li>Write a program that uses a for loop to iterate over a list of numbers and print their squares.</li>
<li>Write a program that uses a while loop to simulate a coin toss, where the loop continues until the user decides to stop.</li>
</ol>

<p><strong>Solution</strong></p>

<ol>
<li><p><code>python
x = int(input("Enter a number: "))
if x % 2 == 0:
print("The number is even")
else:
print("The number is odd")
</code></p></li>
<li><p><code>python
numbers = [1, 2, 3, 4, 5]
for number in numbers:
print(number ** 2)
</code></p></li>
<li><p><code>python
import random
while True:
coin_toss = random.randint(0, 1)
if coin_toss == 0:
    print("Heads")
else:
    print("Tails")
response = input("Do you want to continue? (yes/no): ")
if response.lower() != "yes":
    break
</code></p></li>
</ol>
