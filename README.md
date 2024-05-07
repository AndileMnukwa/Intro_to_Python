# Python
# Week 1

Python is a high-level, interpreted programming language known for its simplicity and readability. It was created by Guido van Rossum and first released in 1991. Python emphasizes code readability and allows programmers to express concepts in fewer lines of code compared to other programming languages.

# this is the first comment
span = 1 # amd this is the second comment
         # ... and now a third
text = "# This is not a correct because it's inside quotes."

# Variables and Types
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

# Day 3

# Ints and Floats
input: 20/4
out  : 5.0

input: int(4**4.0)
out  : 256

input: int(8.99999)
out  : 8

input: round(1.2 - 1.0, 2)
out  : 0.2

integers, decimals, booleans(Casting Booleans) 

# strings
slicing 
    myList = [1, 2, 3, 4, 5]
        myList[2:4]
    out: [3, 4]
    
formatting 
    f'My number is: '+str(5)
    out: 'My name is: 5'

    f'Pi is: {math.pi:.2f}'
    out: 'Pi is: 3.14'

    f'Pi is: {}'.format(math.pi)
    out: 'Pi is: 3.141592653589793'

Multi-line Strings
      myString = '''
      Here is a long block of text
      I can add newlines!
      the text doesn't stop until it sees \'\'\'

      '''

      myString
      "\Here is a long block of text\nI can add newlines!\nthe text doesn't stop until it sees '''\n\n"

output: print(mystring)

      Here is a long block of text
      I can add newlines!
      the text doesn't stop until it sees '''

# bytes
  In: bytes(4)
  out: b'\x00\x00\x00\x00'

  In: smileBytes = bytearray('😊', 'utf-8')
  out: '😊'

 # If and Else

 # 1, 2, Fizz, 4, Buzz, 7, 8, Fizz, Buzz, 11, Fizz, 13, FizzBuzz, 16

for n in range(1, 101):
    if n % 15 == 0:
        print('FizzBuzz')
    else:
        if n % 3 == 0:
            print('Fizz')
        else:
            if n % 5 == 0:
                print('Buzz')
            else:
                print(n)

output:

 
1
2
Fizz
4
Buzz
Fizz
7
8
Fizz
Buzz
11
Fizz
13
14
FizzBuzz   

# Whileloops
from datetime import  datetime

wait_until = datetime.now().second + 2
while datetime.now().second != wait_until:
    1 + 1

print(f'We are at {wait_until} seconds!')

output:
         We are at 35 seconds!

# For

animalLookup = {
    'á': ['aardvark', 'antelope'],
    'b': ['bear'],
    'c': ['cat'],
    'd': ['dog'],
}

for letter, animals in animalLookup.items():
    pass
for letter, animals in animalLookup.items():
    if len(animals) > 1:
        continue
    print(f'Only one animal! {animals[0]}')

for letter, animals in animalLookup.items():
    if len(animals) > 1:
        print(f'Found {len(animals)} animals: {animals}')
        break

output:
Only one animal! bear
Only one animal! cat
Only one animal! dog
Found 2 animals: ['aardvark', 'antelope']

# Faster finding primes solution

def allPrimesUpTo(num):
    primes = [2]
    for number in range(3, num):
        sqrtNum = number ** 0.5
        for factor in primes:
            if number % factor == 0:
                # Not prime
                break
            if factor > sqrtNum:
                # It's prime!
                primes.append(number)
                break
    return primes

if __name__ == "__main__":
    # Testing the function
    print(allPrimesUpTo(10))
    print(allPrimesUpTo(100))

# Week 2

# AnatomyOfAFunction
# Named Parameters 

def performOperation(num1, num2, operation='sum', message='Default message'):
         print(message)
         if operation == 'sum':
                  return num1 + num2
         if operation == 'multiply':
                  rewturn num1 * num2
         performOperation(2, 3, message='A new message',operation='multiply'

         output: 
                   A new message 
                   6

# **kwargs
def performOperation(*args, operation='sum'):
         if operation == 'sum':
                  return sum(args)
         if operation == 'multiply':
                  return math.prod(args)
         performOperation(1,2,3, 7, 8, opration='sum'
output: 27

# Function Scope
def performOperation(*args, **kwargs):
         print(args)
         print(kwargs)
performOperation(1, 2, operation='sum')
 (1, 2)
 {'operation': 'sum'}

 # Global and Local scope

message = 'Some global data'
def funtion1(varA, varB):
         print(message)
         print(locals())

def function2(varC, varB):
         print(message)
         print(locals())
function1(1, 2)
function2(3, 4)

output: Some global data
         {'varA': 1, 'varB': 2}
         Some global data
         {'varC': 3, 'varB': 4}

# Variables as Functions
         x = 5
          def x():
          return 5
# Functions are not unique or special in Python — they are simply variables associated with some data.

# Lambda Functions
input: 2 + 3
output: 5

myList = [{'num': 3}, {'num': 2}, {'num': 1}]
sorted(myList.key=lambda x: x['num'])

output: [{'num': 1), {'num': 2}, {'num': 3}]

    
    



