<p><strong>Chapter 7.4: Hands-on Exercise - Dictionaries and Sets</strong></p>

<p><strong>Introduction</strong></p>

<p>In this chapter, we will delve into the world of dictionaries and sets in Python. These data structures are essential in any programming language, and Python provides an efficient way to work with them. We will explore the basics of dictionaries and sets, and then move on to some hands-on exercises to reinforce our understanding.</p>

<p><strong>Dictionaries</strong></p>

<p>A dictionary in Python is an unordered collection of key-value pairs. It is a mutable data type, which means it can be modified after creation. Dictionaries are defined using curly brackets <code>{}</code> and consist of keys and values. The keys are unique and immutable, while the values can be of any data type.</p>

<p>Here is an example of a dictionary:
<code>python
person = {
    "name": "John",
    "age": 30,
    "city": "New York"
}
</code>
In this example, <code>"name"</code>, <code>"age"</code>, and <code>"city"</code> are the keys, and <code>"John"</code>, <code>30</code>, and <code>"New York"</code> are the corresponding values.</p>

<p><strong>Sets</strong></p>

<p>A set in Python is an unordered collection of unique elements. It is a mutable data type, which means it can be modified after creation. Sets are defined using the <code>set()</code> function or by using the <code>{}</code> syntax with no keys.</p>

<p>Here is an example of a set:
<code>python
fruits = {"apple", "banana", "orange"}
</code>
In this example, <code>"apple"</code>, <code>"banana"</code>, and <code>"orange"</code> are the elements of the set.</p>

<p><strong>Hands-on Exercise</strong></p>

<p>Now that we have covered the basics of dictionaries and sets, let's move on to some hands-on exercises.</p>

<p><strong>Exercise 1: Creating a Dictionary</strong></p>

<p>Create a dictionary called <code>student</code> with the following key-value pairs:</p>

<ul>
<li><code>"name"</code>: <code>"Jane"</code></li>
<li><code>"age"</code>: <code>25</code></li>
<li><code>"major"</code>: <code>"Computer Science"</code></li>
</ul>

<p>Print the dictionary to the console.</p>

<p><strong>Solution</strong>
```python
student = {
    "name": "Jane",
    "age": 25,
    "major": "Computer Science"
}</p>

<p>print(student)
```
<strong>Exercise 2: Accessing Dictionary Values</strong></p>

<p>Using the <code>student</code> dictionary from Exercise 1, access the value of the <code>"name"</code> key and print it to the console.</p>

<p><strong>Solution</strong>
<code>python
print(student["name"])
</code>
<strong>Exercise 3: Modifying Dictionary Values</strong></p>

<p>Using the <code>student</code> dictionary from Exercise 1, modify the value of the <code>"age"</code> key to <code>26</code>. Print the updated dictionary to the console.</p>

<p><strong>Solution</strong>
<code>python
student["age"] = 26
print(student)
</code>
<strong>Exercise 4: Creating a Set</strong></p>

<p>Create a set called <code>colors</code> with the following elements:</p>

<ul>
<li><code>"red"</code></li>
<li><code>"green"</code></li>
<li><code>"blue"</code></li>
</ul>

<p>Print the set to the console.</p>

<p><strong>Solution</strong>
<code>python
colors = {"red", "green", "blue"}
print(colors)
</code>
<strong>Exercise 5: Adding Elements to a Set</strong></p>

<p>Using the <code>colors</code> set from Exercise 4, add the element <code>"yellow"</code> to the set. Print the updated set to the console.</p>

<p><strong>Solution</strong>
<code>python
colors.add("yellow")
print(colors)
</code>
<strong>Exercise 6: Removing Elements from a Set</strong></p>

<p>Using the <code>colors</code> set from Exercise 5, remove the element <code>"green"</code> from the set. Print the updated set to the console.</p>

<p><strong>Solution</strong>
<code>python
colors.remove("green")
print(colors)
</code>
<strong>Conclusion</strong></p>

<p>In this chapter, we have covered the basics of dictionaries and sets in Python. We have also completed several hands-on exercises to reinforce our understanding of these data structures. With practice and experience, you will become proficient in working with dictionaries and sets in Python.</p>

<p><strong>Additional Practice</strong></p>

<p>Here are some additional practice exercises to help you reinforce your understanding of dictionaries and sets:</p>

<ul>
<li>Create a dictionary with the following key-value pairs: <code>"name"</code>: <code>"John"</code>, <code>"age"</code>: <code>30</code>, <code>"city"</code>: <code>"New York"</code>. Access the value of the <code>"name"</code> key and print it to the console.</li>
<li>Create a set with the following elements: <code>"apple"</code>, <code>"banana"</code>, <code>"orange"</code>. Add the element <code>"grape"</code> to the set and print the updated set to the console.</li>
<li>Create a dictionary with the following key-value pairs: <code>"name"</code>: <code>"Jane"</code>, <code>"age"</code>: <code>25</code>, <code>"major"</code>: <code>"Computer Science"</code>. Modify the value of the <code>"age"</code> key to <code>26</code> and print the updated dictionary to the console.</li>
</ul>

<p>By completing these exercises, you will gain a deeper understanding of dictionaries and sets in Python and be able to apply this knowledge to real-world problems.</p>
