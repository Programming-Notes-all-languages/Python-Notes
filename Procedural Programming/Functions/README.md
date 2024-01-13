<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#defining-a-function'>Defining a Function</a>
  </li>
  <li>
    <a href='#passing-arguments'>Passing Arguments</a>
  </li>
  <li>
    <a href='#positional-arguments'>Positional Arguments</a>
  </li>  
  <li>
    <a href='#keyword-arguments'>Keyword Arguments</a>
  </li> 
  <li>
    <a href='#default-values'>Default Values</a>
  </li>
  <li>
    <a href='#return-values'>Return Values</a>
  </li> 
  <li>
    <a href='#returning-a-dictionary'>Returning a Dictionary</a>
  </li>    
  <li>
    <a href='#passing-a-list'>Passing a List</a>
  </li>  
  <li>
    <a href='#passing-an-arbitrary-number-of-arguments'>Passing an Arbitrary Number of Arguments</a>
  </li> 
  <li>
    <a href='#using-arbitrary-keyword-arguments'>Using Arbitrary Keyword Arguments</a>
  </li> 
  <li>
    <a href='#storing-your-functions-in-modules'>Storing your Functions in Modules</a>
  </li>   
  <li>
    <a href='#random-number-generation'>Random Number Generation</a>
  </li>                
</ol>
</details>

## Defining a Function
<ul>
  <li>
    <a>The code below is a simple program that contains a function named hello():</a>
    <details>
    <summary>Example Program</summary>
      <ul>
        <pre>
          <code>
            def hello():<br />
	            """Display a simple greeting."""<br />
	            print("Hello!")<br />
            hello()<br />
          </code>
        </pre>  
        <details>
        <summary>Output</summary>
          <pre>
            <code>
              Hello!<br />
            </code>
          </pre>  
        </details>
      </ul>  
    </details>
    <ul>
      <li>
        <a>This program above is a complete function, despite its simplicity.  In the first line of the program, there is the keyword <em>def</em> which informs Python that you are about to define a function.  This is the first part of the <em>function's definition</em>.  A function definition contains the name of the function, a parameter list, and code which is what the function's job is</a>
      </li> 
      <li>
        <a>In the example above, an indented line follows the def hello():.  This code consists of the <em>body</em> of the function</a>
      </li>
      <li>
        <a>the line directly below def hello(): which is enclosed in three sets of quotation marks is called a <em>docstring</em>.  A docstring is a short summary describing what the function does</a>  
      </li>  
      <li>
        <a>Once a function is defined, it then needs to be called in order for the function to be used during compilation.  A <em>function call</em> tells Python that a specified function is intended on being used.  In order to call a function, you write the name of the function, followed by a set of parentheses.  Inside the parentheses goes the list of arguments, if the function has any</a>
      </li>  
    </ul> 
  </li> 
  <li>
    <a>Here is another example of a simple function; however, this time the function hello() takes in a single argument as a parameter</a> 
  </li> 
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          def hello(name):<br />
              """Display a simple greeting."""<br />
              print("Hello! " + name)<br />
              hello("Garrett")<br />
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            Hello Garrett!<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details> 
    <ul>
      <li>
        <a>The variable name in the function above called hello() is called a <em>parameter</em>.  A parameter is a piece of information that is given to a function to help the function do its desired job.  The information that is passed to the function during the function's call is called an <em>argument</em>.  In the example above, Garrett is the function's argument, which gets passed in as the value for the variable name within the function definition</a> 
      </li>  
    </ul>  
  </li>      
</ul>

## Passing Arguments
<ul>
  <li>
    <a>In a more complicated function definition, a function will have multiple parameters.  When this is the case, the call to the function will then too have multiple arguments</a>
  </li>
  <li>
    <a>You can call a function an infinite number of times</a>
  </li>
  <li>
    <a>You can use <em>positional arguments</em>, meaning that the order of the arguments in the function's call must match the order of the function's parameter list.  You can also use <em>keyword arguments</em>, where the arguments are written in the function call with the parameter's name assigned to it via the assignment operator</a>
  </li>   
