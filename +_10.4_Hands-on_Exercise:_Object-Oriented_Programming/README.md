<p><strong>Chapter 10.4: Hands-on Exercise - Object-Oriented Programming</strong></p>

<p><strong>Introduction</strong></p>

<p>In this chapter, we will delve into the world of object-oriented programming (OOP) through a hands-on exercise. OOP is a programming paradigm that revolves around the concept of objects and classes, which are used to represent real-world entities and their interactions. By the end of this chapter, you will have a solid understanding of the fundamental principles of OOP and how to apply them in a practical setting.</p>

<p><strong>Exercise Overview</strong></p>

<p>In this exercise, we will create a simple banking system using OOP principles. The system will consist of two classes: <code>Account</code> and <code>Customer</code>. The <code>Account</code> class will represent a bank account, while the <code>Customer</code> class will represent a bank customer. We will define properties and methods for each class and demonstrate how they interact with each other.</p>

<p><strong>Step 1: Define the Account Class</strong></p>

<p>The <code>Account</code> class will have the following properties:</p>

<ul>
<li><code>accountNumber</code>: a unique identifier for the account</li>
<li><code>balance</code>: the current balance of the account</li>
<li><code>accountType</code>: the type of account (e.g., checking, savings)</li>
</ul>

<p>The <code>Account</code> class will also have the following methods:</p>

<ul>
<li><code>deposit(amount)</code>: adds the specified amount to the account balance</li>
<li><code>withdraw(amount)</code>: subtracts the specified amount from the account balance</li>
<li><code>getBalance()</code>: returns the current account balance</li>
</ul>

<p>Here is the code for the <code>Account</code> class:
```python
class Account:
    def <strong>init</strong>(self, accountNumber, accountType):
        self.accountNumber = accountNumber
        self.accountType = accountType
        self.balance = 0.0</p>

<pre><code>def deposit(self, amount):
    self.balance += amount

def withdraw(self, amount):
    if amount &gt; self.balance:
        print("Insufficient funds")
    else:
        self.balance -= amount

def getBalance(self):
    return self.balance
</code></pre>

<p>```
<strong>Step 2: Define the Customer Class</strong></p>

<p>The <code>Customer</code> class will have the following properties:</p>

<ul>
<li><code>customerName</code>: the name of the customer</li>
<li><code>customerAddress</code>: the address of the customer</li>
<li><code>account</code>: an instance of the <code>Account</code> class</li>
</ul>

<p>The <code>Customer</code> class will also have the following methods:</p>

<ul>
<li><code>openAccount(accountNumber, accountType)</code>: creates a new account for the customer</li>
<li><code>deposit(amount)</code>: deposits the specified amount into the customer's account</li>
<li><code>withdraw(amount)</code>: withdraws the specified amount from the customer's account</li>
<li><code>getAccountBalance()</code>: returns the current balance of the customer's account</li>
</ul>

<p>Here is the code for the <code>Customer</code> class:
```python
class Customer:
    def <strong>init</strong>(self, customerName, customerAddress):
        self.customerName = customerName
        self.customerAddress = customerAddress
        self.account = None</p>

<pre><code>def openAccount(self, accountNumber, accountType):
    self.account = Account(accountNumber, accountType)

def deposit(self, amount):
    if self.account:
        self.account.deposit(amount)
    else:
        print("No account found")

def withdraw(self, amount):
    if self.account:
        self.account.withdraw(amount)
    else:
        print("No account found")

def getAccountBalance(self):
    if self.account:
        return self.account.getBalance()
    else:
        print("No account found")
</code></pre>

<p>```
<strong>Step 3: Create a Customer and Open an Account</strong></p>

<p>Create a new customer and open an account for them:
<code>python
customer = Customer("John Doe", "123 Main St")
customer.openAccount("123456789", "checking")
</code>
<strong>Step 4: Deposit and Withdraw Funds</strong></p>

<p>Deposit $100 into the customer's account:
<code>python
customer.deposit(100.0)
</code>
Withdraw $50 from the customer's account:
<code>python
customer.withdraw(50.0)
</code>
<strong>Step 5: Get the Account Balance</strong></p>

<p>Get the current balance of the customer's account:
<code>python
balance = customer.getAccountBalance()
print("Account balance:", balance)
</code>
<strong>Conclusion</strong></p>

<p>In this hands-on exercise, we created a simple banking system using OOP principles. We defined two classes, <code>Account</code> and <code>Customer</code>, and demonstrated how they interact with each other. We also created a customer, opened an account for them, deposited and withdrew funds, and retrieved the account balance. This exercise illustrates the fundamental principles of OOP, including encapsulation, inheritance, and polymorphism.</p>

<p><strong>Exercise Questions</strong></p>

<ol>
<li>What is the purpose of the <code>__init__</code> method in the <code>Account</code> class?</li>
<li>How does the <code>deposit</code> method in the <code>Account</code> class handle invalid deposit amounts?</li>
<li>What is the purpose of the <code>openAccount</code> method in the <code>Customer</code> class?</li>
<li>How does the <code>withdraw</code> method in the <code>Customer</code> class handle insufficient funds?</li>
<li>What is the purpose of the <code>getAccountBalance</code> method in the <code>Customer</code> class?</li>
</ol>

<p><strong>Exercise Solutions</strong></p>

<ol>
<li>The <code>__init__</code> method in the <code>Account</code> class initializes the account properties, including the account number, account type, and balance.</li>
<li>The <code>deposit</code> method in the <code>Account</code> class does not handle invalid deposit amounts. It simply adds the specified amount to the account balance.</li>
<li>The <code>openAccount</code> method in the <code>Customer</code> class creates a new account for the customer and assigns it to the customer's account property.</li>
<li>The <code>withdraw</code> method in the <code>Customer</code> class checks if the account balance is sufficient before withdrawing the specified amount. If the balance is insufficient, it prints an error message.</li>
<li>The <code>getAccountBalance</code> method in the <code>Customer</code> class returns the current balance of the customer's account.</li>
</ol>
