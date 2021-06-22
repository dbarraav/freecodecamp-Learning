# Notes
## Why Program?
* Programmers anticipate needs
* Computer = hardware and software

## Hardware Architecture
* Input Devices: keyboard, mouse, and touch screen
* Output Devices: screen, speakers, printer, DVD burner
* Software:
    * Central Processing Unit- runs the program
    * Main Memory: fast small temporary storage
* Secondary Memory(Hard Drive): slower large permanent storage

* Python is translated to machine language before transferred to main memory and eventually CPU

## Python as a Language
* Syntax Errors: Always continue learning

## Elements of Python
* There are some words that are reserved and cannot be used as variable names/identifiers
* Script is a just a file that can be used to run Python code rather than doing so interactively through command line
* There are three types of steps: sequential, conditional, and repeated

## Variables, Expressions, and Statements
* Constants as fixed values
* Variables are named places where data is stored for later retrieval
* Variables must start with letter of underscorea and consist of letters, numbers, and underscores. They should also be case sensitive

## Intermediate Expressions
* Type of variable matters
    * type()
    * bool(), int(), float(), str()
* Order of operations - PEMDAS and left to right
* Input function is input()

## Conditional Execution
* Comparison operators
* Indentation is necessary
* Nested decisions
* Visualize blocks

## More Conditional Structures
* elif statement
* Try and except structure
    * Code in try works if accepted. Else, code in except block is accepted

## Python Functions
* def creates function
    * Built-in functions
        * Type conversions
        * String conversions

## Build your own Functions
* First define and then invoke/call functions
* return keyword is used to exit function and return value of function

## Loops and Iterations
* while loop(aka indefinite loops) runs until condition is False
* break statement can be used to exit out of loop
* continue statement can be used to skip the current iteration

## Definite Loops
* for loop(aka definite loop)

## Loop Idioms
* Make smart loops

## More Patterns
* Counter variable
* Sum variable
* Loop used for finding average, filtering, searching for boolean variable, finding min/max value
* is statement is much stronger than using ==.
    * 0 == 0.0 is considered True
    * 0 is 0.0 is considered False

## Strings in Python
* String is sequence of characeters
* Uses ' or " 
* For strings, + means concatenate
* Read data using strings before converting to integers/floats

## Intermediate Strings
* Use colon operator to select characters within string
* in keyword can also be used to check if a letter or string is in another string
* String comparison: each character is compared. If characters are different, Unicoode value is compared. Character with lower Unicode value is considered smaller. 
* String functions can be called by appending a "." and "function()"
    * upper(), lower(), lstrip(), rstrip(), strip()
* dir() can be used to list the functions of variable of specific type
* In Python 3, all strings are Unicode

## Reading Files
* open() function returns file handle 
    * mode argument determines whether one is reading or writing to file
* A new line can be indicated with \n
* print() automatically adds \n at end
* A text file can be regarded as newlines at end of each new line

## Files as a Sequence
* File handle can be considered sequence of strings with each line being a string
* rstrip() can be used to remove "white space"(\n is considered white space)
* Can use try and except structure to deal with bad file names

## Python Lists
* Algorithms: set of rules or steps used to solve a problem
* Data Structures: a particular way or organizing data in a computer
* What is not a Collection? A variable is not a collection
* A list is a kind of collection 
    * A list element can be put into another Python object, such as a list
* Use square brackets to specify element in list
* Strings are immutable, but lists are mutable
* Use len() to tell number of elements in list 
* range() function returns list of numbers from 0 to one less than the argument in range()

## Working with Lists
* Concatenate lists with + 
* Lists can be sliced wtih :
* An empty list can be made with list()
* Can use in and not in operators to check if something is in list 
* A list can be sorted with sort() function

## Strings and Lists
* split() functions breaks string into list of separate strings from original strings with spaces gone
* argument within split() function can be used as delimiter. Default delimiter is space

## Python Dictionaries
* Dictionaries allow for fast database-like operations in Python
* Dictionaries are known as properties or Map or Hashmap in Java
* Dictionaries have no order. Each key has its own value
* Empty dictionaries can be created with curly brackets

## Dictionaries: Common Applications
* Common use of dictionary is for counters
* An error is shown if referenced key is not in dictionary
    * Use in operator to see if key is in the dictionary
* get() is method to check if key is in dictionary and if not, set a default value

## Dictionaries and Loops
* To count words in line of text, split the line into words and then use dictionary to keep count
* Looping through a dictionary considers iteration variable as key
* Append .keys(), .values(), or .items() to retrieve keys, values, or both from dictionaries
* We can use two iteration variables( 1st var is for key and 2nd var is for value) to go through dictionary

## The Tuples Collection
* Tuples are like a list. They are indexed starting at 0. 
* Tuples are immutable
* Only certain functions are available to tuples since they are immutable
* Tuples are simpler and more efficient in terms of memory use and performance than lists
* When we are making "temporary variables", we prefer tuples over lists
* Tuples can be put on left-hand side of assignment statement
* The items() function of dictionaries return list of tuples
* Comparison operators work with tuples 

## Comparing and Sorting Tuples
* Use sorted() function to sort items/tuples into correct order for dictionary
* Can also sort by values instead of keys
* List comprehension can be used for a shorter version of code

