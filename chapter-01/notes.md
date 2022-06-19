<div id="Top" />

### Expressions
- They are the fundamental form of instruction in Python. 
- Valid expressions are always evaluated by python to a single value which can be any type from *strings*, to *objects*.
- They are composed of a myriad of combinations of values, i.e. 42, 21, 2022, and operations, i.e. addition ( + ), and multiplication ( * ).

<p style="font-size: 14px; margin: 0; font-weight: bold;">Table 1.1 Math Operations According to Precedence</p>

| Operator | Operation        | Example  | Result |
|----------|------------------|----------|--------|
| **       | Exponent         | 8 ** 2   | 16     |
| %        | Modulus          | 10 % 3   | 1      |
| //       | Floored Division | 21 // 10 | 2      |
| /        | Division         | 12 / 3   | 4      |
| *        | Multiplication   | 9 * 9    | 81     |
| -        | Subtraction      | 100 - 100| 0      |
| +        | Addition         | 40 + 2   | 42     |
 
- Basically, the order in which python evaluates expressions that incorporate different combinations of mathematical operations is aligned to that of mathematics. It follows that one can manipulate this order of evaluating operations using a parenthesis `()` like in mathematics.
- Some operators can behave differently based on the types of values it is operating.
	- The `+` symbol can act as the *addition operator* to evaluate the result of adding two integers, two floats, or a combination of the two to produce the sum.
	```python
	>>> 4 + 3
	7
	```
	- The `+` symbol can also act as the *string concatenation operator* where it adds two strings together to produce a longer combination of the strings being operated.
	```python
	>>> "Loid " + "Forger"
	"Loid Forger"
	```
	- However, adding a string and an integer together will produce an error.
	```python
	>>> 40 + "2"
	Traceback (most recent call last):
		File "<stdin>", line 1, in <module>
	TypeError: can only concatenate str (not "int") to str
	```
	- The `*` operator can act as the *multiplication operator* to evaluate the result of multiplying two integers, two floats, or a combination of the two to produce the quotient.
	```python
	>>> 10 * 10
	100
	```
	- The `*` operator can also act as the *string replication operator* which will evaluate into a single string value that is the original string repeated a number of times equal to the integer.
	```python
	>>> "Daifuku" * 3
	"DaifukuDaifukuDaifuku"
	``` 
	- However, multiplying a string and a float will produce an error. This is expected because there are various nuances attributed to the idea of obtaining a replication of a string a fractional number of times. Think about how would you define `"Hello" * pi`?
	```python
	>>> "Daifuku" * 3.0
	Traceback (most recent call last):
	  File "<stdin>", line 1, in <module>
	TypeError: can't multiply sequence by non-int of type 'float'
	```
	- An error will also be produced when multiplying two strings together. This is expected because it doesn't make sense to replicate a string by a string number of times.
- This is due to the fact that Python does not convert either the string or the integer into any other value explicitly. One has to convert either `"40"` into an integer or `2` into a string in order for the `+` symbol to act as either the addition operator or the string concatenation operator.
```python
>>> 2 + 2
4

>>> "2" + "2"
"22"

>>> "I" + " love" + " peanuts."
"I love peanuts."
```
-  Whitespaces between integers and operations alike are insignificant, but the initial indentation in any line of code is significant.
```python
>>> 40 + 2
42

>>>40      +      2
42
>>>             40 + 2

File "<stdin>", line 1
	40 + 2
    ^
IndentationError: unexpected indent
```

### Data Types

- Every value in Python belongs to exactly one built-in data type.
- Common python data types:
  
| Data type | Examples                |
| --------- | ----------------------- |
| Integers  | -1, 0, 1                |
| Floats    | -1.0, 0.0, 1.0          |
| Strings   | "Hello, World!", "2022" | 
- Python has other built-in data types such as `lists`, `tuple`, `dict`, `set`, `bool`, `functions` and `NoneType` among others.

#### Variables
- A variable is a container inside a computer's memory that is associated with a symbolic name or an identifier.
- It can store any single value. So a variable can either contain a `string`, `int`, `tuple`, `dict`, and `NoneType` among others.
- A variable is initialized the moment a value has been stored in it. One can store values into a variable using an assignment statement which consists of an `identifier`, the `=` symbol, and the value to be stored. In the example below, we have an identifier, `anime` followed by the `=` symbol which instructs Python to store the string of `"Magic Kaito 1412"` into the variable.
```python
>>> anime = "Magic Kaito 1412"
'Magic Kaito 1412'
```
- The values stored inside variables can be overwritten by a more recent assignment to that variable.
```python
>>> anime = "Magic Kaito 1412"
>>> anime
'Magic Kaito 1412'

>>> anime = "Detective Conan"
>>> anime
'Detective Conan'
```
- The number of identifiers there can be is limitless. Any programmer can name their variables anything they want or have their own naming conventions for a specific project. However, there are restrictions that Python has implemented which dictate whether a potential identifier for a variable is valid or invalid.
	- The identifier cannot contain a space. It must be continuous.
	- The identifier can only contain valid letters, numbers, and the underscore `_` character.
	- The identifier cannot begin with a number.



[⬆️ Top](#Top)





