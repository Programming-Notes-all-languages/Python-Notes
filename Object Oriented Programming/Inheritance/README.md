<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#inheritance-in-object-oriented-programming'>Inheritance in Object-Oriented Programming</a>
  </li>
  <li>
    <a href='#implementing-inheritance'>Implementing Inheritance</a>
  </li>   
  <li>
    <a href='#abstract-classes-and-methods'>Abstract Classes and Methods</a>  
  </li>      
</ol>
</details>

## Inheritance in Object-Oriented Programming
<ul>
  <li>
    <a>Inheritance is an object-oriented programming principle than enables the programmer to build on an already existing class.  This is a very useful concept in programs that are very large.  There is often the need to build a class that is very similar to an already existing class, but this one has additional features.  Inheritance is the simple answer in achieving this task.  The principle of inheritance is basically the creation of a new class that includes all methods and variables within the base class, but adds additional functionality</a>
  </li>
  <li>
    <a>When talking about inheritance, the classes being referred to are often called base classes and subclasses</a>
  </li>  
  <ul>
    <li>
      <a>The <em>base class</em> is the class in which other classes inherit from.  It is essentially the starting point of subclasses</a>
    </li>
    <li>
      <a>The <em>subclass</em> is the class that is inheriting from another class, called the base class.  The sub class adds additional functionality to the base class, without actually modifying the base class</a>
    </li>  
  </ul>   
  <li>
    <a>Methods within the subclass can redefine methods defined within the base class.  In other words, methods within the subclass can exists that have the same name as those methods within the base class, but have different functionality.  This process is called <em>overriding</em>.  When an overridden method is called, its implementation as defined by the subclass is carried out</a>
  </li>  
</ul>     

## Implementing Inheritance
<ul>
  <li>
    <a>Python's syntax regarding inheritance is simple.  The base class does not need to know which classes within a project are its subclasses--only subclasses need to say which class is its base class.  Here is the syntax for two classes, one called Base and one called Subclass, where Subclass inherits all of the properties from Base:</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <pre>
      <code>
        class Base():<br />
          #methods<br />
        class Subclass(Base):<br />
          #methods<br />  
      </code>
    </pre> 
  </details>
  <ul>
    <li>
      <a>Within the subclass' statement inside of the parentheses goes the name of the class in which it is inheriting from.  In this case, the name Base goes within the parentheses</a>
    </li>
  </ul>    
  <li>
    <a>The super() function is a predefined Python function that will make the subclass inherit a method's implementation from its base class</a>
  </li> 
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          class Employee:<br />
            def __init__(self, name, title, salary):<br />
              self.__name = name<br />
              self.__title = title<br />
              self.__salary = salary<br />
            def printEmployee(self):<br />
              print("Name: " + self.__name)<br />
              print("Title: " + self.__title) <br />
              print("Salary: $" + str(self.__salary))<br />
          <br />      
          class Developer(Employee):<br />
            def __init__(self, name, title, salary, language):<br />
              super().__init__(name, title, salary)<br />
              self.__language = language<br />
            def printEmployee(self):<br />
              super().printEmployee()<br />
              print("Language: " + self.__language)<br />
          <br />      
          dev1 = Developer("Garrett", "Special Developer", 100000, "Python")<br />
          dev1.printEmployee()<br />           
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            Name: Garrett<br />
            Title: Special Developer<br />
            Salary: $100000<br />
            Language: Python<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details> 
</ul>    

## Abstract Classes and Methods
<ul>
  <li>
    <a>An <em>abstract class</em> is a class that is not meant to be initialized, and actually cannot be initialized, rather serve as a base class for subclasses</a>
  </li>
  <li>
    <a>An <em>abstract method</em> is a method that will always be overridden by a method with the same name within the subclasses
  </li>
  <li>
    <a>To make an abstract class, you need to include the following statement at the beginning of the file containing the class' definition: from abc import ABC.  Then, within the first line of the class' definition, the string, ABC, needs to be placed within parentheses following the class' name</a>
  </li>
  <li>
    <a>To make a method an abstract method, it most be preceded by the @abstractmethod decorator.  With the abstract method decorator, abstractmethod also needs to imported from abc (notice how this is different from and class and static methods)</a> 
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          from abc import ABC, abstractmethod<br />
          class Vehicle(ABC):<br />
            def __init__(self, name, numWheels):<br />
              self.__name = name<br />
              self.__numWheels = numWheels<br />
            def getName(self):<br />
              return self.__name<br />
            <br />    
            def getNumWheels(self):<br />
              return self.__numWheels<br />
            @abstractmethod<br />
            def printData(self):<br />
               pass<br />
          <br />
          class Car(Vehicle):<br />
            def __init__(self, name, numWheels, driver):<br />
              super().__init__(name, numWheels)<br />
              self.__driver = driver<br />
            def printData(self):<br />
              print("Name: " + super().getName())<br />
              print("Number of wheels: " + str(super().getNumWheels()))<br />
              print("Driver: " + self.__driver)<br /> 
          <br />
          car1 = Car("Hyundai", 4, "Garrett")<br />
          car1.printData()<br />               
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            Name: Hyundai<br />
            Number of wheels: 4<br />
            Driver: Garrett<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>      
</ul>    
