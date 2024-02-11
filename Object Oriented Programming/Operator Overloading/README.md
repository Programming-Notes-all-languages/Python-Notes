<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#basics-of-operator-overloading'>Basics of Operator Overloading</a>
  </li>
  <li>
    <a href='#comparison-operator-magic-methods'>Comparison Operator Magic Methods</a>
  </li>     
  <li>
    <a href='#math-operator-magic-methods'>Math Operator Magic Methods</a>
  </li>      
</ol>
</details>

## Basics of Operator Overloading
<ul>
  <li>
    <a>Operator overloading is essentially a concept that gives further meaning to already existing operators within Python</a>
  </li>
</ul>    

## Comparison Operator Magic methods
<ul>
  <li>
    <a>Here are the six comparison operator magic methods:</a>
  </li>
  <ul>
    <li>
      <a>equal to (==): __eq__()</a>  
    </li>
    <li>
      <a>not equal to (!=): __ne__()</a>
    </li>
    <li>
      <a>less than (<): __lt__()</a> 
    </li>
    <li>
      <a>greater than (>): __gt__()</a> 
    </li>
    <li>
      <a>less than or equal to (<=): __le__()</a>
    </li>
    <li>
      <a>greater than or equal to (>=): __ge__()</a>
    </li>       
  </ul>
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
              def __eq__(self, other):<br />
                  if self.__name == other.__name and self.__age == other.__age and self.__gender == other.__gender:<br />
                      return True<br />
                  else:<br />
                      return False<br />
              <br />      
              def __gt__(self, other):<br />
                  if self.__age > other.__age:<br />
                      return True<br />
                  else:<br />
                      return False<br />
          <br />               
          person1 = Person("Garrett", 20, "Male")<br />
          person2 = Person("Eddie", 25, "Male")<br />
          <br />
          if person1 == person2:<br />
              print("Both people are the same.")<br />   
          else:<br />
              if person1 > person2:<br />
                  print("Person1 is older.")<br />
              else:<br />
                  print("Person2 is older.")<br />           
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            Person 2 is older.<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
</ul> 

## Math Operator Magic Methods
<ul>
  <li>
    <a>Here are the six comparison operator magic methods:</a>
  </li>
  <ul>
    <li>
        <a>addition (+): __add__()</a>
    </li>
    <li>
        <a>subtraction (-): __sub__()</a>
    </li>
    <li>
        <a>multiplication (*): __mul__()</a>
    </li>
    <li>
        <a>division, floating point result, (/): __truediv__()</a>
    </li>
    <li>
        <a>integer division (//): __floordiv__()</a>
    </li>
    <li>
        <a>modulo (%): __mod__()</a>
    </li>
    <li>
        <a>absolute value (Abs): __abs__()</a>
    </li>
  </ul>  
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          class Vector():<br />
              def __init__(self, x, y, z):<br />
                  self.__x = x<br />
                  self.__y = y<br />
                  self.__z = z<br />
              <br />  
              def __add__(self, other):<br />
                  return Vector(self.__x + other.__x, self.__y + other.__y, self.__z + other.__z)<br />
              <br />
              def __sub__(self, other):<br />
                  return Vector(self.__x - other.__x, self.__y - other.__y, self.__z - other.__z)<br />
              <br />
              def __mul__(self, other):<br />
                  return Vector(self.__x * other.__x, self.__y * other.__y, self.__z * other.__z)<br />
              <br />
              def __truediv__(self, other):<br />
                  return Vector(self.__x / other.__x, self.__y / other.__y, self.__z / other.__z)<br />
              <br />
              def __mod__(self, other):<br />
                  return Vector(self.__x % other.__x, self.__y % other.__y, self.__z % other.__z)<br /> 
              <br />
              def __abs__(self):<br />
                  return Vector(abs(self.__x), abs(self.__y), abs(self.__z))<br />
              <br />  
              def printVector(self):<br />
                  print("(" + str(self.__x) + ", " + str(self.__y) + ", " + str(self.__z) + ")")<br />
          <br />
          v1 = Vector(1, 2, 3)<br />
          v2 = Vector(45, -56, 6)<br />
          v3 = v1 + v2<br />
          v4 = v2 - v1<br />
          v5 = v1 * v2<br />
          v6 = v2 / v1<br />
          v7 = v2 % v1<br />
          v8 = abs(v2)<br />
          <br />
          print("Summation of v1 and v2: ", end="")<br />
          v3.printVector()<br />
          print("Subtracting v2 and v1: ", end="")<br />
          v4.printVector()<br />
          print("Multiplication of v1 and v2: ", end="")<br />
          v5.printVector()<br />
          print("Division of v2 by v1: ", end="")<br />
          v6.printVector()<br />
          print("Modulus of v2 by v1: ", end="")<br />
          v7.printVector()<br />
          print("Absolute value of v2: ", end="")<br />
          v8.printVector()<br />           
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            Summation of v1 and v2: (46, -54, 9)<br />
		    Subtracting v2 and v1: (44, -58, 3)<br />
		    Multiplication of v1 and v2: (45, -112, 18)<br />
		    Division of v2 by v1: (45.0, -28.0, 2.0)<br />
		    Modulus of v2 by v1: (0, 0, 0)<br />
            Absolute value of v2: (45, 56, 6)<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
</ul>               
