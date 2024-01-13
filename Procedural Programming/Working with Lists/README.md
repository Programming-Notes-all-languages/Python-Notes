<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#looping-through-an-entire-list'>Looping Through an Entire List</a>
  </li>
  <li>
    <a href='#using-the-range-function'>Using the range Function</a>
  </li>  
  <li>
    <a href='#simple-statistics-with-a-list-of-numbers'>Simple Statistics with a List of Numbers</a>
  </li>  
  <li>
    <a href='#slicing-lists'>Slicing Lists</a>
  </li> 
  <li>
    <a href='#tuples'>Tuples</a>
  </li>              
</ol>
</details>

## Looping Through an Entire List
<ul>
  <li>
    <a>You will often want to loop through all iterations of a list, performing an identical task each time.  When you have this repetitive task you would like to accomplish, you could use Python's for loop</a>
  </li>
  <li>
    <a>The syntax for a for loop iterating through each index of a list is the following: for index in listName:</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          numbers = [9, 8, 5, 6]<br />
          for number in numbers</br />
              print(number, end = " ")<br />
        </code>
      </pre> 
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            9 8 5 6<br />
          </code>
        </pre>     
      </details>
    </ul>  
  </details>
  <li>
    <a>Python uses indentation to determine which lines of code are attributed to a loop</a>
  </li>
  <li>
    <a>If a loop is, for let's say, dozens and dozens of lines long, then all those lines need to be indented until the code for the loop is completed</a>  
  </li>   
</ul>  

## Using the range Function
<ul>
  <li>
    <a>The range() function starts counting from the first number entered into the function, and stops at the last number entered into the function.  In other words, the range() function is inclusive of the first number, and not inclusive of the second number</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          for i in range(1, 6):<br />
              print(i, end = " ")<br />
        </code>
      </pre> 
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            1 2 3 4 5<br />   
          </code>
        </pre>     
      </details>
    </ul>  
  </details> 
  <li>
    <a>A simple way to make a list of numbers is by using the range() function.  You can wrap the list() function around the range() function and set it equal to a variable name</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          numbers = list(range(1, 6))<br />
          print(numbers)<br />
        </code>
      </pre> 
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            [1, 2, 3, 4, 5]<br /> 
          </code>
        </pre>     
      </details>
    </ul>  
  </details> 
  <li>
    <a>The range() function not only produces numbers simply one after another.  A third argument can be passed telling Python to skip a certain number of integers within a range</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          numbers = list(range(2, 11, 2))<br />
          print(numbers)<br />
        </code>
      </pre> 
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            2 4 6 8 10<br /> 
          </code>
        </pre>     
      </details>
    </ul>  
  </details> 
  <li>
    <a>The range function can basically produce any set of numbers you would like</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          squares = []<br />
          for i in range(1, 11):<br />
              squares.append(i ** 2)<br />
          print(squares)<br />    
        </code>
      </pre> 
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            1 4 9 16 25 36 49 64 81 100<br />  
          </code>
        </pre>     
      </details>
    </ul>  
  </details>     
</ul>  

## Simple Statistics with a List of Numbers
<ul>
  <li>
    <a>There are a few Python functions that are specific to lists of integers and floats.  For example, you can easily find the minimum, maximum, and sum of a list of numbers using pre-defined functions</a>
  </li>
  <ul>
    <li>
      <a>To find the minimum value of the list, use the min() function</a>
    </li>
    <li>
      <a>To find the maximum value of the list, use the max() function</a>
    </li>
    <li>
      <a>To find the sum of all the values of a list, use the sum() function</a>
    </li>    
  </ul>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          numbers = list(range(1, 6))<br />
          print("Minimum: " + str(min(numbers)))<br />
          print("Maximum: " + str(max(numbers)))<br />
          print("Sum: " + str(sum(numbers)))<br />    
        </code>
      </pre> 
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            Minimum: 1<br />
            Maximum: 6<br />
            Sum: 15<br />  
          </code>
        </pre>     
      </details>
    </ul>  
  </details> 
</ul>  

## Slicing Lists
<ul>
  <li>
    <a>Slicing is essentially cutting a portion of a list out that you would like to do something with.  Same with the range() function, the first index of the slice is included, but the last index of the slice that the user types is not included</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          numbers = list(range(1, 6))<br />
          numbers = numbers[1:4]<br />
          print(numbers)<br />  
        </code>
      </pre> 
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            [2, 3, 4]<br />
          </code>
        </pre>     
      </details>
    </ul>  
  </details>  
  <li>
    <a>Omitting the first index when you slice a list tells Python that the slice starts at the first index of the list, in other words, at index zero</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          numbers = list(range(1, 6))<br />
          numbers = numbers[:4]<br />
          print(numbers)<br />   
        </code>
      </pre> 
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            [1, 2, 3, 4]<br />
          </code>
        </pre>     
      </details>
    </ul>  
  </details> 
  <li>
    <a>If you omit the last index in a slice, then similarly to omitting the first index of a slice, the slice begins at the first index and continues until the end of the list</a> 
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          numbers = list(range(1, 6))<br />
          numbers = numbers[1:]<br />
          print(numbers)
        </code>
      </pre> 
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            [2, 3, 4, 5]<br />   
          </code>
        </pre>     
      </details>
    </ul>  
  </details>
  <li>
    <a>The indices of the slice's range can also be negative.  A negative slice indicates that the slice will begin from a position x digits smaller than the last given index in a slice</a>
  </li>   
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          numbers = list(range(1, 6))<br />
          numbers = numbers[-3:]
          print(numbers)    
        </code>
      </pre> 
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            [3, 4, 5]<br />  
          </code>
        </pre>     
      </details>
    </ul>  
  </details>   
</ul> 

## Tuples
<ul>
  <li>
    <a>A <em>tuple</em> is essentially a list that is constant, meaning the list's elements cannot be changed.  Instead of surrounding a tuple with brackets like you would do with a list, you surround a tuple with a set of parentheses</a>
  </li>
  <li>
    <a>Once a tuple has been declared, its values can be accessed just like a list; however, each element of the tuple after its declaration cannot be modified.  The only way a tuple can be modified post declaration is if the entire tuple is redefined</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          dim = (1, 2)<br />
          print("Original: " + str(dim[0] + str(dim[1])))<br />
          dim = (0, 1)<br />
          print("Altered: " + str(dim[0]) + str(dim[1]))<br />
        </code>
      </pre> 
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            12<br />
            01<br />  
          </code>
        </pre>     
      </details>
    </ul>  
  </details> 
</ul>      