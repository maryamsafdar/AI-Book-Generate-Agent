<p><strong>Chapter 9.3: Hands-on Exercise - Exception Handling</strong></p>

<p><strong>Introduction</strong></p>

<p>In the previous chapters, we have discussed the importance of exception handling in programming. Exception handling is a crucial aspect of writing robust and reliable code. It allows developers to handle unexpected errors and exceptions that may occur during the execution of a program. In this chapter, we will put our knowledge of exception handling into practice through a hands-on exercise.</p>

<p><strong>Exercise Overview</strong></p>

<p>In this exercise, we will create a simple banking system that allows users to deposit and withdraw money from their accounts. We will use exception handling to handle potential errors that may occur during these transactions.</p>

<p><strong>Step 1: Create a Bank Account Class</strong></p>

<p>Create a new class called <code>BankAccount</code> with the following properties:</p>

<ul>
<li><code>accountNumber</code>: a unique identifier for the account</li>
<li><code>accountHolder</code>: the name of the account holder</li>
<li><code>balance</code>: the current balance of the account</li>
</ul>

<p><code>python
class BankAccount:
    def __init__(self, accountNumber, accountHolder, balance=0):
        self.accountNumber = accountNumber
        self.accountHolder = accountHolder
        self.balance = balance
</code></p>

<p><strong>Step 2: Add Deposit and Withdraw Methods</strong></p>

<p>Add two methods to the <code>BankAccount</code> class: <code>deposit</code> and <code>withdraw</code>. These methods should update the account balance accordingly.</p>

<p>```python
class BankAccount:
    # ...</p>

<pre><code>def deposit(self, amount):
    if amount &lt;= 0:
        raise ValueError("Deposit amount must be positive")
    self.balance += amount

def withdraw(self, amount):
    if amount &lt;= 0:
        raise ValueError("Withdrawal amount must be positive")
    if amount &gt; self.balance:
        raise ValueError("Insufficient funds")
    self.balance -= amount
</code></pre>

<p>```</p>

<p><strong>Step 3: Handle Exceptions</strong></p>

<p>Create a new function called <code>processTransaction</code> that takes a <code>BankAccount</code> object and a transaction type (either "deposit" or "withdrawal") as input. This function should call the corresponding method on the <code>BankAccount</code> object and handle any exceptions that may occur.</p>

<p><code>python
def processTransaction(account, transactionType, amount):
    try:
        if transactionType == "deposit":
            account.deposit(amount)
        elif transactionType == "withdrawal":
            account.withdraw(amount)
        else:
            raise ValueError("Invalid transaction type")
        print(f"Transaction successful. New balance: {account.balance}")
    except ValueError as e:
        print(f"Error: {e}")
</code></p>

<p><strong>Step 4: Test the Code</strong></p>

<p>Create a new <code>BankAccount</code> object and test the <code>processTransaction</code> function with different scenarios.</p>

<p>```python
account = BankAccount("12345", "John Doe", 1000)</p>

<p>processTransaction(account, "deposit", 500)
processTransaction(account, "withdrawal", 200)
processTransaction(account, "withdrawal", 1500)  # insufficient funds
processTransaction(account, "invalid", 100)  # invalid transaction type
```</p>

<p><strong>Conclusion</strong></p>

<p>In this hands-on exercise, we have demonstrated the importance of exception handling in programming. We have created a simple banking system that handles potential errors and exceptions that may occur during transactions. By using try-except blocks and raising custom exceptions, we have made our code more robust and reliable.</p>

<p><strong>Exercise Questions</strong></p>

<ol>
<li>What is the purpose of exception handling in programming?</li>
<li>How does the <code>processTransaction</code> function handle exceptions?</li>
<li>What happens when the user attempts to withdraw more money than is available in their account?</li>
<li>How can you modify the <code>BankAccount</code> class to handle multiple account holders?</li>
</ol>

<p><strong>Exercise Solutions</strong></p>

<ol>
<li>Exception handling is used to handle unexpected errors and exceptions that may occur during the execution of a program.</li>
<li>The <code>processTransaction</code> function uses a try-except block to catch any exceptions that may occur during the transaction. If an exception occurs, it prints an error message to the user.</li>
<li>When the user attempts to withdraw more money than is available in their account, a <code>ValueError</code> exception is raised with the message "Insufficient funds".</li>
<li>To modify the <code>BankAccount</code> class to handle multiple account holders, you can add a list of account holders to the class and update the <code>deposit</code> and <code>withdraw</code> methods to handle multiple account holders.</li>
</ol>
