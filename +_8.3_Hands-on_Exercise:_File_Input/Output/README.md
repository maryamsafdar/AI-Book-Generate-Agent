<p><strong>Chapter 8.3: Hands-on Exercise - File Input/Output</strong></p>

<p><strong>Introduction</strong></p>

<p>In this chapter, we will delve into the world of file input/output operations. File I/O is a fundamental concept in programming that allows us to read and write data to files. This hands-on exercise will guide you through the process of creating, reading, and writing files using a programming language.</p>

<p><strong>Objective</strong></p>

<p>By the end of this exercise, you will be able to:</p>

<ul>
<li>Create a new file and write data to it</li>
<li>Read data from an existing file</li>
<li>Append data to an existing file</li>
<li>Understand the different modes of file I/O operations</li>
</ul>

<p><strong>Materials Needed</strong></p>

<ul>
<li>A computer with a text editor or IDE (Integrated Development Environment)</li>
<li>A programming language of your choice (e.g., Python, Java, C++)</li>
<li>A sample text file (optional)</li>
</ul>

<p><strong>Step 1: Creating a New File and Writing Data</strong></p>

<p>In this step, we will create a new file and write some data to it. Let's use Python as our programming language.</p>

<p>```python</p>

<h1>Open a new file in write mode</h1>

<p>file = open("example.txt", "w")</p>

<h1>Write some data to the file</h1>

<p>file.write("Hello, World!")</p>

<h1>Close the file</h1>

<p>file.close()
```</p>

<p>In this code, we open a new file called <code>example.txt</code> in write mode (<code>"w"</code>). We then write the string <code>"Hello, World!"</code> to the file using the <code>write()</code> method. Finally, we close the file using the <code>close()</code> method.</p>

<p><strong>Step 2: Reading Data from an Existing File</strong></p>

<p>In this step, we will read data from an existing file. Let's use the same file we created in Step 1.</p>

<p>```python</p>

<h1>Open the file in read mode</h1>

<p>file = open("example.txt", "r")</p>

<h1>Read the data from the file</h1>

<p>data = file.read()</p>

<h1>Print the data</h1>

<p>print(data)</p>

<h1>Close the file</h1>

<p>file.close()
```</p>

<p>In this code, we open the file <code>example.txt</code> in read mode (<code>"r"</code>). We then read the data from the file using the <code>read()</code> method and store it in the variable <code>data</code>. Finally, we print the data to the console and close the file.</p>

<p><strong>Step 3: Appending Data to an Existing File</strong></p>

<p>In this step, we will append some data to an existing file. Let's use the same file we created in Step 1.</p>

<p>```python</p>

<h1>Open the file in append mode</h1>

<p>file = open("example.txt", "a")</p>

<h1>Append some data to the file</h1>

<p>file.write(" This is some additional data.")</p>

<h1>Close the file</h1>

<p>file.close()
```</p>

<p>In this code, we open the file <code>example.txt</code> in append mode (<code>"a"</code>). We then append the string <code>" This is some additional data."</code> to the file using the <code>write()</code> method. Finally, we close the file.</p>

<p><strong>Step 4: Understanding File Modes</strong></p>

<p>In this step, we will explore the different modes of file I/O operations.</p>

<p>| Mode | Description |
| --- | --- |
| <code>"r"</code> | Open a file in read mode. If the file does not exist, an error will occur. |
| <code>"w"</code> | Open a file in write mode. If the file does not exist, it will be created. If the file exists, its contents will be overwritten. |
| <code>"a"</code> | Open a file in append mode. If the file does not exist, it will be created. If the file exists, data will be appended to the end of the file. |
| <code>"r+"</code> | Open a file in read and write mode. If the file does not exist, an error will occur. |
| <code>"w+"</code> | Open a file in read and write mode. If the file does not exist, it will be created. If the file exists, its contents will be overwritten. |
| <code>"a+"</code> | Open a file in read and append mode. If the file does not exist, it will be created. If the file exists, data will be appended to the end of the file. |</p>

<p><strong>Conclusion</strong></p>

<p>In this hands-on exercise, we explored the basics of file input/output operations. We created a new file, wrote data to it, read data from it, and appended data to it. We also learned about the different modes of file I/O operations. With this knowledge, you can now perform file I/O operations in your own programs.</p>

<p><strong>Exercise</strong></p>

<ol>
<li>Create a new file called <code>numbers.txt</code> and write the numbers 1 to 10 to it.</li>
<li>Read the data from the file <code>numbers.txt</code> and print it to the console.</li>
<li>Append the numbers 11 to 20 to the file <code>numbers.txt</code>.</li>
<li>Read the updated data from the file <code>numbers.txt</code> and print it to the console.</li>
</ol>

<p><strong>Solution</strong></p>

<p>```python</p>

<h1>Create a new file and write numbers 1 to 10 to it</h1>

<p>file = open("numbers.txt", "w")
for i in range(1, 11):
    file.write(str(i) + "\n")
file.close()</p>

<h1>Read the data from the file and print it to the console</h1>

<p>file = open("numbers.txt", "r")
data = file.read()
print(data)
file.close()</p>

<h1>Append numbers 11 to 20 to the file</h1>

<p>file = open("numbers.txt", "a")
for i in range(11, 21):
    file.write(str(i) + "\n")
file.close()</p>

<h1>Read the updated data from the file and print it to the console</h1>

<p>file = open("numbers.txt", "r")
data = file.read()
print(data)
file.close()
```</p>
