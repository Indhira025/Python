# 
<h1>🐍 Python Programming – Intermediate Python</h1>

<p>
This section covers intermediate-level Python concepts that help improve problem-solving and coding efficiency. Here code to be write clean, optimized, and reusable code.
</p>

<hr>

<h2>📌 Repository Contents</h2>
<ul>
  <li>Control Statements</li>
  <li>Conditional Statements</li>
  <li>Functions</li>
  <li>Map, Filter, Reduce</li>
  <li>Lambda Functions</li>
  <li>Recursion</li>
  <li>Comprehension</li>
  <li>File Handling</li>
</ul>

<hr>

<h2>🔁 Control Statements</h2>
<p>
<li>Control statements are used to <b>control the flow of execution</b> in a Python program. They decide <b>which code runs and how many times it runs.</b> </li>
 <li>There are two control statements: </li>
  <ul>
    <li> For loop</li>
    <li> While loop</li>
  </ul>
</p>

<h3>for Loop</h3>
<p>The for loop is used to iterate over a sequence such as a list, tuple, string, or range. </p>
<b> Syntax:</b>
<pre>for variable in sequence:
      statements </pre>


<pre><code>
for i in range(1, 6):
    print(i)
</code>
</pre>

<b>Key Points:</b>
<li> Executes a block of code <b> for a fixed number of times</b></li>
<li> Commonly used with range()</li>
<li> Best when the number of iterations is known</li>

<h3>while Loop</h3>
<p>The while loop runs as long as a given condition is true. </p>
<b>Syntax:</b>
<pre>while condition:
    statements</pre>
<pre><code>
i = 1
while i <= 5:
    print(i)
    i += 1
</code></pre>

<b>Key Points:</b>
<li> Executes code <b>until the condition becomes false</b></li>
<li> Used when the number of iterations is <b>not known in advance</b></li>
<li> Condition must be updated to avoid infinite loops</li>

<hr>

<h2>🔀 Conditional Statements</h2>
<p> 
<li> Conditional statements are used to <b>make decisions</b> in a program based on conditions. </li>
<li>There are four conditional statements: </li>  
  <ul>
    <li>If </li>
    <li>Else </li>
    <li>Elif</li>
    <li>Break </li>
  </ul>
</p>

<h3>if Statement</h3>
<p>Executes a block of code <b>only when the condition is true.</b></p>
<pre><code>
age = 18
if age >= 18:
    print("Eligible to vote")
</code></pre>

<h3>if-else Statement</h3>
<p>Executes one block if the condition is true, otherwise executes the else block. </p>
<pre><code>
num = 7
if num % 2 == 0:
    print("Even number")
else:
    print("Odd number")
</code></pre>

<h3>if-elif-else Statement</h3>
<p> Used to check <b>multiple conditions</b></p>
<pre><code>
marks = 65
if marks >= 90:
    print("Grade A")
elif marks >= 60:
    print("Grade B")
else:
    print("Grade C")
</code></pre>

<h3>break Statement</h3>
<p>Used inside loops to <b>stop execution immediately</b> when a condition is met.</p>
<pre><code>
for i in range(1, 6):
    if i == 4:
        break
    print(i)
</code></pre>

<hr>

<h2>🔧 Functions in Python</h2>
<p>A function in Python is a block of reusable code that performs a specific task. Functions help make programs <b>simple, organized, and reusable.</b></p>
<b>Syntax:</b>
<pre>
  def function_name(parameters):
    statements
</pre>
<pre><code>
def greet():
    print("Hello, welcome to Python")
greet()
</code></pre>

<h3>Function with Parameters</h3>
<pre><code>
def add(a, b):
    print(a + b)
add(10, 20)
</code></pre>

<h3>Function with Return Value</h3>
<pre><code>
def square(num):
    return num * num
print(square(5))
</code></pre>

<h3>Types of Functions</h3>
<ul>
  <li>Built-in Functions – print(), len(), type()</li>
  <li>User-defined Functions - Created by the user using def</li>
</ul>
<pre><code>
def kiran(a,b):
    for i in range(a,b):
          if  i % 2 == 0:
                print(‘even’)
kiran(11,16)
</code></pre>

