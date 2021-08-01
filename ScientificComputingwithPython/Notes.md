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

## Regular Expressions
* A regular expression, aka a "regex" or "regexp", provides a concise and flexible means for matching strings of text.
* A smart "find" or "search"
* Very powerful and cryptic. 
* Before using regular expressions, import re
    * Use re.search() to see if string matches a regular expression. Similar to find()
    * Use re.findall() to extract portions of a string that match regular expression. Similar to combination of find() and slicing()
* Wild-Card characters: dot character matches any character
    * Look up guide for regular expressions
* Can fine-tune match, depends on how "clean" data is and purpose of application

## Regular Expressions: Matching and Extracting Data
* re.search() returns a T/F depending on whether string matches reuglar experssion 
* If we actually want the matching strings to be extracted, we us re.findall()
* Greedy Matching: when it can match any two strings, it will match longer string. 
* Non greedy matching: you can add ? character to chill on + and * 
* Fine-tuning strinrg extraction: one can add paranthesis to not include white space in returned string

## Regular Expressions: Practical Applications
* One can use ".find()" to extract host name
* Another method was to use ".split()". One print specific piece of string by choosing element of list outputed. 

## Networking with Python
* Free book: "Introduction to Networking: How the internet works" by charles R Severance
* Easy to read book(made for high schoolers)
* Transport Control Protocol(TCP)
* Layers(bottom to top): link, internet, transport, application
* TCP Connections==Sockets- endpoint of bidirectional inter-process communication flow across an internet protocol-based computer networks
* TCP Port numbers - port is an application-specific or process-specific software communications endpoint 
* Protocols can be in different ports
* Common TCP Ports(Extensions): Telnet, SSH, HTTP, HTTPS, and others
* Python allows one to talk to sockets with "socket" library. Call socket function
* Now that we have socket, what data can we send and receive across socket?

## Networking Protocol
* Socket functions to connect our TC to server TC
* Application protocol is what we're gonna send or receive to a socket
* HTTP - Hypertext Transfer Protocol:
    * This is the dominant application layer protocolo on internet
* A protocol is set of rules that all parties follow so we can predict each other's behavior
* Protocol, host, and document - (http://)(www.dr-chuck.com/)(page1.html)
* Getting data from server:
    * User clicks anchor tag with href
    * Browser makes connection to web server and issues "GET" request
    * Server returns HTML document to the Browser, which formats and displays document to user
* Request/Response Cycle - governed by internet standards. These stanards are for internet protocols and established by IETF
* Standards are called RFCs

## Write Web Browser
* First import library socket. Then make socket and connected to webserver with ".connect()"
* After, send with ".send()"
* We can then receive with ".recv()" with while loop. When we take in data, we also decode it.

## Networking: Text Processing
* We can use ord() function to get bits used to represent a character
* UTF-8 has dynamic length(1-4 bytes). Recommended practice for encoding data
* In Python 3, bytes are different. All strings are internally UNICODE
* When we take about network socket, we need to encode strings. We need to decode it when we receive it
* We encode and then send or receive and decode. 

## Networking: Using urllib in Python
* Import urllib.request. This library does all socket work for us and makes web pages look like file
* Returns object that looks like filehandle
* Data must be decoded and then ".strip()" can be used

## Networking: Web Scraping with Python
* Web scraping is when program or script pretends to be webpage in order to get information from webpages
* Why scrape? Nonitor site for new info, spider web to make database. 
* BE CAREFUL ABOUT WHICH WEBSITES ALLOW WEB SCRAPING
* One library used for scraping from html documents is called BeautifulSoup

## Using Web Services
* Commonly used formats: XML and JSON
* Wire protocol needs to be agreed upon. One could send data from one programming language to another programming language.

## Web Services: XML
* XML stands for eXtensible Markup Language
* Purpose is to help info systems share structured data
* Tags, attributes, serialization/deserialization
* Start tag, end tag, text content, attribute, and self closing tag
* White space don't matter in text content
* Simple and complex elements. Think of XML as a tree or made up of paths

## Web Services: XML Schema
* XML Schema is description of legal format of an XML document
* Used to define contract between systems, meaning there are constraints on structure and content of docs
* XML validator has inputs of XML document and XML Schema Contract
* Common language of XML Schema is XSD(There are more)
* Date/Time Format (ISO 8601)
* Import xml.etree.ElementTree as ET <--Import this library
* GO OVER THIS AGAIN TO BETTER UNDERSTAND

## Web Services: JSON
* JSON representes data as neste "lists" and "dictionaries"
* Import json as library. Result of json.loads(data) is a dictionary

## Web Services: Service Oriented Approach
* A service oriented approach is when data is stored across systems connected via internet or internet network
* Services publish rules applications must follow to make use of service(API)
* First two systems work together. As service becomes more useful, multiple applications want to use info/application 

* Web Services: API
* Application Program Interface specifies interface and controls behavior of objects in interface
* Should read documentation of APIs
* GO OVER THIS AGAIN TO BETTER UNDERSTAND

## Web Services: API Rate Limiting and Security
* Some APIs are free, others are not 
* More requests can be obtained with key
* Some APIs will require you to have account
* Key authorization for security

## Python Objects
* Object oriented is self-contained code and data
* Different type of objects(string, integer, dictionary objects)
* Objects hide details
* Class-template, method-defined capability of class, field/attribute - bit of data in class, object/instance-instance of class

## Objects: A Sample class
* class PartyAnimal   <----(example)
* dir() command lists capabalities

## Object Lifecycle
* Objects are created, used, then discarded
* Constructors and destructors
* Constructor to set up instance variables
* Both constructors and destructors asre optional in class definition. 
* Destructors are seldom used, unlike constructor
* We can have multiple instances of class, each of which has their own instance variables

## Objects: Inheritance
* 