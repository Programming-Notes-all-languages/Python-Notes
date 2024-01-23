<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#reading-from-a-file'>Reading from a File</a>
  </li>
  <li>
    <a href='#file-paths'>File Paths</a>
  </li>
  <li>
    <a href='#reading-line-by-line'>Reading Line by Line</a>
  </li>  
  <li>
    <a href='#making-a-list-of-lines-from-a-file'>Making a List of Lines from a File</a>
  </li> 
  <li>
    <a href='#writing-to-a-file'>Writing to a File</a>
  </li>
  <li>
    <a href='#appending-to-a-file'>Appending to a File</a>
  </li>  
  <li>
    <a href='#checking-existence-of-files-and-deleting-files'>Checking Existence of Files and Deleting Files</a>
  </li>             
</ol>
</details>

## Reading from a File
<ul>
  <li>
    <a>Text files can contain massive amounts of data and information.  Reading information from a file is a method in which the program can get data from the txt file</a>
  </li>
  <details>
    <summary>Example Program</summary>
      <ul>
        <pre>
          <code>
            with open("filename.txt") as fileObject:<br />
	            contents = fileObject.read()<br />
            print(contents)<br />
          </code>
        </pre>  
      </ul>  
    </details>   
  <ul>
    <li>
      <a>To be able to do any work with a file, the file first needs to be <em>opened</em>.  The open function takes in one argument, just the name of the file being requested to be opened.  In the example above, Python is trying to open the file called filename.txt that is located within the same directory as the program being worked on.  The open function then returns an object that represents the file's contents.  In this example, the object that stores the file's contents is called fileObject</a>
    </li>
    <li>
      <a>After an object that represents the file's contents has been created, the read() method can then be used to read all the contents of the file and then stores all of the file's contents into one large string</a>
  </ul>
</ul>  

## File Paths
<ul>
  <li>
    <a>When using the open() function, Python looks in the directory where the current Python program is located.  Depending on how you organize the files within directories, sometimes, the location of the file may not be in the same directory as the current Python file.  In order for Python to open files from another directory, the file's <em>file path</em> needs to be provided within the open function</a>
  </li>
  <li>
    <a>A <em>relative file path</em> tells Python the exact location of a file within your system.  The following is an example of a relative file path embedded inside of an open() function: with open("Projects/Python/filename.txt") as f:</a>  
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          with open("Projects/Python/Notes/file.txt") as f:<br />
              for line in f:<br />
                  print(line.strip(), end="")<br />
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            asdf<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
</ul>

## Making a List of Lines from a File
<ul>
  <li>
    <a>One possibility for storing the contents of a file is by storing each line into a single element of a list</a>
  </li>  
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          lines = []<br />
          temp = ""<br />
          <br />
          with open("Projects/Python/Notes/file.txt") as f:<br />
              for line in f:<br />
                  for i in range(len(line)):<br />
                      if line[i] != '\n':<br />
                          temp += line[i] <br />
              lines.append(temp)<br />
              temp = ""  <br /> 
          print(lines)<br />
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            ['a', 's', 'd', 'f']<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
</ul>

## Writing to a File
<ul>
  <li>
    <a>To tell Python to write to a file, a second argument needs to be passed within the open() function.  The argument "w" will overwrite the existing contents of the file.  Basically, "w" deletes all the contents of a file, and then the user can add content to this newly cleared file</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          with open("Projects/Python/Notes/file.txt", "w") as f:<br />
              f.write("Hello")<br />
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            Hello<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details> 
  <ul>
    <li>
      <a>The program above writes to the file found in the directory Notes (where Notes is found in the directory Python, and where Python is found in the directory Projects).  The program writes "Hello" to the file called file.txt</a>
    </li>
    <li>
      <a>In this example above, the function open() has two arguments: the first argument is the filepath of the file that we want to open and the second argument, "w", tells Python that the file should be opened in <em>write mode</em></a>
    </li>  
  </ul>  
  <li>
    <a>Python is only able to write strings to a text file.  So, if you are trying to enter data to a text file that is a type other than a string, then the information must be wrapped around the str() function to temporarily change the variable's data type</a>
  </li>
  <li>
    <a>The write() function does not automatically insert a newline character after the end of the argument's contents.  Because of this, if you plan on writing information to a file on multiple lines, then you must include the newline character within the argument</a>
  </li>    
</ul>  

## Appending to a File
<ul>
  <li>
    <a>Another option to write to a file without overriding all of the file's contents is to open the file in <em>append mode</em>.  Appending to a file allows the user to write to a file, while also keeping the file's contents that were already present upon its opening.  Any new lines appended to the file will be added at the end of the file.  Additionally, if the file is yet to exist, Python will create an empty file with the specified name in the open() function's argument</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          with open("Projects/Python/Notes/file.txt", "a") as f:<br />
              f.write("Hello")<br />
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            Hello<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
  <ul>
    <li>
      <a>If the file "file.txt" already exists, then the string "Hello" will be appended to the end of the file; otherwise, if the file does not exist, then Python will create an empty file called "file.txt" within the specified directory and will append "Hello" to the end of that file</a>
  </li>   
</ul>    

## Checking Existence of Files and Deleting Files
<ul>
  <li>
    <a>To both check the existence of files and to delete files, you need to import the os library.  This is down by simply adding the following line of code into your program: import os</a>
  </li>
  <li>
    <a>The os.path.exists() function is one possible method that can be used to make sure a file exists.  Within the parentheses goes the file's path</a>
  </li>  
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          import os<br />
          <br />
          if os.path.exists("Projects/Python/Notes/main.py") == True<br />
            print("File exists!")<br />
        </code>
      </pre>  
      <details>
      <summary>Output</summary>
        <pre>
          <code>
            File exists!<br />
          </code>
        </pre>  
      </details>
    </ul>  
  </details>
  <li>
    <a>After a file is created, Python can then delete it; in order to do so, the function os.remove() can be used.  The file's path then needs to be</a>
  </li>
  <details>
  <summary>Example Program</summary>
    <ul>
      <pre>
        <code>
          import os<br />
          <br />
          if os.path.exists("Projects/Python/Project14/TextFiles/text.txt"):<br />
              os.remove("Projects/Python/Project14/TextFiles/text.txt")<br />
        </code>
      </pre>  
    </ul>  
  </details>    
</ul>    