<b>Key Points</b>
<ul>
  <li>Defined using the def keyword</li>
  <li>Improves code reusability</li>
  <li>Reduces repetition</li>
  <li>Makes code easy to understand </li>
  <li>Variables outside the function is known as <b>Global Variables</b></li>
  <li>Variables inside the function is known as <b>Local Variables</b></li>
</ul>

<b>Modularization Using Functions:</b>
<p>Extracting (Calling) the function from other file is known as <b>modularization</b></p>
<b>Syntax:</b>
<p> from file_name import function_name</p>
<pre><code>
from part_2 import kiran                             part_2 file
print(‘I am from uk’)                                def kiran():
def sharuk():                                            print(‘I am from usa’)
    for i in range(1,5):
         print(f‘good morning : {i}’)
</code></pre>

<hr>

<h2>📦 Map, Filter, Reduce</h2>
<p>Map, Filter, and Reduce are built-in functional tools used to process data in a simple and efficient way.</p>

<h3>map()</h3>
<p>The map() function applies a given function to <b>each element</b> of an iterable.</p>
<b>Syntax:</b>
      <pre>map(function, iterable)</pre>
 <pre><code>
         def fun(b):
             if b % 2 ==0:
                  return b
              else:
                  return ‘USA’
          sol = map(fun,[10,11,12,13,14,15])
          print(sol)
 </code></pre>     

<h3>filter()</h3>
<p>The filter() function selects elements from an iterable <b>based on a condition.</b></p>
<b>Syntax:</b>
      <pre>filter(function, iterable)</pre>
 <pre><code>   
      def fun(b):
          if b % 2 ==0:
              return b          
      sol = filter(fun,[10,11,12,13,14,15])
      print(sol)
 </code></pre>

<h3>reduce()</h3>
<p> The reduce() function reduces an iterable to a single value by applying a function repeatedly. Reduce() is available in the functools module.</p>
<b>Syntax:</b>
<pre>
  from functools import reduce
  reduce(function, iterable)
</pre>

<pre><code>
from functools import reduce
f = [1, 2, 3, 4]
sol = reduce(lambda x,y: x+y,f)
print(sol)
</code></pre>

<hr>

<h2>⚡ Lambda Functions</h2>
<p>
<li>A lambda function is a small anonymous function (function without a name). </li>
<li>It is used for short, simple operations.</li> 
</p>

<b>Syntax:</b>
<pre>lambda arguments: expression</pre>

<pre><code>
add = lambda a, b: a + b
print(add(5, 3))
</code></pre>

<h3>Lambda with map()</h3>
<pre><code>
numbers = [1, 2, 3, 4]
result = list(map(lambda x: x * 2, numbers))
print(result)
</code></pre>

<h3>Lambda with filter()</h3>
<pre><code>
numbers = [1, 2, 3, 4, 5]
result = list(filter(lambda x: x % 2 == 0, numbers))
print(result) 
</code></pre>

<h3>Lambda with reduce()</h3>
<pre><code>
from functools import reduce
numbers = [1, 2, 3, 4]
result = reduce(lambda a, b: a + b, numbers)
print(result) 
</code></pre>

<b>Key Points </b>
<ul>
  <li>No def keyword</li>
  <li>Written in one line </li>
  <li>Can have multiple arguments but only one expression</li>
  <li>Used for short and temporary functions</li>
</ul>

<hr>

<h2>🔁 Recursion</h2>
<p>
Recursion is a process where a <b>function calls itself</b> to solve a problem by breaking it into smaller parts.
</p>

<b>Recursion Works:</b>
<ul>
  <li>The function calls itself</li>
  <li>Each call works on a smaller part</li>
  <li>When the base condition is met, the function stops</li>
  <li>The results return back step by step</li>
</ul>

<pre><code>
def count(n):
    if n == 0:
        return
    print(n)
    count(n - 1)

count(3)
</code></pre>

<b> Key Points</b>
<ul>
  <li>Function calls itself</li>
  <li>Base condition is mandatory</li>
  <li>Used to solve problems like factorial, Fibonacci, tree traversal and nested data </li>
</ul>

<hr>

