<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#comments'>Comments</a>
  </li>
  <li>
    <a href='#variable-assignment-and-initialization'>Variable Assignment and Initialization</a>
  </li>
  <li>
    <a href='#naming-and-using-variables'>Naming and Using Variables</a>
  </li>  
  <li>
    <a href='#whitespace-and-basic-formatting'>Whitespace and Basic Formatting</a>
  </li>
  <li>
    <a href='#introduction-to-literals-and-operators'>Introduction to Literals and Operators</a>
  </li> 
  <li>
    <a href='#atomic-data-types-and-type-conversion'>Atomic Data Types and Type Conversion</a>
  </li>
  <li>
    <a href='#avoiding-type-errors-with-the-str-function'>Avoiding Type Errors with the str Function</a>
  </li>   
  <li>
    <a href='#getting-user-input'>Getting User Input</a>
  </li>
  <li>
    <a href='constant-variables'>Constant Variables</a>
  </li>
  <li>
    <a href='#precision-handling'>Precision Handling</a>
  </li>   
  <li>
    <a href='#escape-sequences'>Escape Sequences</a>
  </li> 
  <li>
    <a href='#arithmetic-operators'>Arithmetic Operators</a>
  </li>  
  <li>
    <a href='#shorthand-assignment-operators'>Shorthand Assignment Operators</a>
  </li>      
</ol>
</details>
   

