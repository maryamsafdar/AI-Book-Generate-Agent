<p><strong>Chapter 6.4: Hands-on Exercise - Lists and Tuples</strong></p>

<p><strong>Introduction</strong></p>

<p>In the previous chapters, we have discussed the basics of lists and tuples in Python. Lists are ordered collections of items that can be of any data type, including strings, integers, floats, and other lists. Tuples, on the other hand, are ordered, immutable collections of items that can also be of any data type. In this chapter, we will put our knowledge of lists and tuples to the test with a hands-on exercise.</p>

<p><strong>Exercise Overview</strong></p>

<p>In this exercise, we will create a simple program that uses lists and tuples to store and manipulate data. We will create a list of students and a tuple of grades, and then use various methods to add, remove, and modify elements in the list and tuple.</p>

<p><strong>Step 1: Create a List of Students</strong></p>

<p>First, let's create a list of students. We will use the following code to create a list of students:
```python</p>

<h1>Create a list of students</h1>

<p>students = ["John", "Alice", "Bob", "Charlie", "David"]
``<code>
This code creates a list called</code>students` and assigns it the values "John", "Alice", "Bob", "Charlie", and "David".</p>

<p><strong>Step 2: Create a Tuple of Grades</strong></p>

<p>Next, let's create a tuple of grades. We will use the following code to create a tuple of grades:
```python</p>

<h1>Create a tuple of grades</h1>

<p>grades = (90, 85, 95, 80, 92)
``<code>
This code creates a tuple called</code>grades` and assigns it the values 90, 85, 95, 80, and 92.</p>

<p><strong>Step 3: Add a Student to the List</strong></p>

<p>Now, let's add a new student to the list. We will use the <code>append()</code> method to add a new student to the list:
```python</p>

<h1>Add a new student to the list</h1>

<p>students.append("Emily")
```
This code adds the new student "Emily" to the end of the list.</p>

<p><strong>Step 4: Remove a Student from the List</strong></p>

<p>Next, let's remove a student from the list. We will use the <code>remove()</code> method to remove a student from the list:
```python</p>

<h1>Remove a student from the list</h1>

<p>students.remove("Bob")
```
This code removes the student "Bob" from the list.</p>

<p><strong>Step 5: Modify a Grade in the Tuple</strong></p>

<p>Now, let's modify a grade in the tuple. Since tuples are immutable, we cannot modify a grade directly. Instead, we will create a new tuple with the modified grade:
```python</p>

<h1>Create a new tuple with the modified grade</h1>

<p>grades = (90, 85, 96, 80, 92)
```
This code creates a new tuple with the modified grade.</p>

<p><strong>Step 6: Combine the List and Tuple</strong></p>

<p>Finally, let's combine the list and tuple into a single data structure. We will use the <code>zip()</code> function to combine the list and tuple:
```python</p>

<h1>Combine the list and tuple</h1>

<p>student<em>grades = list(zip(students, grades))
``<code>
This code combines the list and tuple into a single data structure called</code>student</em>grades`.</p>

<p><strong>Conclusion</strong></p>

<p>In this chapter, we have completed a hands-on exercise that demonstrates the use of lists and tuples in Python. We created a list of students and a tuple of grades, and then used various methods to add, remove, and modify elements in the list and tuple. We also combined the list and tuple into a single data structure using the <code>zip()</code> function.</p>

<p><strong>Example Code</strong></p>

<p>Here is the complete code for this exercise:
```python</p>

<h1>Create a list of students</h1>

<p>students = ["John", "Alice", "Bob", "Charlie", "David"]</p>

<h1>Create a tuple of grades</h1>

<p>grades = (90, 85, 95, 80, 92)</p>

<h1>Add a new student to the list</h1>

<p>students.append("Emily")</p>

<h1>Remove a student from the list</h1>

<p>students.remove("Bob")</p>

<h1>Create a new tuple with the modified grade</h1>

<p>grades = (90, 85, 96, 80, 92)</p>

<h1>Combine the list and tuple</h1>

<p>student_grades = list(zip(students, grades))</p>

<h1>Print the combined list and tuple</h1>

<p>print(student_grades)
<code>
This code will output the following:
</code>python
[('John', 90), ('Alice', 85), ('Charlie', 96), ('David', 80), ('Emily', 92)]
```
This output shows the combined list and tuple, with each student paired with their corresponding grade.</p>