<h2>🧠 Comprehension</h2>
<p> 
<li>Comprehension is used to write the code in single line instead of multiple lines of code.
</li>
 <li>Mainly two types of comprehension: </li> 
  <ul>
    <li>List Comprehension </li>
    <li>Dictionary Comprehension</li>
  </ul>
 <li>In this comprehension we have three syntax </li> 
 <ol>
   <li>One for loop & one print condition </li>
   <li>One for loop & one if condition & one print condition</li>
   <li>One for loop & one if condition & one else condition & one print condition</li>
 </ol>
</p>

<h3>List Comprehension</h3>
<p><li>One for loop & one print condition</li></p>
<b>Syntax</b>
<pre>[ < print  area>  <for loop> ] </pre>
<pre><code>
Print( [ ‘good morning’  for i in range(1,4) ] ) 
</code></pre>

<p><li>One for loop & one if condition & one print condition</li></p>
<b>Syntax</b>
<pre>[ < print area>   <for loop>  <if condition> ] </pre>
<pre><code>
 Print( [ f’ even: {i}’  for i in range(11,16)  if i % 2 == 0 ] ) 
</code></pre>

<p><li>One for loop & one if condition & one else condition & one print condition</li></p>
<b>Syntax</b>
<pre>[ < if print>   <if condition>  <else>  <else print>   <for loop> ] </pre>
<pre><code>
Print( [ f’ even: {i}’    if i % 2 == 0     else   f’ odd: {i}’   for i in range(11,16) ] ) 
</code></pre>

<h3>Dictionary Comprehension</h3>
<p><li>One for loop & one print condition</li></p>
<b>Syntax</b>
<pre>[ < print  area>  <for loop> ] </pre>
<pre><code>
fruits = { ‘ apple’ : 100 , ‘ banana ‘ : 200 , ‘ carrot ‘ : 300 }
Print( { i : fruits[i] * 2   for i in fruits } ) 
</code></pre>

<p><li>One for loop & one if condition & one print condition</li></p>
<b>Syntax</b>
<pre>[ < print area>   <for loop>  <if condition> ] </pre>
<pre><code>
fruits = { ‘ apple’ : 100 , ‘ banana ‘ : 200 , ‘ carrot ‘ : 300 }
Print( { i : fruits[i] * 3   for i in fruits  if fruits[i] > 150 } ) 
</code></pre>

<p><li>One for loop & one if condition & one else condition & one print condition</li></p>
<b>Syntax</b>
<pre>[ < if print>   <if condition>  <else>  <else print>   <for loop> ] </pre>
<pre><code>
fruits = { ‘ apple’ : 100 , ‘ banana ‘ : 200 , ‘ carrot ‘ : 300 }
Print( { i : ( j * 3  if j > 150  else  j * 2 )   for i, j in fruits. items() } ) 
</code></pre>

<hr>

<h2>📂 File Handling</h2>
<p>
<li>File handling is used to create, read, write, and update files in Python.</li>
<li>It helps store data permanently. </li>
</p>

<h3>Opening a File</h3>
<p> file = open("data.txt", "mode") </p>
<h3>File Modes</h3>
<ul>
  <li> "r" → Read</li>
  <li> "w" → Write (creates new file / overwrites existing)</li>
  <li> "a" → Append </li>
</ul>

<h3>Reading a File</h3>
<pre><code>
file = open("data.txt", "r")
print(file.read())
print(content) 
file.close()
</code></pre>

<h3>Writing to a File</h3>
<pre><code>
file = open("data.txt", "w")
file.write("Hello Python")
file.close()
</code></pre>

<h3>Appending to a File </h3>
<pre><code>
file = open("data.txt", "a")
file.write("\n Welcome")
file.close()
</code></pre>

<h3>Using with Statement</h3>
<p>Automatically closes the file. </p>
<pre><code>
with open("data.txt", "r") as file:
    print(file.read())
</code></pre>

<b> Key Points</b>
<ul>
  <li>Files are opened using open()</li>
  <li>Always close files after use</li>
  <li>with statement is safer and cleaner</li>
</ul>

<hr>

<h2>✅ Conclusion</h2>
<p>
This repository strengthens intermediate Python concepts such as control flow,
functions, functional programming, recursion, comprehensions, and file handling.
It helps learners write efficient, readable, and reusable Python programs.
</p>

<p><b>Happy Coding! 🚀</b></p>
