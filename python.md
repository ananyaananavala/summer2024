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
    - dictonaries = a collection of {key: value} pairs which are ordered and changeable. no duplicates


- definition of lists: a list is a data structure in python that is a mutable, or changeable, ordered sequence of elements.
- why do we use lists: lists are great to use when you want to work with many related values. they enable you to keep data together that belongs together, condense your code, and perform the same methods and operations on multiple values at once.
- what are the use cases of lists: suitable for ordered collections where frequent additions and removals are needed.


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

***code 4***append a name
names = ["anna", "tommy", "ken", "barbie"]

names.append("john")
print(names)

output: 
['anna', 'tommy', 'ken', 'barbie', 'john']

***code 5*** removing an element
names = ["anna", "tommy", "ken", "barbie"]

names.remove("ken")
print(names)

output: 
['anna', 'tommy', 'barbie']

=== Code Execution Successful ===

***code 6*** sorting lists
numbers = [1, 7, 9, 4, 2]

numbers.sort()
print(numbers)

output: 
[1, 2, 4, 7, 9]

=== Code Execution Successful ===

***code 7*** inserting values
names = ["anna", "tommy", "ken", "barbie"]

names.insert(0, "joy")
print(names)

output: 
['joy', 'anna', 'tommy', 'ken', 'barbie']

=== Code Execution Successful ===

- definition of sets: a set is a data collection type used in python for storing multiple items in a single variable. sets in python are unordered and, as such, are not always consistent in the order they get returned.
- why do we use sets: when you need a collection of unique items for fast membership tests.
- what are the use cases of sets: great for collections of unique items, useful for membership testing and set operations.

***code 1*** running through the set
names = {"anna", "tommy", "ken", "barbie"}

for name in names:
    print(name)

output: 
ken
anna
barbie
tommy

=== Code Execution Successful ===

***code 2*** adding a value in the set
names = {"anna", "tommy", "ken", "barbie"}
names.add("joy")
print(names)

output: 
{'ken', 'tommy', 'barbie', 'joy', 'anna'}

=== Code Execution Successful ===

***code 3*** remove an element
names = {"anna", "tommy", "ken", "barbie"}
names.remove("anna")
print(names)

output:
{'barbie', 'ken', 'tommy'}

=== Code Execution Successful ===

***code 3*** combing the two sets 
set1 = {1,5,3,4}
set2 = {1,9,6,2}
union_set = set1.union(set2)
print(union_set)

output: 
{1, 2, 3, 4, 5, 6, 9}

=== Code Execution Successful ===

***code 4*** finding the similar elements between set 1 and set 2
set1 = {1,5,3,4}
set2 = {1,9,6,2}
intersection_set = set1.intersection(set2)
print(intersection_set)

output: 
{1}

=== Code Execution Successful ===

***code 5*** finding the difference from set 1 to set 2
set1 = {1,5,3,4}
set2 = {1,9,6,2}
difference_set = set1.difference(set2)
print(difference_set)

output: 
{3, 4, 5}

=== Code Execution Successful ===

***code 6*** finding the symmetric difference
set1 = {1,5,3,4}
set2 = {1,9,6,2}
symmetric_difference_set = set1.symmetric_difference(set2)
print(symmetric_difference_set)

output: 
{2, 3, 4, 5, 6, 9}

=== Code Execution Successful ===

- definition of tuples: tuples are ordered, unchangable collections of items. items can be of any type.
- why do we use tuples: we use tuples when you need an ordered collection that should not change.
- what are the use cases of tuples: ideal for fixed collections of items that shouldn't change, such as coordinates(gps).

***code 1*** creating a tuple 
student = ("ananyaa", 17, "computer science")
print(student)

output: 
('ananyaa', 17, 'computer science')

=== Code Execution Successful ===

***code 2*** accesing tuple elements
student = ("ananyaa", 17, "computer science")
name = student[0]
age = student[1]
major = student[2]

print(name)
print(age)
print(major)

output: 
ananyaa
17
computer science

=== Code Execution Successful ===

***code 3*** unpacking the element in the tuple
student = ("ananyaa", 17, "computer science")

name, age, major = student

print(name)
print(age)
print(major)

output: 
ananyaa
17
computer science

=== Code Execution Successful ===

- definition of dictonaries: unordered collections of key-value pairs. keys are unique and changeable.
- why do we use dictonaries: when you need a collection of unique keys mapped to values for fast lookups, mostly used for pair values.
- what are the use cases of dictonaries: best for key-value pairs, useful for fast lookups and data mappings.

***code 1*** creating a dictonary
capitals = {"usa" : "washington d.c",
            "india" : "new dehli", 
            "china" : "beijing", 
            "russia" : "moscow"}
print(capitals.get("usa"))

output: 
washington d.c

=== Code Execution Successful ===