</ul>

## Positional Arguments
<ul>
  <li>
    <a>When calling a function within Python, an argument must be matched with a parameter in order to get no errors.  The easiest way to do this is to write the arguments in the order in which the parameters are written in the function's definition</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          def hello(name, age):<br />
	          """Display a simple greeting."""<br />
	          print("Hello! " + name + "\nYour age: " + str(age))<br />
          hello("Garrett", 20)<br />
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            Hello! Garrett<br />
            Your age: 20<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details> 
</ul>    

## Keyword Arguments
<ul>
  <li>
    <a>Keyword arguments enable the user to enter the arguments in any order in the function's call</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          def hello(name, age):
	          """Display a simple greeting."""
	          print("Hello! " + name + "\nYour age: " + str(age))
          hello(name = "Garrett", age = 20)
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            Hello! Garrett<br />
            Your age: 20<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details> 
  <ul>
    <li>
      <a>The program's output above is identical to the output of the program in the section called positional arguments.  The only difference between both program's is that this program utilizes keyword arguments and the previous program uses positional arguments.  In this program, the variables name and age could have been switched in the function's call, and the output of the program would have still been identical</a>
    </li>
  </ul>  
</ul>   

## Default Values
<ul>
  <li>
    <a>When writing a function's definition, you can give a parameter a <em>default value</em>.  When you have a parameter with a default value, if an argument is not passed for that parameter, then the default value will be initialized for the parameter throughout the duration of the function; otherwise, the value of the argument passed into the parameter will override the default value</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          def hello(name, age = 0):
	          """Display a simple greeting."""
	          print("Hello! " + name + "\nYour age: " + str(age))
          hello(name = "Garrett")
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            Hello! Garrett<br />
            Your age: 0<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details> 
  <ul>
    <li>
      <a>Since there is no argument passed into the parameter age in the function above, the default value of age, which is zero, is then the value to which age is initialized to</a>
    </li>
  </ul>    
</ul>  

## Return Values
<ul>
  <li>
    <a>A function does not always have to print things out to the screen; instead, it can just calculate a value or set of values and return that value or those values.  A <em>return value</em> is a value that is returned by the function using a return statement.  The return statement sends the value being returned from inside of the function's definition to the function's call</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          def formattedName(first, last, middle = " "):
	          """Returns the formatted name"""
	          full = " "
	          if middle == " ":
	              full = first + " " + last
	          else:
	              full = first + " " + middle + " " + last    
	          return full.title()
	      print(formattedName("garrett", "ellis", "david"))
          print(formattedName(first = "garrett", last = "david"))
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            Garrett David Ellis<br />
            Garrett David<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details> 
</ul>

## Returning a Dictionary
<ul>
  <li>
    <a>Functions can even return more complicated data types other than a string, float, bool, or integer.  Functions can even return dictionaries</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          def buildPerson(first, last):<br />
	          """Returns a dictionary of information about a person"""<br />
	          person = {"first": first, "last": last}<br />
	          return person<br />
          print(buildPerson<br />("Garrett", "Ellis"))<br />
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            {'first': 'Garrett', 'last': 'Ellis'}<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details> 
  <ul>
    <li>
      <a>In the function above, buildPerson takes in two arguments into its parameter list: first and last.  Then, these values are stored into a dictionary which is a local variable within the function.  At the end of the function, the function returns the dictionary using a return statement</a> 
    </li>
  </ul>    
</ul>  

## Passing a List
<ul>
  <li>
    <a>A list can be passed as an argument through a function call too.  This list can be a list of anything, whether it be a list of lists, or even a list of dictionaries</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          def printUsers(usernames):<br />
              """This function prints a simple greeting to each user in the list"""<br />
              for users in usernames:<br />
                  print("Hello " + user.title() + "!")<br />
          usernames = ["garrett", "sarah", "samantha"];<br />
          printUsers(usernames)<br />        
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            Hello Garrett!<br />
            Hello Sarah!<br />
            Hello Samantha!<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details> 
