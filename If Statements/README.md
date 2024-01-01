<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#checking-for-equality'>Checking for Equality</a>
  </li>
  <li>
    <a href='#checking-for-inequality'>Checking for Inequality</a>
  </li>
  <li>
    <a href='#using-and-to-check-multiple-conditions'>Using and to Check Multiple Conditions</a>
  </li>  
  <li>
    <a href='#using-or-to-check-multiple-conditions'>Using or to Check Multiple Conditions</a>
  </li> 
  <li>
    <a href='#checking-whether-a-value-is-in-a-list'>Checking Whether a Value is ini a List</a>
  </li>
  <li>
    <a href='#the-if-elif-else-chain'>The if-elif-else Chain</a>
  </li>               
</ol>
</details>

## Checking for Equality
<ul>
  <li>
    <a>Every if, elif, and else statement can essentially be boiled down to the following--it either evaluates to True or False.  This statement that is either True or False is called a <em>conditional test</em>.  Python uses the values True and False to determine whether a block of code will run or not</a>
  </li>
  <ul>
    <li>
      <a>If a conditional test evaluates to True, the block of code that is indented underneath the if, elif, or else statement will run</a>
    </li>
    <li>
      <a>If a conditional test evaluates to False, the block of code that is indented underneath the if, elif, or else statement will be ignored</a>
    </li> 
  </ul>
  <li>
    <a>Most conditional tests will compare a variable's value to a value of interest</a>
  <li>
    <a>For example, let's say that a variable called name has been initialized and has the value "Garrett".  A simple conditional test could check to see if the variable name is equivalent to the string "Garrett" such as in the following: name == "Garrett".  This conditional test will evaluate to True</a>
  </ul>    
</ul>

## Checking for Inequality
<ul>
  <li> 
    <a>To determine whether two variable's values are not equal to each other, you can use this operator: !=.  The exclamation point in Python means not, so this operator means not equal to</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          letter = 'a'<br />
          if letter != 'A':<br />
              print("Letter is: + a)<br />
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
          Letter is: a<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
</ul> 

## Using and to Check Multiple Conditions
<ul>
  <li>
    <a>Sometimes, you will want to know if two or more conditions all evaluate to True.  In order to do this, you will need to use the <em>and</em> keyword</a>
  </li>
  <li>
    <a>If any condition compounded to an and keyword fails, then the conditional test will evaluate to False.  Both conditions on either side of the and statement must be true for a conditional test to evaluate to True</a> 
  </li>
</ul> 

## Using or to Check Multiple Conditions
<ul>
  <li>
    <a>The keyword <em>or</em> also enables the user to test multiple conditions against each other like the and statement; however, only one condition on either side of the or statement must evaluate to True for a chance of the conditional statement to evaluate to True</a>
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

## Checking Whether a Value is not in a List
<ul>
  <li>
    <a>To find out whether a value is not in a list, you can use the <em>not</em> keyword</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          letters = ['a', 'b', 'c']<br />
          if 'd' not in letters:<br />
              print("Not found!")<br />
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            Not found!
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
</ul>   

## The if-elif-else Chain
<ul>
  <li>
    <a>Oftentimes, you will have a chain consisting of a singular if statement, multiple elif statements, and an else statement.  Python, however, will only execute one block of code from this chain of statements.  When one of the statements evaluates to True, the rest of the statements within the chain are ignored and skipped</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          number = 63<br />
          if number == 1:<br />
              print(1)<br />
          elif number = 2<br />
              print(2)<br />
          else:<br />
              print(number)<br />        
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            63
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
  <li>
    <a>Python allows you to use as many elif statements within a chain as you would like</a>
  </li>
  <li>
    <a>Python does not require an else statement at the end of an if-elif chain.  Sometimes it is useful to have one and sometimes it can be omitted</a>
  </li>    
</ul>    