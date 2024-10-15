<p><strong>Chapter 8: File Input/Output</strong></p>

<p><strong>8.1 Introduction</strong></p>

<p>File input/output (I/O) is a fundamental concept in programming that allows you to read and write data to files. Files are used to store data persistently, even after a program has finished executing. In this chapter, we will explore the basics of file I/O, including how to open, read, write, and close files.</p>

<p><strong>8.2 File Modes</strong></p>

<p>When working with files, you need to specify the mode in which you want to open the file. The mode determines the type of operations you can perform on the file. The most common file modes are:</p>

<ul>
<li><strong>Read Mode ('r')</strong>: Opens the file for reading only. If the file does not exist, an error occurs.</li>
<li><strong>Write Mode ('w')</strong>: Opens the file for writing only. If the file does not exist, it is created. If the file already exists, its contents are deleted.</li>
<li><strong>Append Mode ('a')</strong>: Opens the file for appending only. If the file does not exist, it is created. If the file already exists, new data is appended to the end of the file.</li>
<li><strong>Read and Write Mode ('r+')</strong>: Opens the file for both reading and writing.</li>
<li><strong>Binary Mode ('b')</strong>: Opens the file in binary format, which is used for reading and writing binary data such as images and audio files.</li>
</ul>

<p><strong>8.3 Opening a File</strong></p>

<p>To open a file, you use the <code>open()</code> function, which returns a file object. The <code>open()</code> function takes two arguments: the name of the file and the mode in which to open the file.</p>

<p><code>python
file = open('example.txt', 'r')
</code></p>

<p>In this example, we open a file named <code>example.txt</code> in read mode.</p>

<p><strong>8.4 Reading from a File</strong></p>

<p>Once you have opened a file, you can read its contents using the <code>read()</code> method. The <code>read()</code> method returns the entire contents of the file as a string.</p>

<p><code>python
file = open('example.txt', 'r')
contents = file.read()
print(contents)
file.close()
</code></p>

<p>In this example, we open a file named <code>example.txt</code> in read mode, read its contents, print the contents, and then close the file.</p>

<p><strong>8.5 Writing to a File</strong></p>

<p>To write to a file, you use the <code>write()</code> method. The <code>write()</code> method takes a string as an argument and writes it to the file.</p>

<p><code>python
file = open('example.txt', 'w')
file.write('Hello, World!')
file.close()
</code></p>

<p>In this example, we open a file named <code>example.txt</code> in write mode, write the string <code>'Hello, World!'</code> to the file, and then close the file.</p>

<p><strong>8.6 Closing a File</strong></p>

<p>It is essential to close a file after you have finished using it. Closing a file frees up system resources and prevents data corruption. You can close a file using the <code>close()</code> method.</p>

<p>```python
file = open('example.txt', 'r')</p>

<h1>Perform file operations</h1>

<p>file.close()
```</p>

<p>In this example, we open a file named <code>example.txt</code> in read mode, perform file operations, and then close the file.</p>

<p><strong>8.7 Using the <code>with</code> Statement</strong></p>

<p>The <code>with</code> statement is a more elegant way to open and close files. The <code>with</code> statement automatically closes the file when you are finished using it, even if an error occurs.</p>

<p><code>python
with open('example.txt', 'r') as file:
    contents = file.read()
    print(contents)
</code></p>

<p>In this example, we open a file named <code>example.txt</code> in read mode using the <code>with</code> statement, read its contents, print the contents, and then automatically close the file.</p>

<p><strong>8.8 Reading and Writing Binary Files</strong></p>

<p>To read and write binary files, you need to open the file in binary mode using the <code>'b'</code> mode.</p>

<p><code>python
with open('image.jpg', 'rb') as file:
    image_data = file.read()
    # Process the image data
</code></p>

<p>In this example, we open a binary file named <code>image.jpg</code> in read binary mode using the <code>with</code> statement, read its contents, and then process the image data.</p>

<p><strong>8.9 Conclusion</strong></p>

<p>In this chapter, we have explored the basics of file input/output in programming. We have learned how to open, read, write, and close files using various modes and methods. We have also learned how to use the <code>with</code> statement to automatically close files and how to read and write binary files. With this knowledge, you can now work with files in your programs and store data persistently.</p>

<p><strong>8.10 Exercises</strong></p>

<ol>
<li>Write a program that reads a file and prints its contents to the console.</li>
<li>Write a program that writes a string to a file.</li>
<li>Write a program that appends a string to a file.</li>
<li>Write a program that reads a binary file and prints its contents to the console.</li>
<li>Write a program that writes a binary file using the <code>with</code> statement.</li>
</ol>

<p><strong>8.11 Solutions</strong></p>

<ol>
<li><code>python
with open('example.txt', 'r') as file:
    contents = file.read()
    print(contents)
</code></li>
<li><code>python
with open('example.txt', 'w') as file:
    file.write('Hello, World!')
</code></li>
<li><code>python
with open('example.txt', 'a') as file:
    file.write('Hello, World!')
</code></li>
<li><code>python
with open('image.jpg', 'rb') as file:
    image_data = file.read()
    print(image_data)
</code></li>
<li><code>python
with open('image.jpg', 'wb') as file:
    file.write(b'Hello, World!')
</code></li>
</ol>
