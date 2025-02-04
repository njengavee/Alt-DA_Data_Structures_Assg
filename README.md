# DO NOT CREATE OR DELETE ANY CELLS
## DO NOT CREATE OR DELETE ANY CELLS
### DO NOT CREATE OR DELETE ANY CELLS
#### DO NOT CREATE OR DELETE ANY CELLS
# Objects and Data Structures Assessment Test
- I Strongly advise you take the questions and practice on a different notebook and then when you are certain you have to correct code bring it in here and paste in the approriate cell.
- To answer the questions first delete this line `raise NotImplementedError()` and then write your code after the `#your code here comment`
## 1. Strings
- Create a variable s and put the string hello world in it, then extract every second letter and store it in a variable called letter_sequence.
- Create a formatted string using format and {} and store it in variable called greeting such that If "Jadesola" is inserted as the name and "25" as the age, the result should be Hello Jadesola, you are 25 years old.
```python
# YOUR CODE HERE
# creating a variable
s = "hello world"
print(s)

# Extracting every second letter
letter_sequence = s[::2]
print(letter_sequence)

# string formatting with .format() method
greeting = "Hello {}, you are {} years old"
greeting.format('Jadesola', 25)
```
```python
#do not modify this cell
#do not modify this cell
#do not modify this cell
#do not modify this cell
assert letter_sequence == "hlowrd"
assert greeting.format("Jackson", 25) == "Hello Jackson, you are 25 years old"
```
## 2. Lists
With a list defined like this list3 = [1, 2, [3, 4, 'hello']] modify it by:
- Changing "hello" to "goodbye".
- Append 100 to the list.
- Removing 2 from the list.
- Reverse the entire list.
- Store the final result in a variable called modiFied


```python
list3 = [1, 2, [3, 4, 'hello']]
# YOUR CODE HERE
# changing "hello" to "goodbye"
list3[2][2] = "goodbye"
print(list3)

# appending 100 to the list
list3.append(100)
print(list3)

# removing 2 from the list
list3.remove(2)
print(list3)

# reverse the entire list and store in variable modiFied
modiFied = list3[::-1]
print(modiFied)
```

```python
#do not modify this cell
#do not modify this cell
#do not modify this cell
#do not modify this cell
assert modiFied == [
    10 ** 2,
    [9/3, 16**0.5, "good" + "bye"],
    2 - 1
]
```

## 3. Dictionaries
Given the dictionary: d = {"k1": [{"nest_key": ["this is deep", ["hello"]]}], "age": 30}

- Extract "hello" and store it in dict_answer.
- Add a new key name with the value Alice.
- Increase age by 5.

```python
d = {"k1": [{"nest_key": ["this is deep", ["hello"]]}], "age": 30}
# YOUR CODE HERE
# Extract "hello" from dict
dict_answer = d["k1"][0]["nest_key"][1][0]
print(dict_answer)

# Add a new key "name" with the value "Alice"
d["name"] = "Alice"
print(d)

# Increase age by 5
d["age"] += 5
print(d)
```

```python
#do not modify this cell
#do not modify this cell
#do not modify this cell
#do not modify this cell
assert dict_answer == "hello"
assert d["name"] == "Alice"
assert d["age"] == 35
```

## 4. Tuples
- Create a tuple my_tuple with values (5, 15, 3).
- Unpack it into three variables: a, b, c.
- Concatenate my_tuple with (4, 5, 6) and store it in new_tuple.

```python
# YOUR CODE HERE
# create a tuple
my_tuple = (5, 15, 3)
print(my_tuple)

# Unpack it into three variables: a, b, c.
a, b, c = my_tuple
print(a, b, c)

# Concatenate my_tuple with (4, 5, 6)
new_tuple = my_tuple + (4, 5, 6)
print(new_tuple)
```

```python
#do not modify this cell
#do not modify this cell
#do not modify this cell
#do not modify this cell
assert a == 15/3 and b == 7+8 and c == 9**0.5
```

## 5. Sets
Use a set to find the unique values of the list below and assign it to a variable unique_values:

```python
list5 = [1,2,2,33,4,4,11,22,3,3,2]
# YOUR CODE HERE
# finding unique values from list5
unique_values = set(list5)
print(unique_values)
```

```python
#do not modify this cell
#do not modify this cell
#do not modify this cell
#do not modify this cell
assert unique_values ==  {1, 2, 3, 4, 11, 22, 33}
```

# Great Job on your first assessment!
