<p><strong>Chapter 3.4: Hands-on Exercise - Control Structures</strong></p>

<p><strong>Introduction</strong></p>

<p>In the previous chapters, we have discussed the basics of programming and the importance of control structures in writing efficient code. Control structures are the building blocks of any programming language, and they allow us to control the flow of our program's execution. In this chapter, we will put our knowledge of control structures into practice with a hands-on exercise.</p>

<p><strong>Exercise Overview</strong></p>

<p>In this exercise, we will create a simple program that uses control structures to simulate a banking system. The program will allow users to deposit, withdraw, and check their account balance. We will use if-else statements, for loops, and while loops to control the flow of our program.</p>

<p><strong>Step 1: Define the Program Requirements</strong></p>

<p>Before we start writing our program, let's define the requirements. Our program should have the following features:</p>

<ul>
<li>Allow users to deposit money into their account</li>
<li>Allow users to withdraw money from their account</li>
<li>Allow users to check their account balance</li>
<li>Prevent users from withdrawing more money than they have in their account</li>
<li>Prevent users from depositing a negative amount of money</li>
</ul>

<p><strong>Step 2: Write the Program</strong></p>

<p>Here is a sample implementation of the program in Python:
```python</p>

<h1>Initialize the account balance</h1>

<p>balance = 0</p>

<h1>Main program loop</h1>

<p>while True:
    # Display the menu
    print("Banking System Menu:")
    print("1. Deposit money")
    print("2. Withdraw money")
    print("3. Check balance")
    print("4. Exit")</p>

<pre><code># Get the user's choice
choice = input("Enter your choice: ")

# Handle the user's choice
if choice == "1":
    # Deposit money
    amount = float(input("Enter the amount to deposit: "))
    if amount &lt; 0:
        print("Error: Cannot deposit a negative amount.")
    else:
        balance += amount
        print("Deposit successful. New balance: $", balance)
elif choice == "2":
    # Withdraw money
    amount = float(input("Enter the amount to withdraw: "))
    if amount &lt; 0:
        print("Error: Cannot withdraw a negative amount.")
    elif amount &gt; balance:
        print("Error: Insufficient funds.")
    else:
        balance -= amount
        print("Withdrawal successful. New balance: $", balance)
elif choice == "3":
    # Check balance
    print("Current balance: $", balance)
elif choice == "4":
    # Exit the program
    print("Goodbye!")
    break
else:
    print("Error: Invalid choice. Please try again.")
</code></pre>

<p>```
<strong>Step 3: Test the Program</strong></p>

<p>Now that we have written our program, let's test it to make sure it works as expected. We can test the program by running it and trying out different scenarios. For example, we can deposit money, withdraw money, and check our balance to make sure the program is updating the balance correctly.</p>

<p><strong>Conclusion</strong></p>

<p>In this chapter, we have put our knowledge of control structures into practice with a hands-on exercise. We have created a simple banking system program that uses if-else statements, for loops, and while loops to control the flow of the program. We have also tested the program to make sure it works as expected. This exercise has demonstrated the importance of control structures in writing efficient and effective code.</p>

<p><strong>Exercise Questions</strong></p>

<ol>
<li>What is the purpose of the while loop in the program?</li>
<li>How does the program prevent users from withdrawing more money than they have in their account?</li>
<li>What happens if the user enters a negative amount when depositing or withdrawing money?</li>
<li>How does the program handle invalid user input?</li>
</ol>

<p><strong>Exercise Answers</strong></p>

<ol>
<li>The while loop is used to repeatedly display the menu and handle the user's choice until the user chooses to exit the program.</li>
<li>The program checks if the withdrawal amount is greater than the current balance before allowing the withdrawal. If the amount is greater, it displays an error message and prevents the withdrawal.</li>
<li>If the user enters a negative amount when depositing or withdrawing money, the program displays an error message and prevents the transaction.</li>
<li>The program handles invalid user input by displaying an error message and prompting the user to enter a valid choice.</li>
</ol>
