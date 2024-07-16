# summer2024
python learned topics and pratices 

ch1: modules, comments and pip
- modules: a module is a file containing code written by 
somebody else (usually) which can be imported and used in our programs. 
- pip: pip is the package manager for puthon you can use pip to install a module on you system
           - pip install flask installs, flask module
- types of modules: there are two types of modules in python
         1. built in modules: pre installed in python
         2. external modules: need to install using pip
             - some examples of build in modules are os, abs, etc...
             - some examples of ecternal modules are tensorflow, flask etc...
ch2: variables and datatypes
a variable is the name given to a memory location in a program for example
a = 30                          --> variables = container to store a value
b = "harry"                     --> keywords = reserved words in python
c = 71.22                       --> identifiers = class/ function/ variable name

data types: primarily these are following data types in python
1. integers
2. floating point numbers
3. string
4. booleans
5. none
python is a fantastic lanuage that automaticallu identifies the type of data for us
a = 71                          --> identifies **a** as class <int>
b = 88.44                       --> identifies **b** as class <float>
name = "harry"                  --> identifies **name** as class <str>

rules for defining a variable name --> also applies to other identifiers
- a variable name contain alphabets, digits and underscores
- a variable name can only start with an alphabet and underscore
- a variable name can't start w/ a digit
- no white space is allowed to be used inside a variablel name

programming: 
       ________________________________________
      |                                        |                       
      |                                        |                             programming --> python
      |                                        |                   
      |               MACHINE                  |         <------------------->         PYTHON
      |                                        |                                     code python : - high level language
      |                                        |                                                   - translates to binary lang.
      |                                        |                                                   - 0's and 1's
      _________________________________________
                         / \

what is python: 
- python is simple and easy
- free and open source
- developed by guido van rossum
- high level
- portables

python character set:
- letters: a to z, A to Z
- digits: 0 - 9
- specail symbols: -, +, *, / etc..
- whitespaces: blank space, tab, carriage, return, newline, formed
- other characters: python can process all ASC II and unicode characters as part of fata or literals

variables: 
- a variable is a name given to a memory location in a program
  name = "ananyaa"
  age = 17
  price = 1,986

memory: 
 _________________________________________________
|       age     price           name             |     
|       17      1,986          ananyaa           |
_________________________________________________
name = "ananyaa"
age = 17          --> integer
price = 25.99     --> floating value

***code 1***
name = "ananyaa"
age = 17
price = 25.99

print(name)                 print("name")
output: ananyaa             output: name

***code 2***
name = "ananyaa"
age = 17
price = 25.99
print("my name is: ", name)
print("my age is: ", age)

output: my name is: ananyaa
        my age is: 17

= is an assignemnt operator

rules for identifiers
1. identifiers can be combination of uppercase and lowercase letters, digits or an underscore (_).
   so myVariable, variable_1, variable_for_print all are valid python identifiers
2. an identifier can not start with digit. so while variable1 is valid, 1variable is not valid
3. we can't use special symbols like !, #, @, %, $ etc... in our identifiers
4. identifiers can be of any length

data types
***code 3***
name = "ananyaa"
age = 17
price = 25.99

print(type(name))
print(type(age))
print(type(price))

output: <class 'str'>
        <class 'int'>
        <class 'float'>

- integers: +ve, -ve, 0
- string: "ananyaa", "hello"
- float: 3.99, 2.50,



- python has 4 built-in data structures that can be used to hold a collection of objects, 
they are list, tuple, set, and dictionary.
- they can be changeable, unchangeable, set type and mapping respectivly
- collection is a single varible used to store muliple values
    - lists = [] ordered and changeable, duplicates are okay
    - sets = {} unordered and unchangeable but, can add or remove elements. no duplicates
    - tuple = () ordered and unchangeable. its faster and duplicates are okay

- definition of lists: a list is a data structure in python that is a mutable, or changeable, ordered sequence of elements.
- why do we use lists: lists are great to use when you want to work with many related values. they enable you to keep data together that belongs together, condense your code, and perform the same methods and operations on multiple values at once.
- what are the use cases of lists: python's list is a flexible, versatile, powerful, and popular built-in data type. it allows you to create variable-length and mutable sequences of objects. in a list, you can store objects of any type. you can also mix objects of different types within the same list, although list elements often share the same type

***code 1*** running through the list
names = ["anna", "tommy", "ken", "barbie"]

for name in names:
    print(name)

output: 
anna
tommy
ken
barbie

=== Code Execution Successful ===

***code 2*** changing one of the elements in the list 
names = ["anna", "tommy", "ken", "barbie"]

names[0] = "arjhun"

for name in names:
   print(name)
   
output: 
arjhun
tommy
ken
barbie

=== Code Execution Successful ===

***code 3*** removing one of the elements
names = ["anna", "tommy", "ken", "barbie"]

names.remove("anna")
print(names)

output: 
['tommy', 'ken', 'barbie']

=== Code Execution Successful ===

***code 3***append a name
names = ["anna", "tommy", "ken", "barbie"]

names.append("john")
print(names)

output: 
['anna', 'tommy', 'ken', 'barbie', 'john']

***code 4*** removing an element
names = ["anna", "tommy", "ken", "barbie"]

names.remove("ken")
print(names)

output: 
['anna', 'tommy', 'barbie']

=== Code Execution Successful ===

***code 5*** sorting lists
numbers = [1, 7, 9, 4, 2]

numbers.sort()
print(numbers)

output: 
[1, 2, 4, 7, 9]

=== Code Execution Successful ===




