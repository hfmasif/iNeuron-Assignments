### Q26. What is a string? How can we declare string in Python?




```python
# String is collection of texts/characters.

str_var = 'Hello Asif'
```

### Q27. How can we access the string using its index?




```python
# By using index number inside the [] brackets
```

### Q28. Write a code to get the desired output of the following

###### string = "Big Data iNeuron"
###### desired_output = "iNeuron"


```python
string = "Big Data iNeuron"
print(string[ 9 : ])
```

    iNeuron
    

### Q29. Write a code to get the desired output of the following

###### string = "Big Data iNeuron"
###### desired_output = "norueNi"


```python
string = "Big Data iNeuron"
print(string[ -1 : 8 : -1 ])
```

    norueNi
    

### Q30. Resverse the string given in the above question.




```python
print(string[ -1 : : -1 ])
```

    norueNi ataD giB
    




### Q31. How can you delete entire string at once?




```python
del string
```

### Q32. What is escape sequence?
Escape sequences allow you to include special characters in strings. 
To do this, simply add a backslash \ before the character you want to escape.


```python
str = 'What\'s up ?'
print(str)
```

    What's up ?
    

### Q33. How can you print the below string?

'iNeuron's Big Data Course'



```python
str = 'iNeuron\'s Big Data Course'
print(str)
```

    iNeuron's Big Data Course
    

### Q34. What is a list in Python?

A list is a data structure in Python that is a mutable or changeable, ordered sequence of elements. Each element or value that is inside of a list is called an item. Just as strings are defined as characters between quotes, lists are defined by having values between square brackets[]

List are used to store multiple items in a single variable.

### Q35. How can you create a list in Python?




```python
list_var1 = []
print(list_var1)
print(type(list_var1))

list_var2 = [100,200,300,400,500]
print(list_var2)
print(type(list_var2))
```

    []
    <class 'list'>
    [100, 200, 300, 400, 500]
    <class 'list'>
    

### Q36. How can we access the elements in a list?

By using for loop or using indexing

# Q37. Write a code to access the word "iNeuron" from the given list.

lst = [1,2,3,"Hi",[45,54, "iNeuron"], "Big Data"]



```python
lst = [1, 2, 3, "Hi", [45, 54, "iNeuron"], "Big Data"]

print(lst[4][2])
```

    iNeuron
    

# Q38. Take a list as an input from the user and find the length of the list.




```python
x = list(map(int, input("enter multiple value ").split()))
print(x)
print(type(x))
print(len(x))

```

    enter multiple value 1 4 7
    [1, 4, 7]
    <class 'list'>
    3
    

# Q39. Add the word "Big" in the 3rd index of the given list.
 lst = ["Welcome", "to", "Data", "course"]




```python
lst = ["Welcome", "to", "Data", "course"]
lst.insert(2, "Big")
print(lst)
```

    ['Welcome', 'to', 'Big', 'Data', 'course']
    

# Q40. What is a tuple? How is it different from list?
Tuple is a another data structure in python. list is mutable but tuple is not. When tuple is declared it will be unchangable but we can change/update elements in list.


# Q41. How can you create a tuple in Python?




```python
tuple_var1 = ()
print(type(tuple_var1))

tuple_var2 = (10,20,30,15,11)
print(tuple_var2)
```

    <class 'tuple'>
    (10, 20, 30, 15, 11)
    

# Q42. Create a tuple and try to add your name in the tuple. Are you able to do it? Support your answer with reason.

Not able to do that. Because tuple does not support any editing or assigning values after creating once.


```python
tuple_name = ()
tuple_name.append('Asif')
print(tuple_name)
```


    ---------------------------------------------------------------------------

    AttributeError                            Traceback (most recent call last)

    Input In [119], in <cell line: 2>()
          1 tuple_name = ()
    ----> 2 tuple_name.append('Asif')
          3 print(tuple_name)
    

    AttributeError: 'tuple' object has no attribute 'append'


# Q43. Can two tuple be appended. If yes, write a code for it. If not, why?

No. Tuple is used only when we know the exact value or any constraint value which has possibilities to not change after execution. So append or any kind of mutability is not supported in tuple  


```python
tuple1 = (1,2,3,4,5,6)
tuple2 = (9,8,7,6,5,4)
tuple1.append(tuple2)
print(tuple1)
```


    ---------------------------------------------------------------------------

    AttributeError                            Traceback (most recent call last)

    Input In [120], in <cell line: 3>()
          1 tuple1 = (1,2,3,4,5,6)
          2 tuple2 = (9,8,7,6,5,4)
    ----> 3 tuple1.append(tuple2)
          4 print(tuple1)
    

    AttributeError: 'tuple' object has no attribute 'append'


# Q44. Take a tuple as an input and print the count of elements in it.




```python
tuple_input = tuple(map(int, input("Enter values as a tuple: ").split()))
print(tuple_input)
print(type(tuple_input))
```

    Enter values as a tuple: 4 5 6 4
    (4, 5, 6, 4)
    <class 'tuple'>
    

# Q45. What are sets in Python?

 A SET is an unordered collection data type that is iterable, mutable and has no duplicate elements. Python's set class represents the mathmetical notion(concept) of a set. This is based on a data structure known as a hash table.


# Q46. How can you create a set?




```python
set_var = set()
print(type(set_var))
```

    <class 'set'>
    

# Q47. Create a set and add "iNeuron" in your set.




```python
set_var = set()
set_var.add('iNeuron')
print(set_var)
```

    {'iNeuron'}
    

