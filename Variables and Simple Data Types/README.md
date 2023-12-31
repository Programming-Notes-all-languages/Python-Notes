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
    <a href='#changing-case-in-a-string-with-methods'>Changing Case in a String with Methods</a>
  </li> 
  <li>
    <a href='#combining-or-concatenating-strings'>Combining or Concatenating Strings</a>
  </li>
  <li>
    <a href='#adding/stripping-whitespace-to-strings-with-tabs-or-newlines'>Adding/Stripping Whitespace to Strings with Tabs or Newlines</a>
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
    <a href='#avoiding-type-errors-with-the-str()-function'>Avoiding Type Errors with the str() Function</a>
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
</ol>
</details>

## Variables
<ul>
  <li>
    <a>A <em>variable</em> is a container stored in memory that holds a value that a user can define</a>
  </li>
  <li>
    <a>Here is an example of a variable declaration and initialization: message = "Hello Python World!</a>
      <ul>
        <li>
          <a>If you would like to print message's contents to the terminal, you would do the following: print(message)</a>
        </li>
        <li>
          <a>The output of this code would be the following: Hello Python World!</a>
        </li>
      </ul>
    </a>
  </li>
  <li>
    <a>A variable's value can be changed at any point in your program.  The variable's new declaration can happen anywhere and Python will always update the variable's new value</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          message = "hello world"        
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
            hello
          </code>
        </pre>     
      </details>
    </ul>  
  </details>
</ul>  

## Naming and Using Variables
<ul>
  <li>
    <a>There are a few rules that need to be adhered to when initializing variables within Python:<a>
    <ul>
      <li>
        <a>Variable name can only contain the following: letters, numbers, and underscores.  Variable names can start with letters and underscores, but not numbers</a>
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

## Strings
<ul>
  <li>
    <a>A string is simply a series of characters.  In Python, you can put single or double quotes around any set of characters and Python will consider this text as a string</a>
  </li>
  <li>
    <a>Two examples of a string are the following: "Hello this is a string!" and 'Hello this is a string!'</a>
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

## Adding/Stripping Whitespace to Strings with Tabs or Newlines
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

## Integers
<ul>
  <li>
    <a>You can do the following operations on integers in python: add (+), subtract (-), multiply (*), divide (/), and modulo (%)</a>
  </li>
  <li>
    <a>Python uses two multiplication symbols to represent exponents</a>
  </li>  
  <ul>
    <li>
      <a>For example, let's say that we have the following declaration for value, value = 3**3. value is equal to 27</a>
    </li>
  </ul>
</ul> 

## Floats
<ul>
  <li>
    <a>Python calls any number that has a decimal point a variable of type float</a>
  </li>
  <li>
    <a>For the most part, Python is not as sensitive with decimals like other programming languages like C++</a>
  </li>
  <li>
    <a>For example, let's say that we have the following declaration for a variable named value, value =  0.1 + 0.2.  The value of the variable value is now equal to 0.3</a> 
  </li>
</ul>

## Boolean
<ul>
  <li>
    <a>A boolean variable is a variable that is either True or False</a>
  </li>
  <li>
    <a>For example, let's say that we have the following declaration for a variable named value, value = True.  The variable value is of type boolean and is equal to True</a>
  </li>  
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

## Avoiding Type Errors with the str() Function
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

## Comments
<ul>
  <li>
    <a>In Python, the hash mark (#) is a character that indicates to the compiler that this line of code is a single line comment.  Anything followed by the hash mark is ignored by the Python compiler</a>
  </li>
  <li>
    <a>The reason for writing comments is to explain to the person reading your code what your code is supposed to do</a>
  </li>
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
