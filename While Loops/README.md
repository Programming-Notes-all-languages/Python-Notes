<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#the-while-loop-in-action'>The while Loop in Action</a>
  </li>
  <li>
    <a href='#using-a-flag'>Using a Flag</a>
  </li>
  <li>
    <a href='#using-break-to-exit-a-loop'>Using break to Exit a Loop</a>
  </li>  
  <li>
    <a href='#using-continue-in-a-loop'>Using continue in a Loop</a>
  </li>               
</ol>
</details>

## The while Loop in Action
<ul>
  <li>
    <a>A while loop will continue over and over until the conditional test evaluates to True.  In other words, if a conditional test continues to evaluate to False, the loop will continue</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          number = 1<br />
	      while number <= 5:<br />
	      if number == 1:<br />
	          print("Number: ", end= "")<br />
	      print(str(number), end= " ")<br />
          number += 1<br />
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            Number: 1 2 3 4 5<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>  
</ul>

## Using a Flag
<ul>
  <li>
    <a>A <em>flag</em> is a boolean value that can be used to control whether certain code needs to be run or not.  Flags are often used in while loops to control the number of iterations a loop goes through</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          value = True
          prompt = "Tell me something and I will repeat it back to you:\nEnter 'quit' to end the program.\n"
          while value:
	          message = input(prompt)
	          if message == "quit":
		          value = False
	          else:
                  print("Your message: " + message)
        print("You left the loop!")
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            Tell me something and I will repeat it back to you:
            Enter 'quit' to end the program.
            Am I in the loop?
            Your message: Am I in the loop?
            Tell me something and I will repeat it back to you:
            Enter 'quit' to end the program.<br />
            quit<br />
            You left the loop!<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
</ul>    

## Using break to Exit a Loop
<ul>
  <li>
    <a>There is a statement that will exit a loop immediately, regardless of whether the flag's value is True or if the conditional test evaluates to True.  This statement is called a <em>break</em> statement</a>
  </li>
</ul>

## Using continue in a Loop
<ul>
  <li>
    <a>The statement that will stop the run of the current iteration of a loop and bring the compiler back to the conditional test statement of the loop is known as the <em>continue</em> statement</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          number = 0<br />
          while number < 10:<br />
              number += 1<br />
              if number % 2 == 0:<br />
                  continue<br />
              print(number, end= " ")<br />
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            1 3 5 7 9 <br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
</ul>    