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
    <a href='#slicing-list'>Slicing List</a>
  </li> 
  <li>
    <a href='#tuples'>Tuples</a>
  </li>              
</ol>
</details>

## Lopping Through an Entire List
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
            9 8 5 6 
          </code>
        </pre>     
      </details>
    </ul>  
  </details>
  <li>
    <a>Python uses indentation to determine where one line of code is connected to the line above it</a>
  </li>
  <li>
    <a>To tell Python that multiple lines of code below the for statement are a part of the for loop, all those lines of code should be indented</a>  
  </li>   
</ul>      