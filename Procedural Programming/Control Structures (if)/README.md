<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#comparison-operators'>Comparison Operators</a>
  </li>
  <li>
    <a href='#logical-operators'>Logical Operators</a>
  </li>
  <li>
    <a href='#conditional-statements'>Conditional Statements</a>
  </li>  
  <li>
    <a href='#introduction-to-loops'>Introduction to Loops</a>
  </li>           
</ol>
</details>

## Comparison Operators

<ul>
  <li>
    <a><em>Equal to operator</em>: compares two values and evaluates to true if the value on the left-hand side of the operator equals the value on the right-hand side of the operator; otherwise, evaluates to false</a>
    <ul>
      <li>
        <a>x == y #compares the values x and y</a>
      </li>
    </ul>
  </li> 
  <li>
    <a><em>Not equal to operator</em>: compares two values and evaluates to false if the value on the left-hand side of the operator equals the value on the right-hand side of the operator; otherwise, evaluates to true</em></a>    
    <ul>
      <li>
        <a>x != y #compares the values x and y</a>
      </li>
    </ul>
  </li>
  <li>
    <a><em>Less than operator</em>: compares two values and evaluates to true if the value on the left-hand side of the operator is less than the value on the right-hand side of the operator; otherwise, evaluates to false</a>   
    <ul>
      <li>
        <a>x < y #compares the values x and y</a> 
      </li>
    </ul>
  </li>
  <li>
    <a><em>Greater than operator</em>: compares two values and evaluates to true if the value on the left-hand side of the operator is greater than the value on the right-hand side of the operator; otherwise, evaluates to false</a> 
    <ul>
      <li>
        <a>x > y #compares the values x and y</a>
      </li>
    </ul>      
  </li> 
  <li>
    <a><em>Less than or equal to operator</em>: compares two values and evaluates to true if the value on the left-hand side of the operator is less than or equal to the value on the right-hand side of the operator; otherwise, evaluates to false</a> 
    <ul>
      <li>
        <a>x <= y #compares the values x and y</a>
      </li>
    </ul>
  </li>  
  <li>
    <a><em>Greater than or equal to operator</em>: compares two values and evaluates to true if the value on the left-hand side of the operator is greater than or equal to the value on the right-hand side of the operator; otherwise, evaluates to false</a> 
    <ul>
      <li>
        <a>x >= y #compares the values x and y</a>
      </li>
    </ul>
  </li>        
</ul>

## Logical Operators
<ul>
  <li>
    <a><em>Logical and operator</em>: compares two statements and evaluate to true if the statement on the left-hand side of the operator is true and if the statement on the right-hand side of the operator is true; otherwise, evaluates to false</a>
    <ul>
      <li>
        <a>x and y #compares the statements x and y</a>
      </li>
    </ul>
  </li>
  <li>
    <a><em>Logical or operator</em>: compares two statements and evaluates to true if at least one of the statements on either the left-hand side or the right-hand side of the operator evaluates to true; otherwise, evaluates to false</a>
    <ul>
      <li>
        <a>x or y #compares the statements x and y</a>
      </li>
    </ul>
  </li>
  <li>
    <a><em>Logical not operator</em>: evaluates to true if a statement or set of statements evaluates to false; otherwise, evaluates to false</a>
    <ul>
      <li>
        <a>not (x and y) #compares the statements x and y and negates its value</a>
      </li>
    </ul>
  </li>
</ul>   

## Conditional Statements
<ul>
  <li>
    <a><em>Conditional statements</em>: test whether conditions evaluates to True and if a condition evaluates to True, the body of code associated with that conditional statement runs. However, if the condition does not evaluate to True, all the code associated with that selection statement is skipped</a>
    <ul>
      <li>
      <a>Here is the syntax for a pair of conditional statements:<br /></a>
      <a>&emsp;&emsp;if expression:<br />
      &emsp;&emsp;&emsp;&emsp;statement<br />
      &emsp;&emsp;else:<br />
      &emsp;&emsp;&emsp;&emsp;statement<br /></a>    
      </li>
      <li>
        <a>If there is the need to have more than one condition that either evaluates to True or False, then there is the elif statement. The elif statement precedes the else statement and lies below the if statement. There can be an infinite number of elif conditional tests; however, there can only be one if statement and one else statement per conditional chain</a>
      </li>
      <details>
      <summary>Example Program</summary>    
        <ul>
          <pre>
            <code>
              &emsp;&emsp;grade = 89.5<br />
              <br />
              &emsp;&emsp;if grade > 70 and grade != 100:<br />
              &emsp;&emsp;&emsp;&emsp;print("You passed the class!")<br />
              &emsp;&emsp;elif grade == 100:<br />
              &emsp;&emsp;&emsp;&emsp;print("You passed and got a perfect score!")<br />
              &emsp;&emsp;else:<br />
              &emsp;&emsp;&emsp;&emsp;print("You failed!")<br />  
            </code>
          </pre>  
          <details>
          <summary>Output</summary>
            <pre>
              <code>
                You passed the class!<br />
              </code>
            </pre>  
          </details>
        </ul>  
      </details>
    </ul>  
  </li>   
</ul> 

## Checking Whether a Value is in a List
<ul>
  <li>
    <a>Sometimes, the programmer will need to find out if an element is contained in a list.  A for loop could be done to accomplish this task, where you loop through each iteration of the list and compare each element to the value you are searching.  There is another way to do this though</a>
  </li>
  <li>
    <a>The use of the keyword <em>in</em> can be used to find whether a list contains a specific element
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          letters = ['a','b','c','d','e']<br />
          if 'a' in letters:<br />
              print("Found it!")<br />
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            Found it!<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details> 
</ul> 

## Introduction to Loops
<ul>
  <li>
    <a>In Python, there are two types of loop statements: the while statement and the for statement</a>
  </li>
  <li>
    <a>The code associated with a loop statement and is repeated as long as a specified condition is met is called the <em>loop body</em></a>
  </li>
  <li>
    <a>Every time the loop runs, it is called a single <em>iteration</em></a>
  </li>
</ul>        
