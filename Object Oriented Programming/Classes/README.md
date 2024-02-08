<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#writing-a-class-in-python'>Writing a Class in Python</a>
  </li>
  <li>
    <a href='#instance-methods,-static-methods,-and-class-methods'>Instance Methods, Static Methods, and Class Methods</a>
  </li>
  <li>
    <a href='#difference-between-functions-and-methods'>Difference between Functions and Methods</a>
  </li>  
  <li>
    <a href='#creating-and-calling-objects-from-a-class'>Creating and Calling Objects from a Class</a>
  </li> 
  <li>
    <a href='#passing-arguments-to-a-method'>Passing Arguments to a Method</a>
  </li>
  <li>
    <a href='#initialization-parameters'>Initialization Parameters</a>
  </li>             
</ol>
</details>

## Writing a Class in Python
<ul>
  <li>
    <a>You first begin a <em>class</em> definition with the class keyword.  Following the class keyword comes the name of the class which is defined by the user.  The convention for naming a class is that the class' name begins with an uppercase character.  After the name of the class, a set of parenthesis can follow, but that is optional.  The statement must then end with a colon, which indicates to Python that the beginning of the class' body is about to commence</a>
  </li>
  <li>
    <a>All the methods and class variables that are a part of the class must be indented.  The indentation with a class is the same as the indentation with conditional statements and functions in Python</a>
  </li>  
  <li>
    <a>Within the body of the class lies many functions; however, in Python, any function defined within a class is given a special name, a <em>method</em></a>
  </li>
  <li>
    <a>The first method within every single class should be called __init__().  Whenever a class is instantiated, meaning an object of the class is created, this method will always run.  The name __init__ is reserved by Python to be a constructor for a class</a>
  </li>    
  <li>
    <a>Methods can have multiple types of variables, including: local variables, instance variables, and class variables</a>
    <ul>
      <li>
        <a><em>Local variables</em> are variables that do not start with self.  A local variable is not an attribute of a class, and is only alive throughout the duration of the method.  Once the method exits, the local variable is gone</a>
      </li>
      <li>
        <a><em>Instance variables</em> are variables that have an object scope, meaning that they are accessible to all methods within the class</a>  
      </li>
      <li>
        <a><em>Class variables</em> are variables that are shared by every instance of the same class.  These variables are defined within the class, but outside of any method</a>
      </li>
    </ul>      
  </li>
  <li>
    <a>Each object, also known as an instantiation of a class, has its own set of instance variables.  These instance variables are not shared amongst other instances of the class</a>  
  </li>
</ul>    

## Instance Methods, Static Methods, and Class Methods
<ul>
  <li>
    <a>Instance methods are methods that perform actions on instance variables.  Instance methods also need the keyword self in them.  Instance methods:</a>
    <ul>
      <li>
        <a>Are bound to the instance of the class</a>
      </li>
      <li>
        <a>Can modify an instance of a class</a>
      </li>
      <li>
        <a>Can both access and modify any instance and class variables</a>
      </li>    
    </ul>    
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          class Calculator:<br /> 
              def __init__(self, version):<br /> 
                  self.version = version<br /> 
              <br />     
              def description(self):<br /> 
                  print("The current version of the calculator is: " + str(self.version))<br /> 
              <br /> 
          calc1 = Calculator(1)<br /> 
          calc2 = Calculator(2)<br /> 
          <br />  
          calc1.description()<br /> 
          calc2.description()<br /> 
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            {'color': 'green'}<br />
            {'color': 'green', 'name': 'Garrett'}<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>  
  <li>
    <a>Class methods are methods that call on the class itself rather than an instance of the class.  Class methods use the keyword cls instead of the keyword self like in instance methods.  Class methods:</a> 
  </li>
  <ul>
    <li>
      <a>Are bound to the class in which the method is defined under</a>
    </li>
    <li>
      <a>Can modify the state of the class</a>
    </li>
    <li>
      <a>Can only access class variables--not instance variables</a>
    </li>
    <li>
      <a>Use the class method decorator, @classmethod, to define a class method</a>
    </li>  
  </ul>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          class Calculator:<br />
              mode = 1<br />
              <br />
              @classmethod<br />
              def incrementMode(cls):<br />
                  cls.mode += 1<br />
              <br />
              @classmethod<br />
              def printMode(cls):<br />
                  print("Mode: " + str(cls.mode))<br />
          <br />
          Calculator.incrementMode()<br />
          Calculator.printMode()<br />
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            Mode: 2<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details> 
  <li>
    <a>Static methods are methods that do not have access to both class variables and instance variables.  Static variables:</a>  
  </li>
  <ul>
    <li>
      <a>Are bound to the class</a>
    </li>
    <li>
      <a>Cannot modify any of the class or instance variables</a>
    </li>
    <li>
      <a>Cannot change the state of a class or instance of a class</a>
    </li>
    <li>
      <a>Use the static method decorator, @staticmethod, to define a static method</a>
    </li>  
  </ul>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          class Calculator:<br />
              @staticmethod<br />
              def printMessage():<br />
                  print("Hello!")<br />
          <br />
          Calculator.printMessage()<br />
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
</ul> 

## Differences between Functions and Methods
<ul>
  <li>
    <a>Here are the two key differences between functions and methods in Python:</a>
  </li>
  <ul>
    <li>
      <a>Every single method of a class must be indented with a tab after the statement which contains the keyword class and the name of the class defined by the user</a>
    </li>
    <li>
      <a>All methods, except for static methods, have a special first parameter within the method's definition.  By convention, the special parameter's name for instance methods is self and the special parameter's name for class methods is cls</a>
    </li>  
  </ul>
</ul>   

## Creating and Calling Objects from a Class
<ul>
  <li>
    <a>To use a class in most cases, you will have to create an instance of a class.  This is only true, however, for instance methods.  Class and static methods are bound to a class, not an instance of a class.  To instantiate a class, you use the assignment operator and include a statement like this into your program: object = className(argumentsIfAny)</a>
  </li>
  <li>
    <a>After the creation of an object, to then call a method from that instance's class, you would use the generic syntax as follows: objectName.methodName(argumentsIfAny)</a>
  </li>
  <li>
    <a>One of the main features of object-oriented programming is that you can instantiate an infinite number of objects from a single class</a>
  </li>  
</ul>

## Passing Arguments to a Method
<ul>
  <li>
    <a>When calling any function, the number of arguments must match the number of parameters in the function's parameter list.  The same rule applies for methods too; however, some methods like instance and class methods will appear to have one extra parameter in their parameter list</a>
  </li>
</ul>  

## Initialization Parameters
<ul>
  <li>
    <a>Passing arguments to a method also works when instantiating a class.  Oftentimes, a class' constructor will have multiple parameters; therefore, when creating an instance of a class, the constructor's call will need to match the number of arguments as defined within the class</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          class Person:<br />
              def __init__(self, name, age, sex):<br />
              self.name = name<br />
              self.age = age<br />
              self.sex = sex<br />
              <br />
              def print(self):<br />
                  print("Name: " + self.name + "\nAge: " + str(self.age) + "\nSex: " + self.sex)<br />    
          <br />
          person1 = Person("Garrett", 20, "male")<br />
          person1.print()<br />
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            Name: Garrett<br />
            Age: 20<br />
            Sex: male<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
</ul>    