## Comments
<ul>
  <li>
    <a><em>Comments</em> are notes created by the programmer that are included within the program. The compiler ignores these comments as they are only there for the programmer's use</a>
  </li>
  <li>
    <a>In Python, there are two styles of comments:</a>
    <ul>
      <li>
        <a><em>Single-line comments</em></span>: are denoted with the hash mark, #, and tell the compiler to ignore all code from the hash mark to the end of the line of code</a>
      </li>
      <details>
      <summary>Example Program</summary>
        <ul>
          <pre>
            <code>
              print("Hello!") #This is a comment
            </code>
          </pre>    
          <details>
          <summary>Output</summary>
            <pre>
              <code>
                Hello!
              </code>
            </pre>  
          </details>
        </ul>  
      </details>
      <li>
        <a><em>Multi-line comments</em>: are denoted by the """ set of characters. Everything that is enclosed within the """ and """ set of characters is a comment and therefore ignored by the compiler</a>
      </li>  
      <details>
      <summary>Example Program</summary>
        <ul>
          <pre>
            <code>
              """
              This is a multi-line comment
              This line will be ignored
              And so will this line
              """
              print("Hello")
            </code>
          </pre>  
          <details>
          <summary>Output</summary>
            <pre>
              <code>
                Hello
              </code>
            </pre>  
          </details>
        </ul>  
      </details>
    </ul>
  </li> 
  <li>
    <a>Multi-line comments can be comprised of multiple single-line comments; however, multi-line comments cannot be embedded with any multi-line comments</a>
  </li>       
  <li>
    <a>Comments are useful to explain what certain lines and blocks of code do, especially when other programmers are reading the code</a>
  </li>  
</ul> 

## Variable Assignment and Initialization
<ul>
  <li>
    <a>A <em>variable</em> is a name given to an instance of a data type not defined by the user. The name of this instance is also called an <em>identifier</em>. Variables and identifiers are two words that mean the exact same thing</a>
  </li>
  <li>
    <a><em>Initialization</em> is the process in which a variable is assigned a memory address</a>
  </li>
  <li>
    <a>After a variable has been defined, it can be assigned a value using the <em>assignment operator</em>. The assignment operator is the equals sign character, =. The process of a variable being initialized is called <em>assignment</em>. Assignment and initialization are two words that mean the same thing</a>
  </li>
  <ul>
    <li>
      <a>variable = "literal" #literal on the right side of the assignment operator is assigned to the variable on the left side of the assignment operator</a>
    </li>
  </ul>              
  <li>
    <a>An <em>initializer</em> is the information, whether that be a literal or another variable, that is used to initialize a variable</a>
  </li>
</ul>  

## Naming and Using Variables
<ul>
  <li>
    <a>There are a few rules that need to be adhered to when initializing variables within Python:<a>
    <ul>
      <li>
        <a>Variable names can only contain the following: letters, numbers, and underscores.  Variable names can start with letters and underscores, but not numbers</a>
      </li>
      <li>
        <a>Python does not allow spaces within any portion of a variable's name</a>
      </li>
      <li>
        <a>A good practice is to avoid using keywords and function names as variable names</a>
      </li>
    </ul>  
  </li>
</ul>   

## Whitespace and Basic Formatting
<ul>
  <li>
    <a><em>Whitespace</em> is a term that refers to characters that are used for formatting purposes; in Python, this refers primarily to spaces, tabs, and newlines</a>
  </li>  
  <li>
    <a>The Python compiler generally ignores whitespaces; however, there are a few exceptions to this rule:</a>
    <ul>
      <li>
        <a>One exception where the Python compiler does not pay attention to whitespace is inside quoted text</a>
      </li>
      <li>
        <a>Python uses spaces to define code blocks, such as within classes, functions, loops, etc.</a>
      </li>  
    </ul>    
  </li>  
  <li>
    <a>Variable names cannot contain whitespaces</a>
  </li> 
</ul>

## Introduction to Literals and Operators
<ul>
  <li>
    <a><em>Literals</em> are fixed values that have been inserted directly into the source code</a>
    <ul>
      <li>
        <a>Examples of literals are 1, 2.5, "garrett", and 'c'. These are literals because you cannot assign different values to those terms</a>
      </li>
    </ul>
  </li>
  <li>
    <a><em>Operators</em> are symbols that perform operations on variables and values</a>
    <ul>
      <li>
        <a>Operators can be chained together; the output of one operation can be used as the input for another operator</a>
      </li>
    </ul>
  </li>
</ul>

## Atomic Data Types and Type Conversion
<ul>
  <li>
    <a>Objects that are <em>mutable</em> can have their contents altered after their initializations. Mutable objects are like writing in pencil; the content that the pencil produces can be erased</a>
  </li>
  <ul>
    <li>
      <a>Here is a list of common mutable objects: lists, dictionaries, sets, and user-defined classes</a>
    </li>  
  </ul>  
  <li>
    <a>Objects that are <em>immutable</em> cannot have their contents altered after their initializations. Immutable objects are like writing in Sharpie; the content that the Sharpie produces cannot be erased and is there forever. The only way to change the contents of an immutable object is to reinitialize the object with a different value</a>
  </li>  
  <ul>
    <li>
      <a>Here is a list of common immutable objects: ints, floats, bools, strings, and tuples</a>
    </li>
  </ul>    
  <li>
    <a>Numeric types:</a>
    <ul>
      <li>
        <a><em>int</em>: used to store an integer</a>
      </li>
      <li>
        <a><em>float</em>: used to store a decimal number</a>
      </li>
      <li>
        <a><em>complex</em>: used to store a complex number</a> 
      </li>
      <details>
      <summary>Example Program</summary>
        <ul>
          <pre>
            <code>
              x = 1        # int
              y = 12.1     # float
              z = 1 + 45j  # complex
              <br />
              print(z)
            </code>
          </pre>    
          <details>
          <summary>Output</summary>
            <pre>
              <code>
                (1+45j)
              </code>
            </pre>  
          </details>
        </ul>  
      </details>   
    </ul>
  </li>
  <li>
    <a><em>bool</em>: has two possible values and stores one of the following: True or False</a>
  </li>
  <li>
    <a><em>str</em>: used to store a list of characters or a single character</a>
    <ul>
      <li>
        <a>A string is simply a series of characters.  In Python, you can put single or double quotes around any set of characters and Python will consider this text as a string</a>
      </li>
      <li>
        <a>Two examples of a string are the following: "Hello this is a string!" and 'Hello this is a string!'</a>
      </li>  
    </ul>      
  </li> 
  <li>
    <a>Sequence types:</a>
    <ul>
      <li>
        <a><em>list</em>: more information on lists can be found </a><a href="https://github.com/Programming-Notes-all-languages/Python-Notes/tree/main/Procedural%20Programming/Variables%20and%20Simple%20Data%20Types">here</a>
      </li>
      <li>
        <a><em>tuple</em>: more information on tuples can be found </a><a href="https://github.com/Programming-Notes-all-languages/Python-Notes/tree/main/Procedural%20Programming/Variables%20and%20Simple%20Data%20Types">here</a>
      </li>
      <li>
        <a><em>dictionary</em>: more information on dictionaries can be found </a><a href="https://github.com/Programming-Notes-all-languages/Python-Notes/tree/main/Procedural%20Programming/Dictionaries">here</a> 
      </li>  
    </ul>    
  <li>
    <a>Type conversion:</a>
    <ul>
      <li>
        <a>Can use variable = dataType(variable) to change the variable's type to dataType</a>
      </li>
      <li>
        <details>
        <summary>Example Program</summary>
          <ul>
            <pre>
              <code>
                number = 55
                strNumber = str(55)
                <br />
                print("The string value of " + str(number) + " is " + strNumber)
              </code>
            </pre>  
            <details>
            <summary>Output</summary>
              <pre>
                <code>
                  The string value of 55 is 55
                </code>
              </pre>  
            </details>
          </ul>  
        </details>
      </li>  
    </ul>
  </li>                 
</ul>    

## Avoiding Type Errors with the str Function
<ul>
  <li>
    <a>Type errors indicate that Python cannot recognize some type of information. An example of this is in Python's print() function which only works when all of the contents embedded within the function are of the same data type</a>
  </li>
  <li>
    <a>For example, let's say a program tries to print the following using the print() function: "Happy " + age + "rd Birthday!". Let's also say that age is a variable of type int, storing the integer three. Here, Python does not know if the variable age should represent the integer value three, or if age should represent the string three. Because of this, uncertainty, Python throws out an error when the program runs</a>
  </li>  
  <ul>
    <li>
      <a>To fix this error, the conversion of age from a variable of type int to a variable of type str is necessary. print("Happy " + str(age) + "rd Birthday!") now works as intended and the compiler prints the following message to the screen: Happy 3rd birthday!
    </li>
    <li> 
      <a>what this str() function does above is that it temporarily changes the variable type of age from an integer to a variable of type string. After this line of code, the age's variable type returns to int. To permanently change age's variable type to str, the following line of code can be written: age = str(age)</a>
    </li>
  </ul>    
</ul>  

## Getting User Input
<ul>
  <li>
    <a>To get user input, you need to use the input() function which is already pre-defined by Python</a>
  </li>
  <li>
    <a>For example, let's say that we want the user to enter a message into the terminal and then we were to store this message into a variable called message. This could be accomplished by doing the following: message = input("Enter in a message: "). It is important to note that the variable message will store a string</a>
  </li>
  <li>
    <a>If you would like to get an input and store that input into a variable of a type other than string, then you could do the following: value = int(input("Enter in a message: ")). Now, instead of the variable value being initialized as a variable of type string, the variable is of type integer</a>
  </li>
</ul>

## Constant Variables
<ul>
  <li>
    <a>A constant variable is a variable value that cannot be changed throughout the compilation of the program. To do this, create a separate Python file which can be called anything, but is conventionally called constant.py. In this file, declare and initialize the variables and in the main.py file, insert import constant at the beginning of the program. Now, those variables that you assigned in constant.py can be accessed in main.py and their values cannot be changed</a>
  </li>
</ul>

## Precision Handling
<ul>
  <li>
    <a>The format() function is used to change the number of decimal places that a variable contains temporarily</a>
  </li>
  <li>
    <a>The format() function takes in either a literal or an identifier and rounds that value to the number of decimal spaces defined following conventional rounding conventions</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          #variable assignment
          a = 1234.56
          <br />
          #printing out rounded a, accurate to the tenths place
          print("{:.1f}".format(1.3434))
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            1.3
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
</ul> 

## Escape Sequences
<ul>
  <li>
    <a>The backslash \ is the indicator of an escape sequence</a>
  </li>
  <li>
    <a>Some of the common escape sequences are listed below:</a>
    <ul>
      <li>
        <a>\n: newline</a>
      </li>
      <li>
        <a>\t: tab</a>
      </li>
    </ul>
  </li>
</ul>

## Arithmetic Operators
<ul>
  <li>
    <a><em>Addition operator</em>: adds the value on the left-hand side of the operator to the value on the right-hand side of the operator</a>
    <ul>
      <li>
        <a>x + y #sums the values x and y</a>
      </li>
    </ul>    
  </li>
  <li>
    <a><em>Subtraction operator</em>: subtracts the value on the right-hand side of the operator from the value on the left-hand side of the operator</a> 
    <ul>
      <li>
        <a>x - y #subtracts the value y from the value x</a>
      </li>
    </ul>    
  </li>
  <li>
    <a><em>Multiplication operator</em>: multiplies the value on the right-hand side of the operator to the value on the left-hand side of the operator</a>
    <ul>
      <li>
        <a>x * y #multiplies the values x and y</a>
      </li>
    </ul>    
  </li>
  <li>
    <a><em>Division operator</em>: divides the value on the left-hand side of the operator by the value on the right-hand side of the operator</a>
    <ul>
      <li>
        <a>x / y #divides the x value by the value y</a>
      </li>
    </ul>    
  </li>
  <li>
    <a><em>Modulus operator</em>: divides the value on the left-hand side of the operator by the value on the right-hand side of the operator and returns the remainder</a>
    <ul>
      <li>
        <a>x % y #finds the remainder of the value x divided by value y</a>
      </li>
    </ul>     
  </li>
  <li>
    <a><em>Exponentiation operator</em>: raises the value on the left-hand side of the operator to the value on the right-hand side of the operator</a>
    <ul>
      <li>
        <a>x ** y #finds the value of x raised to the value y</a>
      </li>
    </ul>    
  </li>
  <li>
    <a><em>Floor division</em>: divides the value on the left-hand side of the operator by the value on the right-hand side of the operator and returns that value to rounded down to the nearest integer</a>
    <ul>
      <li>
        <a>x // y #finds the value of x divided by y rounded down to the nearest integer</a>
      </li>
    </ul>    
  </li>  
</ul>   

## Shorthand Assignment Operators
<ul>
  <li>
    <a><em>Addition assignment operator</em>: adds the value on the right-hand side of the operator to the value on the left-hand side and stores the summation in the variable on the left-hand side of the operator</a>
    <ul>
      <li>
        <a>x += y #means x equals the sum of x and y</a>
      </li>
      <li>
        <a>--> x = x + y</a>
      </li>  
    </ul>
  </li>
  <li>
    <a><em>Subtraction assignment operator</em>: subtracts the value on the right-hand side of the operator from the value on the left-hand side and stores the subtraction in the variable on the left-hand side of the operator</a>
    <ul>
      <li>
        <a>x -= y #means x equals the subtraction of y from x</a>
      </li>
      <li>
        <a>--> x = x - y</a>
      </li> 
    </ul>
  </li>
  <li>
    <a><em>Multiplication assignment operator</em>: multiplies the value on the right-hand side of the operator to the value on the left-hand side and stores the product in the variable on the left-hand side of the operator</a>
    <ul>
      <li>
        <a>x *= y #means x equals the product of x and y</a>
      </li>
      <li>
        <a>--> x = x * y</a>
      </li> 
    </ul>
  </li>
  <li>
    <a><em>Division assignment operator</em>: divides the value on the left-hand side of the operator to the value on the left-hand side of the operator and stores the division in the variable on the left-hand side of the operator</a>
    <ul>
      <li>
        <a>x /= y #means x equals x divided by y</a>
      </li>
      <li>
        <a>--> x = x / y</a>
      </li> 
    </ul>
  </li>
  <li>
    <a><em>Modulo assignment operator</em>: finds the remainder of the value on the left-hand side of the operator divided by the value on the right-hand side and stores the remainder in the variable on the left-hand side of the operator</a>
    <ul>
      <li>
        <a>x %= y #means x equals the remainder of x divided by y</a>
      </li>
      <li>
        <a>--> x = x % y</a>
      </li> 
    </ul>
  </li>  
  <li>
    <a><em>Exponentiation assignment operator</em>: raises the value on the left-hand side of the operator to the value on the right-hand side of the operator and stores that value in the variable on the left-hand side of the operator</a>  
    <ul>
      <li>
        <a>x **= y #means x equals the x raised to the y</a>
      </li>
      <li>
        <a>--> x = x ** y</a>
      </li> 
    </ul>                 
  </li> 
  <li>
    <a><em>Floor division assignment operator</em>: divides the value on the left-hand side of the operator by the value on the right-hand side of the operator and stores the division rounded down to the nearest integer to the variable on the left-hand side of the operator</a>
    <ul>
      <li>
        <a>x //= y #means x equals the floor division of x divided by y</a>
      </li>
      <li>
        <a>--> x = x // y</a>
      </li> 
    </ul>
  </li>  
</ul>
