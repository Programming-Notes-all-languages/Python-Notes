<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#variables'>Variables</a>
  </li>
  <li>
    <a href='#naming-and-using-variables'>Naming and Using Variables</a>
  </li>
  <li>
    <a href='#strings'>Strings</a>
  </li>  
  <li>
    <a href='#arithmetic-operators'>Arithmetic Operators</a>
  </li>
  <li>
    <a href='#changing-case-in-a-string-with-methods'>Changing Case in a String with Methods</a>
  </li> 
  <li>
    <a href='#combining-or-concatenating-strings'>Combining or Concatenating Strings</a>
  </li>
  <li>
    <a href='#adding-and-stripping-whitespace-to-strings-with-tabs-or-newlines'>Adding and Stripping Whitespace to Strings with Tabs or Newlines</a>
  </li>   
  <li>
    <a href='#integers'>Integers</a>
  </li>
  <li>
    <a href='floats'>Floats</a>
  </li>
  <li>
    <a href='#boolean'>Boolean</a>
  </li>
  <li>
    <a href='#modulo-operator'>Modulo Operator</a>
  </li>
  <li>
    <a href='#avoiding-type-errors-with-the-str-function'>Avoiding Type Errors with the str Function</a>
  </li> 
  <li>
    <a href='#comments'>Comments</a>
  </li>   
  <li>
    <a href='#getting-user-input'>Getting User Input</a>
  </li>
  <li>
    <a href='#constant-variables'>Constant Variables</a>
  </li>
  <li>
    <a href='precision-handling'>Precision Handling</a>
  </li>    
  <li>
    <a href='#mutable-and-immutable-objects'>Mutable and Immutable Objects</a>
  </li>            
</ol>
</details>
   