</ul>    

## Passing an Arbitrary Number of Arguments
<ul>
  <li>
    <a>Sometimes, you will not know ahead of time when you are defining a function how many parameters the function should take in.  Fortunately, Python allows functions to take in as many arguments from the calling statement</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          def makePizza(*toppings):<br />
              """This function prints a list of toppings that will go on a pizza"""<br />
              print(toppings)<br />
          makePizza("cheese")<br />
          makePizza("garlic", "onions", "cheese")<br />    
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            ('cheese')<br />
            ('garlic', 'onions', 'cheese')<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
  <ul>
    <li>
      <a>The asterisk (*) that is found before the parameter name tells Python to make all variables that are not associated with a parameter to be appended to an empty tuple, which is called the parameter's name</a> 
    </li>
  </ul>
</ul>    
<ul>
  <li>  
    <a>If there is a function that accept several different types of arguments for parameters, the parameter that accepts an unknown number of arguments must be placed at the end of the parameter list.  If the arguments are delivered positionally in the function call, then the arguments which are associated with the parameter of an arbitrary number of arguments must be placed at the end of the function call</a>
  </li>   
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          def makePizza(size, *toppings):<br />
              """This function prints the list of toppings that have been requested"""<br />
              print("Making a " + str(size) + "-inch pizza with the following toppings:)<br />
              for topping in toppings:<br />
                  print("- " + topping.title())<br />
          makePizza(19, "cheese")<br />
          makePizza(20, "garlic", "onions", "cheese")<br />        
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            Making a 19-inch pizza with the following toppings:<br />
            - Cheese<br />
            Making a 20-inch pizza with the following toppings:<br />
            - Garlic<br />
            - Onions<br />
            - Cheese<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>    
</ul>    

## Using Arbitrary Keyword Arguments
<ul>
  <li>
    <a>Sometimes, instead of creating a tuple from an arbitrary number of arguments being passed into a parameter, creating a dictionary may be more useful.  To do this, a key needs to be passed and attached to a value using the assignment operator</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          def buildProfile(first, last, **userInfo):<br />
              profile = {}<br />
              profile["first"] = first<br />
              profile["last"] = last<br />
              for key, value in userInfo.items():<br />
                  profile[key] = value<br />
              return profile<br />
          userInfo = buildProfile("Garrett", "Ellis", location = "Tampa", field = "math")<br />
          print(userInfo)<br />        
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            {'first': 'Garrett', 'last': 'Ellis', 'location': 'Tampa', 'field': 'math'}<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
  <ul>
    <li>
      <a>The function above takes in the arbitrary arguments into the last parameter of the function, and this parameter creates a dictionary from the arbitrary arguments</a>
    </li>
  </ul>     
</ul>    

## Random Number Generation
<ul>
  <li>
    <a>In order for you to be able to generate random numbers in Python, you must use the random library.  To add this library to your project, add the following line of code to the beginning of your project: import random</a>
  </li>
  <li>
    <a>Python pre-defines a set of functions within the random library to help the user generate random numbers</a>
  </li>    
  <li>
    <a>To print a random number between zero and one, you can use the random() function</a>
  </li>  
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          import random<br />  
          print(random.random())<br />     
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            The output of this program is any random float that exists between the integers zero and one<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
  <li>
    <a>Python also has a function called choice() which will return a randomly generated item from a list and a tuple, and a random character from a string</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          import random<br />
          letters = ['a', 'b', 'c']<br />
          print(random.choice(letters))<br />       
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            The output of this program could either be: 'a', 'b', or 'c'<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
  <li>
    <a>To generate a random integer between two numbers, inclusive, Python has a function within the random library called randint().  Within the function, you provide two arguments: one which represents the minimum value and one which represents the maximum value for which the random integer should reside between inclusively</a> 
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          import random<br />
          print(random.randint(1, 10))<br />       
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            The output of this program could be any integer that lies between one and ten, including both values one and ten<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>   
</ul>  