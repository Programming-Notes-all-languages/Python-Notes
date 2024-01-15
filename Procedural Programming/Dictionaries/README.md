<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#working-with-dictionaries'>Working with Dictionaries</a>
  </li>
  <li>
    <a href='#adding-new-key-value-pairs'>Adding New Key-Value Pairs</a>
  </li>
  <li>
    <a href='#starting-with-an-empty-dictionary'>Starting with an Empty Dictionary</a>
  </li>  
  <li>
    <a href='#modifying-values-in-a-dictionary'>Modifying Values in a Dictionary</a>
  </li> 
  <li>
    <a href='#removing-key-value-pairs'>Removing Key-Value Pairs</a>
  </li>
  <li>
    <a href='#looping-through-a-dictionary'>Looping Through a Dictionary</a>
  </li>
  <li>
    <a href='#looping-through-all-the-keys-in-a-dictionary'>Looping Through all the Keys in a Dictionary</a>
  </li> 
  <li>
    <a href='#looping-through-a-dictionarys-keys-in-order'>Looping Through a Dictionary's Keys in Order</a>
  </li>
  <li>
    <a href='#a-list-of-dictionaries'>A List of Dictionaries</a>
  </li>  
  <li>
    <a href='#a-list-in-a-dictionary'>A List in a Dictionary</a>
  </li>        
  <li>
    <a href='#a-dictionary-in-a-dictionary'>A Dictionary in a Dictionary</a>
  </li>             
</ol>
</details>

## Working with Dictionaries
<ul>
  <li>
    <a>A <em>dictionary</em> in Python is a collection of keys and values, where each <em>key</em> is assigned a <em>value</em></a>
  </li>
  <li>
    <a>A key's value can be of any type, such as a string, float, integer, list, and even another dictionary</a>
  </li>
  <li>
    <a>A dictionary is wrapped in braces ({}) and contains keys and values within the braces</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          alien = {"color": "green"}<br />
          print("The alien's color is: " + alien["color"])<br />
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            The alien's color is: green<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details> 
  <li>
    <a>A <em>key-value pair</em> is a key that has a value associated with it.  Every key and value is separated by a colon, meaning that there is a colon after the key is enter, which precedes the key's value</a>
  </li>  
</ul> 

## Adding New Key-Value Pairs
<ul>
  <li>
    <a>Dictionaries are dynamic, meaning that they are not fixed and can be altered throughout the duration of the program</a>
  </li>
  <li>
    <a>To add a new key-value pair to a dictionary, you write the name of the dictionary followed by a set of brackets which encloses the name of the new key.  Then, you assign a value to the new key using the assignment operator</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          alien = {"color": "green"}<br />
          print(alien)<br />
          alien["name"] = "Garrett"<br />
          print(alien)<br />
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
</ul>

## Starting with an Empty Dictionary
<ul>
  <li>
    <a>To define an empty dictionary, you do a practice similar to defining an empty list or tuple.  You simply just write the dictionary name followed by an assignment operator and a set of empty braces</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          alien = {}<br />
          print(alien)<br />
          alien["color"] = "green"<br />
          print(alien)
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            {}<br />
            {'color': 'green'}<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
</ul>  

## Modifying Values in a Dictionary
<ul>
  <li> 
    <a>When modifying a value in a dictionary, you need to give Python the name of a dictionary with an existing key inside of a set of square brackets.  Then, using the assignment operator, you give the key a new value to be associated with</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          increment = 0<br />
          alien = {"positionX": 0, "positionY": 0, "speed": "medium"}<br />
          print("Original position in coordinate form: " + str(alien["positionX"]) + ", " + str(alien["positionY"]))<br />
          if alien["speed"] == "slow":<br />
              increment += 1<br />
          elif alien["speed"] == "medium":<br />
              increment += 2<br />
          else:<br />
              increment += 3<br />      
          alien["positionX"] += increment<br />
          print("New position in coordinate form: " + str(alien["positionX"]) + ", " + str(alien["positionY"]))<br />
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            Original position in coordinate form: 0, 0<br />
            New position in coordinate form: 2, 0 <br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
</ul>    