***code 2*** asking the code for a country that is not in the list 
capitals = {"usa" : "washington d.c",
            "india" : "new dehli", 
            "china" : "beijing", 
            "russia" : "moscow"}
print(capitals.get("japan"))

output: 
None

=== Code Execution Successful ===

***code 3*** modifying code 2
capitals = {"usa" : "washington d.c",
            "india" : "new dehli", 
            "china" : "beijing", 
            "russia" : "moscow"}

if capitals.get("japan"):
    print("that capital exits")
else: 
    print("that capital doesn't exist")

output: 
that capital doesn't exist

=== Code Execution Successful ===

***code 4*** checking for a capital that exsits in the dictonary
capitals = {"usa" : "washington d.c",
            "india" : "new dehli", 
            "china" : "beijing", 
            "russia" : "moscow"}

if capitals.get("india"):
    print("that capital exits")
else: 
    print("that capital doesn't exist")

output: 
that capital exits

=== Code Execution Successful === 

***code 5*** updating the dictonary
capitals = {"usa" : "washington d.c",
            "india" : "new dehli", 
            "china" : "beijing", 
            "russia" : "moscow"}

capitals.update({"germany" : "berlin"})
capitals.update({"usa" : "alaska"})
print(capitals)

output:
{'usa': 'alaska', 'india': 'new dehli', 'china': 'beijing', 'russia': 'moscow', 'germany': 'berlin'}

=== Code Execution Successful ===

***code 6*** deleting one of the elements
capitals = {"usa" : "washington d.c",
            "india" : "new dehli", 
            "china" : "beijing", 
            "russia" : "moscow"}

capitals.pop("china")
print(capitals)

output: 
{'usa': 'washington d.c', 'india': 'new dehli', 'russia': 'moscow'}

=== Code Execution Successful ===

***code 7*** printing only the keys
capitals = {"usa" : "washington d.c",
            "india" : "new dehli", 
            "china" : "beijing", 
            "russia" : "moscow"}

keys = capitals.keys()
print(keys)

output: 
dict_keys(['usa', 'india', 'china', 'russia'])

=== Code Execution Successful ===

***code 8*** printing only the keys using for statement
capitals = {"usa" : "washington d.c",
            "india" : "new dehli", 
            "china" : "beijing", 
            "russia" : "moscow"}

keys = capitals.keys()

for key in capitals.keys():
    print(key)

output: 
usa
india
china
russia

=== Code Execution Successful ===

***code 9*** printing only values using for statement
capitals = {"usa" : "washington d.c",
            "india" : "new dehli", 
            "china" : "beijing", 
            "russia" : "moscow"}

values = capitals.values()

for value in capitals.values():
    print(value)

output: 
washington d.c
new dehli
beijing
moscow

=== Code Execution Successful ===

***code 10*** printing keys and values using for statement

differences between collections
- mutability(changeable):
      mutable: lists, dictionaries, sets.
      immutable: tuples.
- order:
      ordered: lists, tuples.
      unordered: dictionaries, sets.
- uniqueness:
      unique items: sets, dictionary keys.
      non-unique items: lists, tuples, dictionary values.

***code 11*** printing items in the dictonary
capitals = {"usa" : "washington d.c",
            "india" : "new dehli", 
            "china" : "beijing", 
            "russia" : "moscow"}

items = capitals.items()
print(items)

output: 
dict_items([('usa', 'washington d.c'), ('india', 'new dehli'), ('china', 'beijing'), ('russia', 'moscow')])

=== Code Execution Successful ===

***code 12*** printing items in the dictonary using for statement
capitals = {"usa" : "washington d.c",
            "india" : "new dehli", 
            "china" : "beijing", 
            "russia" : "moscow"}


for key, value in capitals.items():
    print(f"{key} : {value}")

ouput: 
usa : washington d.c
india : new dehli
china : beijing
russia : moscow

=== Code Execution Successful ===

  
- performance
    - lists
         - accessing elements: fast and efficient. you can quickly get any item by its index.
         - appending: adding an item to the end of the list is generally very fast.
         - inserting/removing in the middle: slow. if you add or remove items from the middle, it can take a lot of time because items may             need to be shifted.
    - tuples
         - accessing elements: just as fast as lists.
         - fixed size: since tuples can't be changed (immutable), they are slightly faster for reading data.
         - usage: best for fixed collections of items that don’t need to change.
    - dictionaries
         - lookups: very fast. finding an item by its key takes very little time.
         - insertions/deletions: also very fast. adding or removing key-value pairs is quick.
         - keys: the keys must be unique and hashable (like strings and numbers).
    - sets
         - add/remove/check membership: very fast. adding items, removing items, or checking if an item is in the set is quick.
         - unique items: sets automatically ensure all items are unique.
         - items: the items must be unique and hashable (like strings and numbers).



