# 
<h1>🐍 Python Programming – Intermediate Python</h1>

<p>
Python is a beginner-friendly programming language used for software development,
data analysis, and automation. This repository covers fundamental concepts and
basic syntax to get started with Python programming.
</p>

<hr>

<h2>📌 Repository Contents</h2>
<ul>
  <li>Introduction to Python</li>
  <li>Basic Syntax and Comments</li>
  <li>Data Types and Variables</li>
  <li>Type Conversions</li>
  <li>Print Condition</li>
  <li>Operators</li>
  <li>Libraries</li>
  <li>Functions and Built-in Functions</li>
  <li>Strings</li>
  <li>List</li>
  <li>Tuple</li>
  <li>Set</li>
  <li>Dictionary</li>
</ul>

<hr>

<h2>🧠 Introduction to Python</h2>
<p>
  Python is a <b>high-level, interpreted programming language</b> known for its <b>simple syntax, readability, and versatility</b>.It was created by <b>Guido van Rossum</b>, and released in <b>1991</b>. </p>
<p> It is widely used in software development, data analysis, machine learning, web development, automation, and scripting.
</p>

<h1>⭐ Key Features of Python</h1>
<ul>
  <li><b>Easy to Learn & Use</b> – Simple and readable syntax</li>
  <li><b>Interpreted Language</b> – Code executes line by line</li>
  <li><b>High-Level Language</b> – No manual memory management</li>
  <li><b>Dynamically Typed</b> – No need to declare data types</li>
  <li><b>Object-Oriented</b> – Supports OOP concepts</li>
  <li><b>Platform Independent</b> – Runs on Windows, macOS, Linux</li>
  <li><b>Open Source</b> – Free and community-supported</li>
  <li><b>Rich Ecosystem</b> – Libraries for AI, ML, Web, Automation</li>
  <li><b>Scalable & Flexible</b> – Suitable for small scripts as well as large applications</li>
</ul>

<hr>

<h2>💻 Python Installation & Setup</h2>
<ol>
  <li>Download Python from <a href="https://www.python.org/" target="_blank">python.org</a></li>
  <li>Install Python and add it to PATH</li>
  <li>Verify installation:</li>
</ol>

<pre><code>python --version</code></pre>

<hr>

<h2>🧩 Basic Syntax</h2>
<p>
<ul>
  <li>Python uses simple and readable syntax, similar to the English language.</li>
  <li>Indentation is mandatory in Python and is used to define code blocks. where it replaces Curly braces {}. </li>
</ul>
</p>

<pre><code>
if 5 > 2:
    print("Five is greater than two!")
</code></pre>