## Removing Key-Value Pairs
<ul>
  <li>
    <a>If you would like to remove a key-value pair from a dictionary, you can use the del statement to completely remove that pair.  You first write the del keyword, followed by the name of the dictionary next to a set a brackets that enclose the desired key to be deleted</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          alien = {"color": "green", "points": 5}<br />
          print(alien)<br />
          del alien["color"]<br />
          print(alien)
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            {'color': 'green', 'points': 5}<br />
            {'points': 5}<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
</ul>    

## Looping Through a Dictionary
<ul>
  <li>
    <a>Python dictionaries can contain only a few key-value pairs, and some dictionaries can contain millions of pairs.  Because of this, Python lets you loop through a dictionary</a>
  </li>
  <li>
    <a>Looping through each key-value pair within a dictionary can be done using the items() method</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          alien = {"positionX": 0, "positionY": 0, "speed": "medium"}<br />
          for key, value in alien.items():<br />
              print(str(key) + ": " + str(value))<br />
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            positionX: 0<br />
            positionY: 0<br />
            speed: medium<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
</ul>    

## Looping Through All the Keys in a Dictionary
<ul>
  <li>
    <a>Looping through just each of the keys within a dictionary can be done using the keys() method</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          alien = {"positionX": 0, "positionY": 0, "speed": "medium"}<br />
          for key in alien.keys():<br />
              print(str(key))<br />
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            positionX<br />
            positionY<br />
            speed<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details> 
</ul>

## Looping Through a Dictionary's Keys in Order
<ul>
  <li>
    <a>When just looping through a dictionary using no special function or method, the order in which the keys are returned is the same order as the keys were initialized.  One option to get the keys to print in a nicer order is using the sorted function</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          alien = {"positionX": 0, "positionY": 0, "speed": "medium"}<br />
          for key in sorted(alien.keys()):<br />
              print(str(key))<br />
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
          positionX<br />
          positionY<br />
          speed<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
</ul>   

## Looping Through all Values in a Dictionary
<ul>
  <li>
    <a>To loop through all of the values within a dictionary, you could use the values() method</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          alien = {"positionX": 0, "positionY": 0, "speed": "medium"}<br />
          for key in alien.values():<br />
              print(str(key))<br />
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            0<br />
            0<br />
            medium<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
</ul>  

## A List of Dictionaries
<ul>
  <li>
    <a>Sometimes, it is useful to store multiple dictionaries within a list, which is called <em>nesting</em>.  You can have a list of multiple dictionaries, a dictionary full of lists, and even dictionaries containing dictionaries</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          alien = {"positionX": 0, "positionY": 0, "speed": "medium"}<br />
          alien1 = {"positionX": 1, "positionY": 1, "speed": "medium"}<br />
          listAliens = [alien, alien1]<br />
          for martian in listAliens:<br />
              print(martian)<br />
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            {'positionX': 0, 'positionY': 0, 'speed': 'medium'}<br />
            {'positionX': 1, 'positionY': 1, 'speed': 'medium'}<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
</ul>    

## A List in a Dictionary
<ul>
  <li>
    <a>Rather than having a list full of dictionaries, it is sometimes useful to have lists within dictionaries</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          alien = {"list1": [0, 1, 2, 3], "list2": ['a', 'b', 'c']}<br />
          for key, value in alien.items():<br />
              print(key + str() + ': ' + str(value))<br />
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            list1: [0, 1, 2, 3]<br />
            list2: ['a', 'b', 'c']<br /> 
          </code>
        </pre>  
      </details>
    </ul>  
  </details> 
</ul>

## A Dictionary in a Dictionary
<ul>
  <li>
    <a>Dictionaries can be nested inside of dictionaries, but things can get complicated quickly using this idea</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          users = {"egarrett": {"first": "Garrett", "last": "Ellis"}, "dellis": {"first": "David", "last": "Ellis"}}<br />
          for key, value in users.items():<br />
	      print("User: " + key)<br />
          print("First Name: " + value["first"] + "\nLast Name: " + value["last"])<br />
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            User: egarrett<br />
	    First Name: Garrett<br />
	    Last Name: Ellis<br />
	    User: dellis<br />
	    First Name: David<br />
            Last Name: Ellis<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>  
</ul>  
