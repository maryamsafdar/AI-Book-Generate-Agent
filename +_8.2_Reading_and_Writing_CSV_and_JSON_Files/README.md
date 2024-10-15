<p><strong>Chapter 8.2: Reading and Writing CSV and JSON Files</strong></p>

<p><strong>Introduction</strong></p>

<p>In the world of data analysis and processing, two of the most widely used file formats are CSV (Comma Separated Values) and JSON (JavaScript Object Notation). CSV files are used to store tabular data, such as spreadsheets, while JSON files are used to store data in a key-value format. In this chapter, we will explore how to read and write CSV and JSON files using Python.</p>

<p><strong>Reading CSV Files</strong></p>

<p>CSV files are plain text files that contain tabular data. Each row in the file represents a single record, and each column represents a field or attribute of that record. The values in each row are separated by commas, hence the name Comma Separated Values.</p>

<p>To read a CSV file in Python, we can use the <code>csv</code> module. Here is an example of how to read a CSV file:
```python
import csv</p>

<h1>Open the CSV file</h1>

<p>with open('data.csv', 'r') as file:
    # Create a CSV reader object
    reader = csv.reader(file)</p>

<pre><code># Iterate over the rows in the file
for row in reader:
    print(row)
</code></pre>

<p>``<code>
In this example, we open the</code>data.csv<code>file in read mode (</code>'r'<code>) and create a</code>csv.reader<code>object to read the file. We then iterate over the rows in the file using a</code>for` loop, and print each row to the console.</p>

<p><strong>Writing CSV Files</strong></p>

<p>To write a CSV file in Python, we can use the <code>csv</code> module again. Here is an example of how to write a CSV file:
```python
import csv</p>

<h1>Define the data to write to the file</h1>

<p>data = [
    ['Name', 'Age', 'City'],
    ['John Doe', 30, 'New York'],
    ['Jane Doe', 25, 'Los Angeles']
]</p>

<h1>Open the CSV file</h1>

<p>with open('data.csv', 'w') as file:
    # Create a CSV writer object
    writer = csv.writer(file)</p>

<pre><code># Write the data to the file
writer.writerows(data)
</code></pre>

<p>``<code>
In this example, we define a list of lists, where each inner list represents a row in the CSV file. We then open the</code>data.csv<code>file in write mode (</code>'w'<code>) and create a</code>csv.writer<code>object to write the file. We then use the</code>writerows` method to write the data to the file.</p>

<p><strong>Reading JSON Files</strong></p>

<p>JSON files are plain text files that contain data in a key-value format. Each key-value pair is separated by a colon, and each pair is separated by a comma.</p>

<p>To read a JSON file in Python, we can use the <code>json</code> module. Here is an example of how to read a JSON file:
```python
import json</p>

<h1>Open the JSON file</h1>

<p>with open('data.json', 'r') as file:
    # Load the JSON data from the file
    data = json.load(file)</p>

<pre><code># Print the data
print(data)
</code></pre>

<p>``<code>
In this example, we open the</code>data.json<code>file in read mode (</code>'r'<code>) and use the</code>json.load` function to load the JSON data from the file. We then print the data to the console.</p>

<p><strong>Writing JSON Files</strong></p>

<p>To write a JSON file in Python, we can use the <code>json</code> module again. Here is an example of how to write a JSON file:
```python
import json</p>

<h1>Define the data to write to the file</h1>

<p>data = {
    'name': 'John Doe',
    'age': 30,
    'city': 'New York'
}</p>

<h1>Open the JSON file</h1>

<p>with open('data.json', 'w') as file:
    # Dump the JSON data to the file
    json.dump(data, file)
``<code>
In this example, we define a dictionary that represents the data to write to the file. We then open the</code>data.json<code>file in write mode (</code>'w'<code>) and use the</code>json.dump` function to write the JSON data to the file.</p>

<p><strong>Conclusion</strong></p>

<p>In this chapter, we have explored how to read and write CSV and JSON files using Python. We have seen how to use the <code>csv</code> module to read and write CSV files, and how to use the <code>json</code> module to read and write JSON files. These skills are essential for working with data in Python, and will be useful in a wide range of applications.</p>

<p><strong>Exercise</strong></p>

<ol>
<li>Write a Python program that reads a CSV file and prints the data to the console.</li>
<li>Write a Python program that writes a CSV file from a list of lists.</li>
<li>Write a Python program that reads a JSON file and prints the data to the console.</li>
<li>Write a Python program that writes a JSON file from a dictionary.</li>
</ol>

<p><strong>Solution</strong></p>

<ol>
<li>Here is a Python program that reads a CSV file and prints the data to the console:
```python
import csv</li>
</ol>

<p>with open('data.csv', 'r') as file:
    reader = csv.reader(file)
    for row in reader:
        print(row)
<code>
2. Here is a Python program that writes a CSV file from a list of lists:
</code>python
import csv</p>

<p>data = [
    ['Name', 'Age', 'City'],
    ['John Doe', 30, 'New York'],
    ['Jane Doe', 25, 'Los Angeles']
]</p>

<p>with open('data.csv', 'w') as file:
    writer = csv.writer(file)
    writer.writerows(data)
<code>
3. Here is a Python program that reads a JSON file and prints the data to the console:
</code>python
import json</p>

<p>with open('data.json', 'r') as file:
    data = json.load(file)
    print(data)
<code>
4. Here is a Python program that writes a JSON file from a dictionary:
</code>python
import json</p>

<p>data = {
    'name': 'John Doe',
    'age': 30,
    'city': 'New York'
}</p>

<p>with open('data.json', 'w') as file:
    json.dump(data, file)
```</p>