<h1>💬 Comments</h1>
<p>Comments are used to <b>explain code</b> and are ignored by the Python interpreter. </p>
<ul>
  <li>Single-line comment → <code>#</code></li>
  <li>Multi-line comment → <code>'''</code> or <code>"""</code></li>
</ul>

<pre><code>
# This is a single-line comment
print("Hello, Python")
</code>
</pre>

<hr>

<h2>📦 Data Types and Variables</h2>
<p>
  <ul>
    <li>Data types in Python are the different kinds of values that tell Python what type of data a variable can store. </li>
    <li>There are main 3 data types: </li>
    <ul>
      <li> Integer (int) – holds any whole number</li>
      <li> Float (float) – holds decimal numbers </li>
      <li> String (str) – written anything in b/w quotes ( “  ” )  </li>
    </ul>
  </ul>
  </p>

<pre><code>
x = 5
print(type(x))
</code></pre>

<p><b>Variables:</b></p>
<ul>
  <li>Variables in Python are names used to store data values so that we can use and change them later in a program. </li>
</ul>

<pre><code>
x = 10
name = "Python"
print(x)
</code></pre>

<p><b>Rules to create variables:</b></p>
<ul>
  <li>A variable name must <b>start with a letter (a–z, A–Z) or an underscore (_).</b> </li>
  <li>A variable name <b>cannot start with a number. </b></li>
  <li>A variable name can contain <b>letters, numbers, and underscores only.</b> </li>
  <li>Variable names are <b>case-sensitive. </b></li>
  <li><b>Keywords </b>(reserved words) , <b>Punctuations</b> cannot be used as variable names.</li>
</ul>

<hr>

<h2>🔁 Type Conversions</h2>
<ul>
  <li>Type conversion means changing one data type into another data type.</li>
  <li>There are two types of type conversions in Python:</li>
</ul>

<p><b>Implicit Conversion:</b> Python automatically changes one data type into another.</p>
<pre><code>
a = 5
b = 2.5
c = a + b
</code>
</pre>

<p><b>Explicit Conversion:</b>The programmer changes the data type manually using functions.</p>
<p><b>Common conversion functions:</b></p>
<ul>
  <li>int() – converts to integer</li>
  <li>float() – converts to float</li>
  <li>str() – converts to string </li>
</ul>
  <pre><code>
x = "10"
y = int(x)
z = float(x)
</code></pre>

<hr>

<h2>🖨️ Print Condition</h2>
<p> <ul>
  <li>When we want to call a variable from the memory then we use print() condition. </li>
  <li>To create the relation with str and int , str and float inside the print() condition.</li>
  <li>We can create this in 4 different ways:</li>
  <ul>
    <li>Using Comma ( , ) where it will give us one tab space.</li>
    <pre><code>
      f = 27
      print( ‘ My name is Ajay & My age is ‘ , f)
    </code></pre>

 <li>Using “  + ” it will not give tab space and “  + ” will create the relation with string only.</li>
 <pre><code>
    f = 27
    print("My age is " + str(f))
</code></pre>
 <li>Using identifiers like %d – integer , %f – float , %s – string.  </li>
 <pre><code>
    f = 27
    print("My age is %d" % f)
 </code></pre>
 <li>Using f and { }.</li>
 <pre><code>
    f = 27
    print(f"My age is {f}")
   </code></pre>
</ul></ul>
</p>
<hr>

<h2>➗ Operators</h2>
<ul>
  <li>Arithmetic:<pre> + - * / % ** //</pre></li>
  <li>Relational:<pre> == != > < >= <=</pre></li>
  <li>Logical: <pre>and or not</pre></li>
  <li>Assignment:<pre> = += -= *=</pre></li>
  <li>Membership:<pre> in, not in</pre></li>
</ul>

<hr>

<h2>📚 Libraries</h2>
<p>Libraries in Python are collections of pre-written code that help us perform tasks easily without writing everything from scratch.</p>
<p><b> Common Python Libraries </b></p>
<ul>
  <li><b>NumPy</b>– Used for working with numbers and arrays</li>
  <li><b>Pandas</b>– Used for data analysis and handling tables</li>
  <li><b>Matplotlib</b>– Used for creating charts and graphs</li>
  <li><b>Seaborn</b>– Used for advanced data visualization</li>
  <li><b>Math</b>– Used for mathematical calculations</li>
</ul>

<pre><code>
import math
print(math.sqrt(16))
</code></pre>

<hr>

<h2>🔧 Functions</h2>
<p>A function is a block of code that performs a specific task and can be used again and again. </p>
<pre><code>
def add(a, b):
    return a + b
</code></pre>

<h3>Built-in Functions</h3>
<p>
  <li>Built-in functions are functions that are already available in Python. </li>
  <li>We can use them directly without creating them. </li>
</p>
<p>Common Built-in Functions </p> 
<ul>
  <li><b>print()</b>– Displays output</li>
  <li><b>input()</b>– Takes input from the user</li>
  <li><b>len()</b>– Finds length of data</li>
  <li><b>type()</b>– Finds data type</li>
  <li><b>sum()</b>– Adds values</li>
  <li><b>max()</b>– Finds maximum value</li>
  <li><b>min()</b>– Finds minimum value</li>
</ul>
<pre><code>                
  x = [1, 2, 3]
  print(len(x))
</code></pre>

<hr>

<h2>🧵 Strings</h2>
<p>
  <li>A string in Python is used to store text or characters. </li>
  <li>Strings are written inside single quotes (' '), double quotes (" "), or triple quotes (''' ''' or """ """). </li> </p>
<pre><code>
  name = "Python"
  message = 'Hello World'
</code></pre>
<p><b> Important Points About Strings</b></p>
<ul>
  <li>Strings are ordered (each character has a position). </li>
  <li>Strings are immutable, which means they cannot be changed after creation.</li>
  <li>Strings can contain letters, numbers, and symbols.</li>
</ul>

<p><b>Common String Operations </b></p>
<li><b>Concatenation (Joining strings)</b></li>
<pre><code>
  a = "Hello"
  b = "Python"
  print(a + "   " + b)    # Hello Python
</code></pre>
<li><b>Length of string </b></li>
<pre><code>
  text = "Python"
  print(len(text))     # 6
</code></pre>
<li><b>Indexing </b></li>
<pre><code>
  word = "Python"
  print(word[0])    # P
</code></pre>
<li><b>Slicing </b></li>
<pre><code>
 print(word[0:3])   #Pyt
</code></pre>
<p><b>Common String Functions</b> </p>
<ul>
  <li>upper() – Converts to uppercase </li>
  <li>lower() – Converts to lowercase </li>
  <li>strip() – Removes spaces</li>
  <li>replace() – Replaces characters</li>
  <li>split() – Splits string into parts</li>
</ul>

<hr>

<h2>📋 List</h2>
<p>
  <li>A list in Python is a data type used to store multiple values in a single variable. </li>
  <li> Lists are written using square brackets [ ].</li> </p>
  <pre><code>
    numbers = [1, 2, 3, 4]
    names = ["Alice", "Bob", "Charlie"]
  </code></pre>
  
  <p><b>Important Points About Lists </b></p>
  <ul>
    <li>Lists are ordered (each item has a position).</li>
    <li>Lists are mutable, which means values can be changed.</li>
    <li>Lists can store different data types. </li> </ul>
  <pre><code>
    my_list = [1, "Python", 3.5]
  </code></pre>  
  
  <p><b>Common List Operations</b></p>
  <li><b>Accessing elements</b></li>
  <pre><code>
  my_list = [1, "Python", 3.5]
  print(numbers[0])          # 1
  </code></pre>
  <li><b>Changing elements </b></li>
  <pre><code>
  numbers[1] = 10 
  </code></pre>
  <li><b>Adding elements </b></li>
  <pre><code>
  numbers.append(5)
  </code></pre>
  <li><b>Removing elements</b></li>
  <pre><code>
  numbers.remove(3) 
  </code></pre>
  <li><b>Length of list</b></li>
  <pre><code>
  print(len(numbers))
  </code></pre>

  <p><b>Common List Functions </b></p>
  <ul>
    <li><b>append()</b> – Adds an item</li>
    <li><b>insert()</b> – Adds item at a position</li>
    <li><b>remove()</b> – Removes an item</li>
    <li><b>pop()</b> – Removes last item </li>
    <li><b>sort()</b> – Sorts the list</li>
    <li><b>reverse()</b> – Reverses the list</li>
  </ul>

<hr>

<h2>📌 Tuple</h2>
<li>A tuple in Python is a data type used to store multiple values in a single variable. </li>
<li>Tuples are written using round brackets ( ).</li>
<pre><code>
numbers = (1, 2, 3, 4)
names = ("Alice", "Bob", "Charlie")
</code></pre>

<p><b>Important Points About Tuples</b></p>
<li>Tuples are ordered (each item has a position).</li>
<li>Tuples are immutable, which means values cannot be changed.</li>
<li>Tuples can store different data types.</li>

<p><b>Common Tuple Operations </b></p>
<li><b>Accessing elements</b></li>
<pre><code>
my_tuple = (1, "Python", 3.5) 
print(numbers[0])   # 1 
</code></pre>
<li><b>Length of tuple </b></li>
<pre><code>
print(len(numbers)) 
</code></pre>
<li><b>Looping through tuple</b></li>
<pre><code>
  for item in numbers:
      print(item)
</code></pre>

<p><b>Uses of Tuples</b></p>
<ul>
  <li>Faster than lists</li>
  <li>Used when data should not change</li>
  <li>Keeps data safe from modification</li></ul>

<hr>

<h2>🔢 Set</h2>
<li>A set in Python is a data type used to store multiple unique values in a single variable.</li>
<li>Sets are written using curly brackets { }. </li>
<pre><code>
numbers = {1, 2, 3, 4}
names = {"Alice", "Bob", "Charlie"}
</code></pre>

<p><b>Important Points About Sets</b></p>
<ul>
  <li>Sets store only unique values (no duplicates).</li>
  <li>Sets are unordered (no fixed position).</li>
  <li>Sets are mutable (can be changed).</li>
  <li>Sets do not allow indexing.</li>
</ul>

<p><b>Common Set Operations </b></p>
<li>Adding elements</li>
<pre><code>
numbers = {1, 2, 3, 4}
numbers.add(5)
</code></pre>
<li><b>Removing elements</b></li>
<pre><code>
  numbers.remove(2)
</code></pre>
<li><b>Union</b></li>
<pre><code>
  a = {1, 2, 3}
  b = {3, 4, 5}
  print(a | b)
</code></pre>
<li><b>Intersection </b></li>
<pre><code>
print(a & b)
</code></pre>

<p><b>Uses of Sets</b></p>
<ul>
  <li>To remove duplicate values</li>
  <li>To perform mathematical set operations</li>
  <li>To check membership quickly</li>
</ul>
<hr>

<h2>📖 Dictionary</h2>
<li>A dictionary in Python is a data type used to store data in key–value pairs.</li>
<li>Dictionaries are written using curly brackets { } with a key and value separated by a colon :. </li>
<pre><code>
  student = {
             "name": "Indhira",
              "age": 22,
              "course": "Python"
            }
</code></pre>

<p><b>Important Points About Dictionaries </b></p>
<ul>
  <li>Data is stored as key : value pairs.</li>
  <li>Keys are unique.</li>
  <li>Dictionaries are mutable (values can be changed).</li>
  <li>Values can be of any data type.</li>
</ul>

<p><b>Common Dictionary Operations</b></p>
<li><b>Accessing values</b></li>
<pre><code>
print(student["name"])
</code></pre>
<li><b>Adding or updating values</b></li>
<pre><code> 
student["grade"] = "A"
</code></pre>
<li><b>Removing values</b></li>
<pre><code> 
student.pop("age")
</code></pre>
<li><b>Getting all keys and values</b></li>
<pre><code>
print(student.keys())
print(student.values())
</code></pre>

<p><b>Uses of Dictionaries</b></p>
<ul>
  <li>To store related data together</li>
  <li>Fast data access using keys</li>
  <li>Useful for structured data</li>
</ul>
<hr>

<h2> Conclusion</h2>

<p>
This repository builds a strong foundation in Python by covering core concepts,
syntax, and essential data structures with practical examples. It is ideal for
beginners and freshers to develop problem-solving skills and progress toward
advanced Python applications.
</p>
<hr>
<h3>Contact</h3>

<p>Rongali Indhira
<br>email: indhirarongali123@gmial.com
<br>contact no.: +91 8096488064</p>
<hr>






