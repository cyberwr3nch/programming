# Python

## ToC 

- [Arithmetic Operations](#aop)
- [Boolean Operations](#bol)
- [String Operations](#sop)
- [List Operations](#lop)
- [Range ()](#ran)
- [Tuple Operations](#top)
- [If-else Statement](#ies)
- [Python Operators](#pop)
- [Dictionary Operations](#dop)
- [User Interaction and While loop](#uwl)
- [Functions](#fun)
- [Class](#cls)
- [File and Exceptions](#fae)

### Arithmetic Operations <a name='aop'></a>

```python
print(a+b)                                        # arithmetic operation
print(a-b)                                        # subtraction operation
print(a*b)                                        # multiplication operation
print(a/b)                                        # division operation - gives the quotient(float)
print(a//b)                                       # floor division - gives the quotient(whole)
printa(a%b)                                       # Modulas division - gives the remainder
print(a**b)                                       # exponential - power of  a^b
print(-a)                                         # negative value of the stored integer
print(abs(-a))                                    # like modulo |a| - always positive value
print(int(2.5))                                   # prints only the decimal value not the float value
print(float(a))                                   # prints the decimal value of the int
``` 

### Boolean Operations <a name='bol'></a>

```python
and                                               # performs and operation
or                                                # performs or opertaion
not                                               # performs not operation
```

### String Operations <a name='sop'></a>

```python
a='                  This is a string            ' 
print(a.strip())                                  # removes whitespaces before and after the string  
This is a string                                  # output of strip()

print("Cyberwr3nch".lower())                      # prints everything in the lowercase
cyberwr3nch                                       # ouput of lower()

print("cyberwr3nch".upper())                      # prints everything in the uppercase
CYBERWR3NCH                                       # output of upper()

print("i am a geek".title())                      # prints everything in title format
Im A Geek                                         # output of title()

iam = "cyberwr3nch"                               # variable with the name "iam" and value 'cyberwr3nch'
print(f" I am {iam}")                             # subsituting the value with f"" format
print("I am {}".format(iam))                      # subsituting the values with format()
I am cyberwr3nch                                  # output of formating, string operations such as title()/upper()/lower() can be performed 

print("github".startswith("git"))                 # print boolean if the mentioned string starts with git
print("github".endswith("hub"))                   # print boolean if the mentioned string ends with git
print("github".find('it'))                        # finds the specifed string and provides its index number
print("github was awesome".replace('was', 'is')   # changes was with is

print('-'.join(['F', 'B', 'I'])                   # joins the items in the list with the seperator '-'
                                                  # >>> lis = ["F", "B", "I"]
                                                  # >>> print('-'.join(lis))
                                                  # >>> F-B-I

print(len('github'))                              # prints the length of the string
print("git" in "github")                          # returns boolean if the string is found

a = "This is a line"
print(a.split())                                  # splits the words on space; ['This', 'is', 'a', 'line'] 
```

### List Operations <a name="lop"></a>

```python
a = []                                            # empty list
a = [1,2,3,4]                                     # list declaration

print(a[2])                                       # prints the elemet 3, index of lists starts with 0
a.append(5)                                       # adds 5 at the ends of the list a; a = [1,2,3,4,5]

a = [1,2,4,5]
a.insert(2, 3)                                    # adds 3 in the index 2; a = [1,2,3,4,5]

print([1,2,3,4] + [5])                            # concats two lists

a = [7,2,8,4,5]
a.remove(8)                                       # removes 8 from the list; a = [7,2,4,5]

a = [7,4,8,1]
sorted(a) | a.sort()                              # sorts in ascencding order
sorted(a, reverse=True) | a.sort(reverse=True)    # sorts in descending order
sorted(a, key=<value>) | a.sort(key=<value>)      # performs sorting based on the specified key value; works for nested lists

for i in a:                                       # iterate throught the list and print the lists contents
        print(i)     

a = [1,2,3,4,5]
print(a[0:2])                                     # print items with index range 0-2 from the list; index 2 is discarded in the output; Output: 1,2
print(a[:3])                                      # print items from 0 - 2; Output: 1,2,3
print(a[2:4])                                     # print items from index range 2 - 4; Output: 3,4
print(a[3:])                                      # print items from index 3 to end of the list; Output: 4,5

a = [1,2,3,4]
b = a[:]                                          # copies the contents of the list a to list b
```

### Range () <a name="ran"></a>

```python

print(list(range(1,6)))                           # sudden list of numbers from 1 - 6

print(list(range(1,10,2)))                        # print from numbers 1 - 10 with a hop of 2, = 1, 3, 5, 7, 9
```

### Tuple Operations <a name="top"></a>

```python
a = ()                                            # empty tuple
a = (1,2)                                         # tuple declaration

print(a[0])                                       # accessing tuple values
                                                  # tuples values cannot be changed
```

### IF-Else Statements <a name='ies'></a>

```python
if (condition):                                   # IF Loop declaration
        #code-suite
        pass

if (condition):                                   # IF-Else Loop declaration
        #code-suite
        pass
else:
        #code-suite
        pass


if (condition):                                   # IF-Elif-Else Loop declaration; Nested IF ELSE CONDITION
        #code-suite
        pass
elif (condition):
        #code-suite
        pass
else:
        #code-suite
        pass
```

### Python Operators <a name='pop'></a>

```python
=                                                 # equal to
<                                                 # less than
>                                                 # greater than
!=                                                # not equal to
<=                                                # less than or equal to
>=                                                # greater than or equal to
< and >=                                          # multiple condition checks with the booelan operators
```

### Dictionary Operations <a name='dop'></a>

```python
a = {}                                            # empty dictioniary
dic = {'language': 'python', 'difficulty': 'easy'}# dictionary declaration; syntax: dict_name = {"key1": "value1", "key2": "value2"}
print(dic['language'])                            # accessing dictionary with key

dic['author'] = "Guido van Rossum"                # adding new key and value to the dictonary dict
dic['difficulty']  = 'Medium'                     # Key's value can be changed with the assignement operator(=)
del dic['difficulty']                             # removes the key vale pair 'difficulty' from the dictionary

for key, value in dic.items():                    # the dictonary values can be iterated with items()
        print(f"Key: {key}\n")
        print(f"Values: {value}")

for keyName in dic.keys():                        # prints just the key name 
        print(keyName)

for keyName in sorted(dic.keys()):                # prints key names in sorted order
        print(keyName)

for value_items in dic.value():                   # prints the values of the key
        print(value_items)

nl = []                                           # initializing an empty list
new_dict = {'key': 'val1', 'key2': 'val2'}        # assigning the dictionary with the values
nl.append(new_dict)                               # appending the dictionary to the list

new_dict = {'name': 'cyberwr3nch', 'prog-lang': ['c', 'python']} # adding lists in the dictionary
print(new_dict['name'])                           # accessing value with key
for prog in new_dict['prog-lang']:                # iterating through tht list and accessing the values
        print(f"{prog}\n")

students = {                                      # nested dictionary
        "dhanesh": {                              # dic = {"key":"Value", "key", "value"}
                "f_name": "dhanesh",              # nested_Dic = {"key":{"akey1":"avalue1", "akey2":"avalue2"}, "key2": {"bkey1": "bvalue1" }}
                "l_name": "sivasamy",
                "role": "average student"
        },
        "cyberwr3nch": {
                "f_name": "cyberwr3nch",
                "l_name": "cyber",
                "role": "moderate student"
        },
        "damnedsec": {
                "f_name": "dsec",
                "l_name": "security",
                "role": "average student"
        }
}

for stud_name, stud_details in students.items():
        print(f"{stud_name}\n")
        print(f"{stud_details['role']}")          # accessing the value's, Value
```

### User Input and While loop <a name='uwl'></a>

```python
variable = input("Provide input: ")               # string input method with the message "Provide input: "
variable = int(inpur("Enter num: "))              # integer input method with the messageg "Enter num: "

while (condition):                                # while loop declaration
        #code-suite
        pass

while True:                                       # infinite loop
        #code-suite
        pass

while True:                                       # stop an infinite loop based on the conditions
        if (condition):
                #code-suite
                break
        else:
                pass
```

### Functions <a name='fun'></a>

```python
def func_name():                                  # function declaration
        #code-suite
        pass
func_name()                                       # calling a function, which triggers the code suite inside the function

def func_name(arg1):                              # function declaration with an input to the function
        #code-suite
        print("Hello {arg1}")
func_name("cyberwr3nch")                          # passing argument to the function with the function call

def func_name(*args):                             # accepts any numbers of arguments being passed to the function
        #code-suite
        pass

def func_name(first, last, **user_info):          # **user_info, accepts the key valued pair as an input
        #code-suite
        pass
user_profile = func_name("Dhanesh","Sivasamy",  location="cbe", role="student")                   # Dhanesh being firstname, Sivasamy being second name, the keyed values locationa and role are accepted by the **user_info argument
```

### Classes <a name='cls'></a>

```python
class class_name:                                 # class initialization
        #code-suite

class class_name:       
        def __init__(self):                       # constructor declaration, the __init__() always takes "self" as its first arguemnt
                                                  # we can assign variables for the inistantiated classes
                #code-suite
                pass

class class_name:
        def __init__(self):                       # we can initialize values for the object with self.<varname>=value
                self.name = "cyberwrn3ch"
                self.role = "student"
        
        def out(self):
                print(f"Hi {self.name}, I recon you are a {self.role}")

eggs = class_name()                               # when calling the function without providing an argumet it automaticalls assigns the variables from the __init__()
eggs.out()                                        # calling the function to output the result; class_obj.method(): OUTPUT: Hi cyberwrn3ch, I recon you are a student
                                                  # when a variable/ value is mentioned in the __init__(self, value1), an variable is required when initializing an instance of the class
                                                  # when another method in the class inherits the created object with "self" keyword, [HERE: The created object is passed to the out() inside the class], It passes the total no. of created / assigned values to the method, which makes us able to mention the values of self.name and self.role

eggs.role="master"                                # The values assigned by the __init__() can be modified by addressing them
eggs.out()

class cls_child(class_name):                      # implementing inheritance, the cls_child becomes the child class of the class class_name. Meaning cls_child have all the methods in the class_name
        def __init__(self):                       # super() calls the method specified in the parent class
                super().__init__(name, role)         
```

### File And Exceptions <a name='fae'></a>

```python

with open('filename') as file_object:             # open a file and read its contents
        file_object.read()

with open('filename') as file_object:
        file_object.readlines()                   # reads the file line by line

with open('filename', 'w') as file_object:        # opening a file in write mode
        file_object.write('cyberwr3nch')          # writing the desired stuff to the file
        file_object.close()                       # closing the file
```

```python

# EXCEPTIONS

print(2/0)      # ZeroDivisionError: division by zero, program stops
# handling the exceptions with try/except

try:
        print(2/0)
except ZeroDivisionError:
        print("You cannot divide by 0")

with open("iammaster.txt")  #FileNotFoundError: [Errno 2] No such file or directory: 'iammaster.txt' 

try:
        with open(filename, encoding='utf-8') as f:
        contents = f.read()
except FileNotFoundError:
        print(f"Sorry, the file {filename} does not exist.")
```
