# Basic JavaScript
* Comment code with // or by using /* */
* To initialize variable, use var and end with ;
* You can also initialize and assign at the same time
* Variables usually have first word in lowercase and subsequent words are capitalized
* You can assign variables to strings or integers or float numbers
* You can use +=, -=, *=, or /= when you want to do operation on same variable. This is called augmented [operation](addition, subtraction, multiplication, division)
* Increment or decrement number with ++ or -- following variable
* You can find remainder of variable with modulus(%) 

# Strings
* Strings can be written with single or double quotes. To escape single or double quotes, precede it with \
* One must escape characters with \. 
    * \' - single quote
    * \" - double quote
    * \\ - backslash
    * \n - newline
    * \r - carriage return
    * \t - tab
    * \b - word boundary 
    * \f - form feed
* You can concatenate strings by using the addition sign +
* We can also concatenate with += operator, sort of like augmenting.
* You can insert variable when concatenating strings (string variable + string)
* We can append variables to string using += operator as well
* To find length of string variable, add .length at end of variable
* JavaScript uses zero-based indexing. Bracket notation can get character at specific index of string. 
* One can initalize string variable by just setting it to equal to ""
* String values are immutable in JavaScript. Only way is to reassign whole string variable 
* You can use bracket notation to find nth character in strings
* I can use the .length() function to get last character of string
* Madablibs game to complete strings section

# Arrays
* Arrays can have either numbers, strings, or both
* Arrays can be nested within other arrays, which is called multi-dimensional array
* Acess array by indexing
* Arrays are mutable
* Acess multidimensional array with indexes [][][]
* .push() can be used on arrays to append to end of it. Arrays can be appended to end of it
* .pop() can be used to pop element off end of array. It removes last element and returns it
* .shift() removes the first element of array. Works like how .pop() does

# Functions
* A function can be initialized by using function [name](){[contents]}
* The function can be called by  using function();
* A function can accept parameters
* Variables created without var are within the global scope
* Variables defined with var within function have local scope
* The local variable takes precedence over global variable if within function 
* Use return to send value back from function 
* When the function has no return statement, the returned value is undefined
* I can assigned function(arg) to variable
* To write function for a queue, first use push() and then shift() function

## If/else statement and comparison operators
* Boolean values - true or false (lowercase)
* An if statement can has its condition in parentheses and uses brackets to contain it
* Equality operator is ==
* Strict equality is ===. Unlike equality operator, it does not attempt to convert values being compared to a common type. 
    * 3 == '3' returns true since type conversion if performed
* Type of variable can be determined by using typeof [val]
* Inequality operator is != . Returns opposite value of equality expression
* Strict inequality operator is !== . 
* Greater than operator is > . Greater than or equal to operator is >=
* Less than operator is < . Less than or equal to operator is <=
* Logical and operator && is used to if both of operands are true
* Logical or operator || is used to see if either of operands is true
* Else statement also contained by brackets
* To see which out of multiple conditions are met, use else if (condition){}
* Make sure order of if, else if, else statements is correct
* Golf code was used to practice this section

## Switch statement
* Switch statement can have many case statements. Case executed for first matched case until break.
* Switch statement is contained by brackets. 
* Cases end in break statements. In addition, each case value is followed by a colon
* A default case can be added at the end. It has no case value
* If multiple inputs have same output, it can be represented by not including a break statement in the preceding case statement. The case statement with break statement can indicate that it could be one of the preceding cases.
* Switch statements can be used to replace several else if statements
* Counting cards game was used to test switch statement

# Return
* return can be used to return a comparison (a < b )
* return statement once reached stops function. 

## Objects
* Access objects through properties
* Properties are stored as strings or numbers. Quotes around string can be omitted if it's a single word
* Non-string properties are typecasted as strings
* Access properties of object using dot notation. Can also used bracket notation[]
* Bracket notation is useful when iterating through an object's properties
* Can also use bracket notation when the property's name is collected dynamically during the program execution
* You can update or add properties by using dot or bracket notation
* One can delete object's property by using delete object.property;
* Objects can be thought of as a key/value storage
    * A switch statement can be converted to an object whose property can be found
* 