# Python
# Day1

Python is a high-level, interpreted programming language known for its simplicity and readability. It was created by Guido van Rossum and first released in 1991. Python emphasizes code readability and allows programmers to express concepts in fewer lines of code compared to other programming languages.



Comments could be used for a wide range of purposes, for example: 

Augmenting program code with basic descriptions to generate external documentation.
Integration with source code management systems and other kinds of external programming tools.

Comments in Python start with the hash character, #, and extend to the end of the physical line.

In [1] : the_world_is_flat = true
if the_world_is_flat:
  print("Be careful not to fall off!")

# this is the first comment
span = 1 # amd this is the second comment
         # ... and now a third
text = "# This is not a correct because it's inside quotes."

# Day 2

Variables and Types
There are several types of variables in Python, including integers, which are whole numbers; floats, which are decimal numbers; complex numbers, which are used for complex mathematical calculations; and strings, which are collections of characters. Booleans, which are true or false values, are another type of variable in Python. When working with strings, the plus sign is used to concatenate them, but it cannot be used to add strings and numbers. Error messages can provide useful information when working with Python.

# Data Structures 
# Lists
ar_list = [1,2,3,4]
    print(ar_list)

# Sets 
ar_set={1,2,3,4}
  print(ar_set)
out(1,2,3,4)

type(ar_set)
out: set

# Operators

Arithmetic operator
+, *, **, /, %

Arithmetic Operators with Strings
 'string 1' + 'string 2'
 out: 'string 1 string 2'

 # Control Flow
 # If / Else statements
  a=true, b=false, c=true
  if a:
      print('It is true')
      print('Also print this')
  if b:
      print('Both are true'
  if b:
      print('All three are true')
  else:
    print('It is false')
    print('Always  print this')

  out:
    It is true
    Also print this
    Always print this

# For loops 

  a = [1, 2, 3, 4]
  for number in a:
      print(number)
  out: 1
       2
       3
       4

 # Functions

 def multiply(val1, val2);
   return val1 *val2
multiply(3, 4)
out: 12

a = [1, 2, 3]
 def appendfour(arList);
 arList.append(4)
appendFour(a)
print(a)
out: [1, 2, 3, 4]

print(print('Hello, World!'))
Hello, World!
None

# Classes 
class Dog:
      def _init_(self, name):
        self.name = name
        self.legs = 4

      def speak(self):
        print(self.name + 'says: Bark!')

my_dog = Dog('Rover')
another_dog = Dog('Fluffy')

my_dog.speak()
Rover says: Bark!

another_dog.speak()
Fluffy says: Bark!



    

    
    