## Comments
<ul>
  <li>
    <a><em>Comments</em> are notes created by the programmer that are included within the program. The compiler ignores these comments as they are only there for the programmer's use</a>
  </li>
  <li>
    <a>In Python there are two styles of comments:</a>
    <ul>
      <li>
        <a><em>Single-line comments</em></span>: are denoted with the hash mark, #, and tells the compiler to ignore all code from the hash mark to the end of the line of code</a>
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
    <a>Objects that are <em>mutable</em> can have their contents altered after their initializations.  Mutable objects are like writing in pencil; the content that the pencil produces can be erased</a>
  </li>
  <ul>
    <li>
      <a>Here is a list of common mutable objects: lists, dictionaries, sets, and user-defined classes</a>
    </li>  
  </ul>  
  <li>
    <a>Objects that are <em>immutable</em> cannot have their contents altered after their initializations.  Immutable objects are like writing in Sharpie; the content that the Sharpie produces cannot be erased and is there forever.  The only way change the contents of an immutable object is to reinitialize the object with a different value</a>
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
        <a><em>list</em>: more information on lists can be found [here](https://github.com/Programming-Notes-all-languages/Python-Notes/tree/main/Procedural%20Programming/Introducing%20Lists)</a>
      </li>
    </ul>    
  <li>
    <a>SMALLEST --- char << int << float << double --- GREATEST</a> 
    <ul>
      <li>
        <a>One can store a smaller data type in a larger data type. For example, you can store an int in a float or a double</a>
      </li>
    </ul>     
  </li>  
  <li>
    <a>Type conversion:</a>
    <ul>
      <li>
        <a>Can use variable = dataType(variable); to change the variable's type to dataType</a>
      </li>
      <li>
        <a>Can also use variable = static_cast</a><a><</a><a>dataType</a><a>></a><a>; to change variable type to dataType</a>
      </li>
      <li>
        <a>Converting any char into another type returns that value's ASCII value</a>
      </li>  
      <li>
        <a>Examples of type conversion:</a>
        <details>
        <summary>Example Program</summary>
          <ul>
            <pre>
              <code>
                #include <iostream>
                using namespace std;
                <br />
                int main()
                {
                &emsp;&emsp;double x = 1.1, y = 7.2;
                &emsp;&emsp;x = int(x);
                <br />
                &emsp;&emsp;cout << "The value of x is: " << x << '\n';
                &emsp;&emsp;y = static_cast<int>(y);
                &emsp;&emsp;cout << "The value of y is: " << y << '\n';
                <br />
                &emsp;&emsp;return 0;
                }
              </code>
            </pre>  
            <details>
            <summary>Output</summary>
              <pre>
                <code>
                  The value of x is: 1
                  The value of y is: 7
                </code>
              </pre>  
            </details>
          </ul>  
        </details>
      </li>  
    </ul>
  </li>                 
</ul>

## Changing Case in a String with Methods
<ul>
  <li>
    <a>One of the most simple things one can do with a string is to change the case of some or all of the characters within the string</a>
  </li>
  <li>
    <a>A <em>method</em> is an action that Python takes upon itself to perform a task.  The dot operator, simply a dot (.), that is placed after a variable name tells Python to make the method following the dot to act on the variable preceding the dot</a>  
    <ul>
      <li>
        <a>Every method is followed by an opened and a closed parenthesis set such as the following: name.title()</a>
      </li>
    </ul>
  <li>
    <a>The title() method changes a string so that each character following a white space is uppercase</a>
  </li>  
  <li>
    <a>The lower() method changes every character within the string preceding the dot to be lowercase</a>
  </li>
  <li>
    <a>The upper() method changes every character within the string preceding the dot to be uppercase</a>  
  </li>      
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          message = "hello world"
          print(message)
          message = message.upper()
          print(message)
          message = "hello"
          print(message)
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
          hello world
          HELLO WORLD
          hello
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
  <li>
    <a>To tell Python to not start with a new line after using a print statement, you can do the following: print(variable/string, end = "x")</a>
    <ul>
      <li>
        <a>In this example, we are printing a string or a variable to a string.  Instead of the compiler printing the code beneath this statement on a new line, we tell the compiler to print the statements underneath this statements based on what x is</a> 
      </li> 
      <li> 
        <a>x is a string that can be anything you would like it to be</a>
      </li> 
    </ul>   
  </li> 
  <li>
    <a>Various string constants are made available in Python within the string library.  To add this library, simply add this line of code to your program: import string</a>
  </li>
  <li>
    <a>Here are a few pre-initialized strings that are made available by the string library in Python:</a>
  </li>  
  <ul>
    <li>
      <a>string.ascii_lowercase: is the following string: "abcdefghijklmnopqrstuvwxyz"</a>
    </li> 
    <li>
      <a>string.ascii.uppercase: is the following string: "ABCDEFGHIJKLMNOPQRSTUVWXYZ"</a>
    </li>  
    <li>
      <a>string.ascii.letters: is the concatenation of string.ascii_lowercase and string.ascii_uppercase</a>
    </li>
    <li>
      <a>string.digits: is the following string: "0123456789"</a>
    </li>
    <li>
      <a>string.punctuation is the following string: "!"#$%&'()*+,-./:;<=>?@[\]^_`{|}~"</a> 
    </li>  
  </ul>
</ul>   

## Combining or Concatenating Strings
<ul>
  <li>
    <a>Python uses the plus symbol to combine strings</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          firstName = "Garrett"<br />
          lastName = "Ellis"</br />
	        fullName = firstName + " " + lastName<br />
          print(fullName)<br />
        </code>
      </pre> 
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            Garrett Ellis
          </code>
        </pre>     
      </details>
    </ul>  
  </details> 
</ul>    

## Adding and Stripping Whitespace to Strings with Tabs or Newlines
<ul>
  <li>
    <a>In programming, whitespace refers to a singular character or a string of characters that represent space.  Whitespace characters are not visibly marked, but they do take up space and memory</a>
  </li>
  <li>
    <a>To add a tab to your text, use \t</a>
  </li>
  <li>
    <a>To add a newline to a string, use \n</a>
  </li>      
  <li>
    <a>Python has methods that can look for extra whitespace characters at the beginning and the end of a string and will remove those characters.  Here are the three methods:</a>
  </li>
  <ul>
    <li>
      <a>To make sure that no whitespace characters exists on the right end of a string, use the rstrip() method</a>  
    </li>  
    <li>
      <a>To make sure that no whitespace characters exists on the left end of a string, use the lstrip() method</a>
    </li>  
    <li>
      <a>To strip any and all whitespace characters from the left and right ends of a string, use the strip() method</a>
    </li>  
  </ul>  
</ul>  

## Modulo Operator
<ul>
  <li>
    <a>A useful tool for working with numerical information is the <em>modulo operator</em></a>
  </li>
  <li>
    <a>The modulo operator is a tool that is used to find the remainder producing by dividing one number by another number</a>
  </li>
  <li>
    <a>For example, let's say that we have the following declaration for a variable named value, value = 4 % 3.  The variable called value is equal to one, because four divided by three has a remainder of one</a> 
  </li>
</ul>       

## Avoiding Type Errors with the str Function
<ul>
  <li>
    <a>Type errors indicate that Python cannot recognize the kind of information that you are using</a>
  </li>
  <li>
    <a>For example, let's say you have the following line of code in your program: message = "Happy " + age + "rd Birthday!".  Let's also say that age is a variable of type integer which holds the value three.  Here, Python does not know if the variable age should represent the integer value three, or if age should represent the string three.  Because of this, uncertainty, Python throws an error at us when the program is run</a>
  </li>  
  <ul>
    <li>
      <a>To fix this error, you can wrap the age variable in the str() function.  You would then write the following line of code: message = "Happy " + str(age) + "rd Birthday!", and you would get the expected output: Happy 3rd birthday!
    </li>
    <li> 
      <a>what this str() function does above is that it temporarily changes the variable type of age from an integer to a variable of type string</a>
    </li>
  </ul>    
</ul>  

## Getting User Input
<ul>
  <li>
    <a>To get user input, you need to use the input() function which is already pre-defined by Python</a>
  </li>
  <li>
    <a>For example, let's say that we want the user to enter a message into the terminal and then we were to store this message into a variable called message.  This could be accomplished by doing the following: message = input("Enter in a message: ").  It is important to note that the variable message will store a string</a>
  </li>
  <li>
    <a>If you would like to get an input and store that input into a variable of a type other than string, then you could do the following: value = int(input("Enter in a message: ")).  Now, instead of the variable value being initialized as a variable of type string, now the variable is of type integer</a>
  </li>
</ul>

## Constant Variables
<ul>
  <li>
    <a>A constant variable is a variable value which cannot be changed throughout the compilation of the program.  To do this, create a separate Python file which can be called anything, but is conventionally called constant.py.  In this file, declare and initialize the variables and in the main.py file, insert import constant at the beginning of the program.  Now, those variables that you declared in constant.py can be accessed in main.py, and their values cannot be changed</a>
  </li>
</ul>

## Precision Handling
<ul>
  <li>
    <a>The format() function is used to change the number of decimal places that a variable contains temporarily</a>
  </li>
  <li>
    <a>For example, let's say that we have the following variable of type double declared, value = 0.349857.  To change the number of decimal places to, let's say, to be accurate to the hundreds place, we could use the format() function.  This function will also round this number to the specified number of decimal places.  This line of code will change the value of value to what we had previously specified: value = float"{:.2f}".format(value)</a>
  </li>
</ul> 
