<p><strong>Chapter 7.3: Dictionary and Set Operations</strong></p>

<p>In this chapter, we will delve into the world of dictionary and set operations in Python. Dictionaries and sets are two fundamental data structures in Python that allow you to store and manipulate data efficiently. We will explore the various operations that can be performed on dictionaries and sets, including creation, modification, and manipulation.</p>

<p><strong>7.3.1 Dictionary Operations</strong></p>

<p>A dictionary in Python is an unordered collection of key-value pairs. Dictionaries are mutable, meaning they can be modified after creation. Here are some common dictionary operations:</p>

<ul>
<li><p><strong>Creating a Dictionary</strong>: A dictionary can be created using the <code>dict()</code> constructor or by using the <code>{}</code> syntax.</p>

<p>```python</p>

<h1>Create a dictionary using the dict() constructor</h1></li>
</ul>

<p>my_dict = dict(name='John', age=30)</p>

<h1>Create a dictionary using the {} syntax</h1>

<p>my_dict = {'name': 'John', 'age': 30}
```</p>

<ul>
<li><p><strong>Accessing Dictionary Elements</strong>: Dictionary elements can be accessed using their corresponding keys.</p>

<p><code>python
my_dict = {'name': 'John', 'age': 30}
print(my_dict['name'])  # Output: John
</code></p></li>
<li><p><strong>Modifying Dictionary Elements</strong>: Dictionary elements can be modified by assigning a new value to an existing key.</p>

<p><code>python
my_dict = {'name': 'John', 'age': 30}
my_dict['age'] = 31
print(my_dict)  # Output: {'name': 'John', 'age': 31}
</code></p></li>
<li><p><strong>Adding New Dictionary Elements</strong>: New dictionary elements can be added by assigning a value to a new key.</p>

<p><code>python
my_dict = {'name': 'John', 'age': 30}
my_dict['city'] = 'New York'
print(my_dict)  # Output: {'name': 'John', 'age': 30, 'city': 'New York'}
</code></p></li>
<li><p><strong>Removing Dictionary Elements</strong>: Dictionary elements can be removed using the <code>del</code> statement or the <code>pop()</code> method.</p>

<p>```python
my<em>dict = {'name': 'John', 'age': 30}
del my</em>dict['age']
print(my_dict)  # Output: {'name': 'John'}</p></li>
</ul>

<p>my<em>dict = {'name': 'John', 'age': 30}
my</em>dict.pop('age')
print(my_dict)  # Output: {'name': 'John'}
```</p>

<p><strong>7.3.2 Set Operations</strong></p>

<p>A set in Python is an unordered collection of unique elements. Sets are mutable, meaning they can be modified after creation. Here are some common set operations:</p>

<ul>
<li><p><strong>Creating a Set</strong>: A set can be created using the <code>set()</code> constructor or by using the <code>{}</code> syntax.</p>

<p>```python</p>

<h1>Create a set using the set() constructor</h1></li>
</ul>

<p>my_set = set([1, 2, 3])</p>

<h1>Create a set using the {} syntax</h1>

<p>my_set = {1, 2, 3}
```</p>

<ul>
<li><p><strong>Adding Elements to a Set</strong>: Elements can be added to a set using the <code>add()</code> method.</p>

<p><code>python
my_set = {1, 2, 3}
my_set.add(4)
print(my_set)  # Output: {1, 2, 3, 4}
</code></p></li>
<li><p><strong>Removing Elements from a Set</strong>: Elements can be removed from a set using the <code>remove()</code> method or the <code>discard()</code> method.</p>

<p>```python
my<em>set = {1, 2, 3}
my</em>set.remove(2)
print(my_set)  # Output: {1, 3}</p></li>
</ul>

<p>my<em>set = {1, 2, 3}
my</em>set.discard(2)
print(my_set)  # Output: {1, 3}
```</p>

<ul>
<li><p><strong>Set Union</strong>: The union of two sets can be obtained using the <code>union()</code> method or the <code>|</code> operator.</p>

<p><code>python
my_set1 = {1, 2, 3}
my_set2 = {3, 4, 5}
print(my_set1.union(my_set2))  # Output: {1, 2, 3, 4, 5}
print(my_set1 | my_set2)  # Output: {1, 2, 3, 4, 5}
</code></p></li>
<li><p><strong>Set Intersection</strong>: The intersection of two sets can be obtained using the <code>intersection()</code> method or the <code>&amp;</code> operator.</p>

<p><code>python
my_set1 = {1, 2, 3}
my_set2 = {3, 4, 5}
print(my_set1.intersection(my_set2))  # Output: {3}
print(my_set1 &amp; my_set2)  # Output: {3}
</code></p></li>
<li><p><strong>Set Difference</strong>: The difference of two sets can be obtained using the <code>difference()</code> method or the <code>-</code> operator.</p>

<p><code>python
my_set1 = {1, 2, 3}
my_set2 = {3, 4, 5}
print(my_set1.difference(my_set2))  # Output: {1, 2}
print(my_set1 - my_set2)  # Output: {1, 2}
</code></p></li>
</ul>

<p><strong>7.3.3 Dictionary and Set Operations Example</strong></p>

<p>Here's an example that demonstrates the use of dictionary and set operations:</p>

<p>```python</p>

<h1>Create a dictionary of student information</h1>

<p>students = {
    'John': {'age': 20, 'courses': {'Math', 'Science'}},
    'Jane': {'age': 22, 'courses': {'Math', 'History'}},
    'Bob': {'age': 21, 'courses': {'Science', 'History'}}
}</p>

<h1>Add a new student to the dictionary</h1>

<p>students['Alice'] = {'age': 20, 'courses': {'Math', 'Science'}}</p>

<h1>Remove a student from the dictionary</h1>

<p>del students['Bob']</p>

<h1>Get the courses taken by John</h1>

<p>john<em>courses = students['John']['courses']
print(john</em>courses)  # Output: {'Math', 'Science'}</p>

<h1>Get the students who take Math</h1>

<p>math<em>students = [student for student, info in students.items() if 'Math' in info['courses']]
print(math</em>students)  # Output: ['John', 'Jane', 'Alice']</p>

<h1>Get the students who take both Math and Science</h1>

<p>math<em>science</em>students = [student for student, info in students.items() if 'Math' in info['courses'] and 'Science' in info['courses']]
print(math<em>science</em>students)  # Output: ['John', 'Alice']
```</p>

<p>In this example, we create a dictionary of student information, where each student is associated with their age and courses taken. We then add a new student to the dictionary, remove a student from the dictionary, and perform various set operations to get the courses taken by a student, the students who take a particular course, and the students who take both Math and Science.</p>
