<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#making-instance-variables-more-private'>Making Instance Variables more Private</a>
  </li>
  <li>
    <a href='#setters-and-getters'>Setters and Getters</a>
  </li>         
</ol>
</details>

## Making Instance Variables more Private
<ul>
  <li>
    <a>By default in Python, are instance variables are made public, meaning that those variables can be accessed and modified directly outside of the class.  This however breaks the principle of <em>encapsulation</em>: a way to restrict direct access to components of a class, whether that be instance variables or methods, so the user cannot have access to those values directly</a>
  </li>
  <li>
    <a>To make an instance variable or a method private, you can do the following:</a>
  </li>
  <ul>
    <li>
      <a>Add one underscore to the beginning of the instance variable's or method's name.  This marks the instance variable or method as being never accessible by the user; however, if the client software makes a call an instance variable or method with only one leading underscore, Python will grant it access.  This can lead to errors though.</a> 
    </li>
    <li>
      <a>Add two underscores to the beginning of the instance variable's or methods name.  This ensures that the user cannot access private member attributes and methods with a call and also prevents software from getting direct access to these values</a>
    </li>   
  </ul>     
</ul>   

## Setters and Getters
<ul>
  <li>
    <a>A common way to access private member attributes indirectly is by using accessor and mutator methods, also known as setters and getters</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          class Person():<br />
              def __init__(self, name, age, gender):<br />
                  self.__name = name<br />
                  self.__age = age<br />
                  self.__gender = gender<br />
              <br />    
              def setName(self, name):<br />
                  self.__name = name<br />
              <br />    
              def getName(self):<br />
                  return self.__name<br />
          <br />
          Garrett = Person("Garrett", 20, "male")<br />
          print(Garrett.getName())<br />           
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            Garrett<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
  <ul>
    <li>
      <a>In the example above, the constructor creates three private instance variables and initializes them to a value</a>
    </li>
    <li>
      <a>Then there is the method called setName() which takes in one argument when it is called and sets the private member attribute name to the argument's value</a>
    </li>
    <li>
      <a>Lastly, there is the method called getName() which returns the value of the private member attribute name's value</a>
    </li>   
  </ul>    
</ul>    
