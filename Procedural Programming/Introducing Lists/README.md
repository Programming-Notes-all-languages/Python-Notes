<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#what-is-a-list'>What is a List</a>
  </li>
  <li>
    <a href='#accessing-elements-in-a-list'>Accessing Elements in a List</a>
  </li>
  <li>
    <a href='#appending-elements-to-the-end-of-a-list'>Appending Elements to the End of a List</a>
  </li>  
  <li>
    <a href='#inserting-elements-into-a-list'>Inserting Elements to the End of a List</a>
  </li> 
  <li>
    <a href='#removing-elements-from-a-list'>Removing Elements from a List</a>
  </li>
  <li>
    <a href='#sorting-a-list-with-sort-method-and-sorted-function'>Sorting a List with sort Method and sorted Function</a>
  </li>               
</ol>
</details>

## What is a List
<ul>
  <li>
    <a>A <em>list</em> is a collection of items that are in a order specified by the program.</a>
    <ul>
      <li>
        <a>In Python, square brackets ([]) are used to declare a variable as being a list.  The elements of the list are then placed within the brackets, where each element is separated by commas</a>
      </li> 
      <li>
        <a>To declare an empty list, do the following: variableList = []</a>
    </ul>   
  </li>  
  <li>
    <a>A list can be made of variables that are of different types, meaning that a list's elements contain heterogeneous data types and objects</a>
    <ul>
      <li>
        <a>For instance, a single list can contain integers, floats, strings, and booleans</a>
      </li>  
    </ul>  
  </li>  
</ul>

## Accessing Elements in a List
<ul>
  <li>
    <a>Lists are essentially ordered collections.  To be able to access any element in a list, you would need to tell Python the position, also known as the <em>index</em>, of the desired item</a>
  </li>
  <li>
    <a>Python considers the first item in a list to be at position zero, not one like you would conventionally think</a>
  </li> 
  <li>
    <a>Python has a special syntax for accessing elements in a list based on its position relative to the end of the list.  For example, to access the last element of a list, you would do the following: variableList[-1]</a> 
  </li> 
  <li>
    <a>To print all items in a list, you can simply place the list's name within the print function such as in the following: print(variableList)</a>
  </li>  
</ul> 

## Appending Elements to the End of a List
<ul>
  <li>
    <a>An easy way to add a new element to an end of the list is by <em>appending</em> to a list, using the append() method</a>
  </li> 
  <li>
    <a>For example, let's say that the following list has been declared within a program: numList = [1, 2, 3].  If the user wanted to add the number four to the end of the list, the user could do the following: numList.append(4).  Now, the list is the following: [1, 2, 3, 4]
  </li>
</ul>  

## Inserting Elements into a List
<ul>
  <li>
    <a>You can add a new element to a list at any position, also known as index, by using the insert() method.  This can be accomplished by specifying the index of the new element and the value of the new item</a>
  </li>
  <li>
    <a>For example, let's say that we have the same list again that was mentioned in the previous section called numList, where numList = [1, 2, 3].  If we want to add the value zero to the beginning of the list, you would do the following: numList.insert(0, 0)</a>
  </li>
</ul>

## Removing Elements from a List
<ul>
  <li>
    <a>Removing an element from a list, knowing the index of that element, can be done with the del keyword</a>
  </li>
  <li>
    <a>Let's use the example list from the previous sections, numList.  If you wanted to delete the first element of the list, you could do the following: del numList[0]</a>
  </li>
  <li>
    <a>Another method for deleting an element at a specified list is using the pop() method.  If you use the pop() method without specifying the index of the element that you would like to delete, then the last element of a list will get deleted.  Otherwise, the index value that you would put within the parentheses of the pop() method is the index of the list that will be deleted</a>  
  <li>
    <a>Sometimes, you will not know the position of the value you want to remove from a list</a>
    <ul>
      <li>
        <a>The remove() method can be useful when you only know what value you want to have deleted from a list, but you do not know that element's index</a>
      </li>
      <li>
        <a>Let's say the following list has been declared within our program: varList = ['a', 2.2, 5].  If you do not know the index at which the list's element 5 is located, but you would like to remove that element, you could include this line of code into your program to accomplish this task: varList.remove(5)
      </li>  
    </ul>  
  </li> 
</ul>

## Sorting a List with sort Method and sorted Function
<ul>
  <li>
    <a>The sort() method alters the order of a list permanently.  If a list contains only strings, then the sort() method will sort the list in alphabetical order.  If a list contains only numbers, which can be both integers and floats, then the sort() method will sort the list from smallest to largest</a>
  </li>
  <li>
    <a>The sorted() function on the other hand does not change the order of the list permanently.  The sorted() function will only change the order of the list for that line of code only.</a>
  </li>
  <li>
    <a>If a list contains elements that include mixed types, other than a list just of integers and floats, then the sort() method and the sorted() function cannot be used</a>
  </li>
  <li>
    <a>The len() function can be used to find the length, number of elements, in a list.</a>
  </li>  
</ul>        