# Q48. Try to add multiple values using add() function.




```python
set_var = set()

set_var.add(10)
set_var.add(30)
set_var.add('Asif')
set_var.add(201)
set_var.add(51.51)

print(set_var)
```

    {201, 10, 51.51, 'Asif', 30}
    

# Q49. How is update() different from add()?

update() function is used when we need to change or modify the set. On the other hand, add() is used for adding new elements into the set. 

# Q50. What is clear() in sets?

clear() remove the entire elements in the set.


```python
thisset = {"apple", "banana", "cherry"}

thisset.clear()

print(thisset)

```

    set()
    

# Q51. What is frozen set?

The frozenset() function returns an unchangeable frozenset object (which is like a set object, only unchangeable).

###### systax: fozenset(iterable)
#(iterable) object can be list,tuple,set etc


```python
mylist = ['one', 'two', 'three']
x = frozenset(mylist)
print(x)
```

    frozenset({'two', 'one', 'three'})
    


```python
#if try to change anything into frozenset it will give error
mylist = ['one', 'two', 'three']
x = frozenset(mylist)
x[1] = 'update_two'
print(x)
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    Input In [136], in <cell line: 4>()
          2 mylist = ['one', 'two', 'three']
          3 x = frozenset(mylist)
    ----> 4 x[1] = 'update_two'
          5 print(x)
    

    TypeError: 'frozenset' object does not support item assignment


# Q52. How is frozen set different from set?

In set() we can add elements but frozenset() is unchangable

# Q53. What is union() in sets? Explain via code.

union() means common and uncommon values both from given elements


```python
set_a = {1,2,3,4,5}
set_b = {6,2,4,5,6,1,1,9}
print(set_a.union(set_b))
```

    {1, 2, 3, 4, 5, 6, 9}
    

# Q54. What is intersection() in sets? Explain via code.

insertsection() returns only common values


```python
set_a = {1,2,3,4,5}
set_b = {6,2,4,5,6,1,1,9}
print(set_a.intersection(set_b))
```

    {1, 2, 4, 5}
    

# Q55. What is dictionary in Python?

######  It has keys and values
###### Support indexing
###### it can consists various type of datatype

# Q56. How is dictionary different from all other data structures.

Because it has seperate keys and values. For accessing or any kind of operation we can use these keys and perform our operation through dictionary.

# Q57. How can we delare a dictionary in Python?




```python
dict_var = {}
print(type(dict_var))
```

    <class 'dict'>
    

# Q58. What will the output of the following?

###### var = {}
###### print(type(var))


```python
# output : <class 'dict'>
```

# Q59. How can we add an element in a dictionary?




```python
var_dict = {}

var_dict['key'] = 'Value'

print(var_dict)
```

    {'key': 'Value'}
    

# Q60. Create a dictionary and access all the values in that dictionary.




```python
var_dict = {'name':'Asif', 'age':25, 'gender':'M', 'marital_status':'Sinle'}

print(var_dict['name'])
print(var_dict['age'])
print(var_dict['gender'])
print(var_dict['marital_status'])
```

    Asif
    25
    M
    Sinle
    

# Q61. Create a nested dictionary and access all the element in the inner dictionary.




```python
nested_dict = {'name':'Asif', 
               'age':25, 
               'gender':'M', 
               'other_information':{'location':'Dhaka', 'hometown':'Gazipur'}, 
               'marital_status':'Sinle'}

print(nested_dict['other_information'])
```

    {'location': 'Dhaka', 'hometown': 'Gazipur'}
    

# Q62. What is the use of get() function?

The get() method reurns the value of the item with specified key



```python
car = {"brand": "Ford", "model": "Mustang", "year": 1964}
print(car)

# dictionary.get(keyname)
x = car.get("model")
print(x)

# dictinary.get(keyname, value) #Optional. A value to return if the specified key does not exist.
x = car.get("price", 15000)
print(x)
```

    {'brand': 'Ford', 'model': 'Mustang', 'year': 1964}
    Mustang
    15000
    

# ###Coding Problem###

# Q76. Write a Python program to find the factorial of a given number.




```python
def fact_func(n):
    if n == 0 or n == 1:
        return 1
    factorial = 1
    for i in range(1, n+1):
        factorial *= i
    return factorial

number = int(input("Enter a number : "))
result = fact_func(number)
print(number, "! =", result)
```

    Enter a number : 0
    0 ! = 1
    

# Q77. Write a Python program to calculate the simple interest. Formula to calculate simple interest is SI = (PRT)/100




```python
P = 80000
R = 8
T = 3
SI = (P*R*T)/100

print('The Simple Interest is :', SI)

```

    The Simple Interest is : 19200.0
    

# Q78. Write a Python program to calculate the compound interest. Formula of compound interest is A = P(1+ R/100)^t.




```python
P = 10000
T = 5
R = 10.25
A = P*(1+R/100)**T
CI = A - P
print("Compound Interest =", CI)
print("Compound Interest =", round(CI,2))
```

    Compound Interest = 6288.946267774416
    Compound Interest = 6288.95
    

# Q79. Write a Python program to check if a number is prime or not.




```python
# simple method-not efficient
num = int(input("Enter a number :"))
for i in range(2, num):
    if num % i == 0:
        print("Not Prime")
        break
else:
    print("Prime")
```

    Enter a number :11
    Prime
    

# Q80. Write a Python program to check Armstrong Number.




```python

```
