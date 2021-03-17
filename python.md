# Python

## ToC 
- [Arithmetic Operations](#aop)
- [Boolean Operations](#bol)
- [String Operations](#sop)
- [List Operations](#lop)

### Arithmetic Operations <a name='aop'></a>

```python
print(a+b)                        # arithmetic operation
print(a-b)                        # subtraction operation
print(a*b)                        # multiplication operation
print(a/b)                        # division operation - gives the quotient(float)
print(a//b)                       # floor division - gives the quotient(whole)
printa(a%b)                       # Modulas division - gives the remainder
print(a**b)                       # exponential - power of  a^b
print(-a)                         # negative value of the stored integer
print(abs(-a))                    # like modulo |a| - always positive value
print(int(2.5))                   # prints only the decimal value not the float value
print(float(a))                   # prints the decimal value of the int
``` 

### Boolean Operations <a name='bol'></a>

```python
and                                # performs and operation
or                                 # performs or opertaion
not                                # performs not operation
```

### String Operations <a name='sop'></a>

```python
a='                  This is a string            ' 
print(a.strip())                  # removes whitespaces before and after the string  
This is a string                  # output of strip()

print("Cyberwr3nch".lower())      # prints everything in the lowercase
cyberwr3nch                       # ouput of lower()

print("cyberwr3nch".upper())      # prints everything in the uppercase
CYBERWR3NCH                       # output of upper()

print("github".startswith("git")) # print boolean if the mentioned string starts with git
print("github".endswith("hub"))   # print boolean if the mentioned string ends with git
print("github".find('it'))        # finds the specifed string and provides its index number
print("github was awesome".replace('was', 'is') # changes was with is

print('-'.join(['F', 'B', 'I'])   # joins the items in the list with the seperator '-'
                                  # >>> lis = ["F", "B", "I"]
                                  # >>> print('-'.join(lis))

print(len('github'))              # prints the length of the string
print("git" in "github")          # returns boolean if the string is found
```

### List Operations <a name="lop"></a>

```python
a = [1,2,3,4]
a.append(5)                       # adds 5 at the ends of the list a; a = [1,2,3,4,5]

a = [1,2,4,5]
a.insert(2, 3)                    # adds 3 in the index 2; a = [1,2,3,4,5]

print([1,2,3,4] + [5])            # concats two lists

a = [7,2,8,4,5]
a.remove(8)                       # removes 8 from the list; a = [7,2,4,5]

a = [7,4,8,1]
sorted(a) | a.sort()               # sorts in ascencding order
sorted(a, reverse=True) | a.sort(reverse=True) # sorts in descending order
sorted(a, key=<value>) | a.sort(key=<value>) # performs sorting based on the specified key value; works for nested lists
```
