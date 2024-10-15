<p><strong>Chapter 2.3: Basic Operators and Expressions</strong></p>

<p>In the previous chapters, we discussed the basics of programming and variables. In this chapter, we will delve into the world of operators and expressions, which are essential components of any programming language. Operators are used to perform operations on variables and values, while expressions are combinations of operators, variables, and values that evaluate to a single value.</p>

<p><strong>2.3.1 Arithmetic Operators</strong></p>

<p>Arithmetic operators are used to perform mathematical operations on numbers. The following are the basic arithmetic operators:</p>

<ul>
<li><strong>Addition (+)</strong>: The addition operator is used to add two or more numbers. For example: <code>a = 5 + 3;</code></li>
<li><strong>Subtraction (-)</strong>: The subtraction operator is used to subtract one number from another. For example: <code>a = 5 - 3;</code></li>
<li><strong>Multiplication (*)</strong>: The multiplication operator is used to multiply two or more numbers. For example: <code>a = 5 * 3;</code></li>
<li><strong>Division (/)</strong>: The division operator is used to divide one number by another. For example: <code>a = 5 / 3;</code></li>
<li><strong>Modulus (%)</strong>: The modulus operator is used to find the remainder of a division operation. For example: <code>a = 5 % 3;</code></li>
</ul>

<p>Here's an example code snippet that demonstrates the use of arithmetic operators:</p>

<p>```c
int main() {
    int a = 5;
    int b = 3;
    int sum = a + b;
    int difference = a - b;
    int product = a * b;
    int quotient = a / b;
    int remainder = a % b;</p>

<pre><code>printf("Sum: %d\n", sum);
printf("Difference: %d\n", difference);
printf("Product: %d\n", product);
printf("Quotient: %d\n", quotient);
printf("Remainder: %d\n", remainder);

return 0;
</code></pre>

<p>}
```</p>

<p><strong>2.3.2 Assignment Operators</strong></p>

<p>Assignment operators are used to assign a value to a variable. The following are the basic assignment operators:</p>

<ul>
<li><strong>Assignment (=)</strong>: The assignment operator is used to assign a value to a variable. For example: <code>a = 5;</code></li>
<li><strong>Addition Assignment (+=)</strong>: The addition assignment operator is used to add a value to a variable and assign the result back to the variable. For example: <code>a += 5;</code></li>
<li><strong>Subtraction Assignment (-=)</strong>: The subtraction assignment operator is used to subtract a value from a variable and assign the result back to the variable. For example: <code>a -= 5;</code></li>
<li><strong>Multiplication Assignment (*=)</strong>: The multiplication assignment operator is used to multiply a value with a variable and assign the result back to the variable. For example: <code>a *= 5;</code></li>
<li><strong>Division Assignment (/=)</strong>: The division assignment operator is used to divide a variable by a value and assign the result back to the variable. For example: <code>a /= 5;</code></li>
<li><strong>Modulus Assignment (%=)</strong>: The modulus assignment operator is used to find the remainder of a division operation and assign the result back to the variable. For example: <code>a %= 5;</code></li>
</ul>

<p>Here's an example code snippet that demonstrates the use of assignment operators:</p>

<p>```c
int main() {
    int a = 5;</p>

<pre><code>a += 5;
printf("Addition Assignment: %d\n", a);

a -= 5;
printf("Subtraction Assignment: %d\n", a);

a *= 5;
printf("Multiplication Assignment: %d\n", a);

a /= 5;
printf("Division Assignment: %d\n", a);

a %= 5;
printf("Modulus Assignment: %d\n", a);

return 0;
</code></pre>

<p>}
```</p>

<p><strong>2.3.3 Comparison Operators</strong></p>

<p>Comparison operators are used to compare two values and return a boolean result. The following are the basic comparison operators:</p>

<ul>
<li><strong>Equal to (==)</strong>: The equal to operator is used to check if two values are equal. For example: <code>a == 5;</code></li>
<li><strong>Not Equal to (!=)</strong>: The not equal to operator is used to check if two values are not equal. For example: <code>a != 5;</code></li>
<li><strong>Greater than (&gt;)</strong>: The greater than operator is used to check if a value is greater than another value. For example: <code>a &gt; 5;</code></li>
<li><strong>Less than (&lt;)</strong>: The less than operator is used to check if a value is less than another value. For example: <code>a &lt; 5;</code></li>
<li><strong>Greater than or Equal to (&gt;=)</strong>: The greater than or equal to operator is used to check if a value is greater than or equal to another value. For example: <code>a &gt;= 5;</code></li>
<li><strong>Less than or Equal to (&lt;=)</strong>: The less than or equal to operator is used to check if a value is less than or equal to another value. For example: <code>a &lt;= 5;</code></li>
</ul>

<p>Here's an example code snippet that demonstrates the use of comparison operators:</p>

<p>```c
int main() {
    int a = 5;</p>

<pre><code>if (a == 5) {
    printf("Equal to\n");
}

if (a != 5) {
    printf("Not Equal to\n");
}

if (a &gt; 5) {
    printf("Greater than\n");
}

if (a &lt; 5) {
    printf("Less than\n");
}

if (a &gt;= 5) {
    printf("Greater than or Equal to\n");
}

if (a &lt;= 5) {
    printf("Less than or Equal to\n");
}

return 0;
</code></pre>

<p>}
```</p>

<p><strong>2.3.4 Logical Operators</strong></p>

<p>Logical operators are used to combine two or more conditions and return a boolean result. The following are the basic logical operators:</p>

<ul>
<li><strong>And (&amp;&amp;)</strong>: The and operator is used to check if two conditions are true. For example: <code>a &gt; 5 &amp;&amp; a &lt; 10;</code></li>
<li><strong>Or (||)</strong>: The or operator is used to check if at least one condition is true. For example: <code>a &gt; 5 || a &lt; 10;</code></li>
<li><strong>Not (!)</strong>: The not operator is used to negate a condition. For example: <code>!(a &gt; 5);</code></li>
</ul>

<p>Here's an example code snippet that demonstrates the use of logical operators:</p>

<p>```c
int main() {
    int a = 5;</p>

<pre><code>if (a &gt; 5 &amp;&amp; a &lt; 10) {
    printf("And\n");
}

if (a &gt; 5 || a &lt; 10) {
    printf("Or\n");
}

if (!(a &gt; 5)) {
    printf("Not\n");
}

return 0;
</code></pre>

<p>}
```</p>

<p><strong>Conclusion</strong></p>

<p>In this chapter, we discussed the basic operators and expressions in programming. We covered arithmetic operators, assignment operators, comparison operators, and logical operators. We also provided example code snippets to demonstrate the use of each operator. Understanding operators and expressions is essential for writing effective and efficient code. In the next chapter, we will discuss control structures, which are used to control the flow of a program.</p>
