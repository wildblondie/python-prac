# DataAnnotation Python Assessment Practice Quiz
## 100 Multiple Choice Questions with Answers

---

## SECTION 1: Pythonic Thinking (Questions 1-20)

**1.** What is the "Pythonic" way to check if a list is empty?
- A) `if len(my_list) == 0:`
- B) `if my_list == []:`
- C) `if not my_list:`
- D) `if my_list.isEmpty():`

**Answer: C** — `if not my_list:` is idiomatic Python; empty containers are falsy.

---

**2.** Which is the most Pythonic way to iterate over indices and values of a list?
- A) `for i in range(len(lst)): print(i, lst[i])`
- B) `for i, val in enumerate(lst): print(i, val)`
- C) `i = 0; while i < len(lst): print(i, lst[i]); i += 1`
- D) `for val in lst: print(lst.index(val), val)`

**Answer: B** — `enumerate()` is the Pythonic idiom.

---

**3.** What does PEP 8 recommend for indentation?
- A) Tabs only
- B) 2 spaces
- C) 4 spaces
- D) 8 spaces

**Answer: C**

---

**4.** What is the output of `bool([])`?
- A) True
- B) False
- C) None
- D) Error

**Answer: B**

---

**5.** Which is the Pythonic way to swap two variables?
- A) `temp = a; a = b; b = temp`
- B) `a, b = b, a`
- C) `a = b; b = a`
- D) `swap(a, b)`

**Answer: B**

---

**6.** What does the walrus operator `:=` do?
- A) Compares two values
- B) Assigns a value as part of an expression
- C) Creates a lambda
- D) Unpacks a tuple

**Answer: B** — Introduced in Python 3.8 for assignment expressions.

---

**7.** Which is more Pythonic for combining two lists into pairs?
- A) A manual for-loop with indices
- B) `zip(list1, list2)`
- C) `list1 + list2`
- D) `list1.extend(list2)`

**Answer: B**

---

**8.** What is a "Pythonic" way to check membership in a collection?
- A) `for x in collection: if x == item: return True`
- B) `item in collection`
- C) `collection.contains(item)`
- D) `collection.find(item) != -1`

**Answer: B**

---

**9.** What does EAFP stand for in Python philosophy?
- A) Easier As First Priority
- B) Easier to Ask Forgiveness than Permission
- C) Every Argument Fulfills Purpose
- D) Explicit Always For Programmers

**Answer: B** — Prefer try/except over pre-checking (LBYL).

---

**10.** Which of these is a "Pythonic" way to build a list of squares from 0-9?
- A) A for-loop with `.append()`
- B) `[x**2 for x in range(10)]`
- C) A while-loop
- D) `map()` without converting to list

**Answer: B** — List comprehensions are preferred.

---

**11.** What is the output of `list(filter(lambda x: x % 2 == 0, [1,2,3,4,5,6]))`?
- A) `[1, 3, 5]`
- B) `[2, 4, 6]`
- C) `[1, 2, 3, 4, 5, 6]`
- D) Error

**Answer: B**

---

**12.** According to "The Zen of Python," which is true?
- A) Complex is better than complicated
- B) Simple is better than complex
- C) Implicit is better than explicit
- D) Sparse is worse than dense

**Answer: B**

---

**13.** What's the idiomatic way to open and safely close a file?
- A) `f = open('file.txt'); f.read(); f.close()`
- B) `with open('file.txt') as f: f.read()`
- C) `open('file.txt').read()`
- D) `try: f = open('file.txt') finally: f.close()`

**Answer: B** — Context managers ensure proper cleanup.

---

**14.** What does `if __name__ == "__main__":` do?
- A) Checks if a variable named "main" exists
- B) Ensures code only runs when the script is executed directly
- C) Defines the main function
- D) Imports the main module

**Answer: B**

---

**15.** Which is more Pythonic for string formatting (Python 3.6+)?
- A) `"Hello, " + name + "!"`
- B) `"Hello, %s!" % name`
- C) `f"Hello, {name}!"`
- D) `"Hello, {0}!".format(name)`

**Answer: C** — f-strings are the modern, preferred approach.

---

**16.** What is a "duck typing" example in Python?
- A) Checking `type(obj) == list`
- B) Using `isinstance(obj, list)`
- C) Calling `obj.append()` without checking its type, relying on it having that method
- D) Using type hints exclusively

**Answer: C** — "If it walks like a duck and quacks like a duck..."

---

**17.** What does `*args` allow a function to do?
- A) Accept keyword arguments only
- B) Accept a variable number of positional arguments
- C) Return multiple values
- D) Define default parameters

**Answer: B**

---

**18.** What is the output of `any([0, '', None, False])`?
- A) True
- B) False
- C) None
- D) Error

**Answer: B** — All values are falsy.

---

**19.** Which of the following is generally considered non-Pythonic?
- A) Using list comprehensions for simple transformations
- B) Using `type(x) == int` instead of `isinstance(x, int)`
- C) Using context managers for file handling
- D) Using `enumerate()` in loops

**Answer: B** — `isinstance()` is preferred (supports inheritance, more flexible).

---

**20.** What does the `**kwargs` parameter allow?
- A) Passing a variable number of keyword arguments as a dictionary
- B) Passing a variable number of positional arguments
- C) Raising an exception with keyword info
- D) Unpacking a list

**Answer: A**

---

## SECTION 2: Strings & Slicing (Questions 21-40)

**21.** What is the output of `"hello"[1:4]`?
- A) `"hell"`
- B) `"ell"`
- C) `"ello"`
- D) `"hel"`

**Answer: B**

---

**22.** What does `"hello"[::-1]` return?
- A) `"hello"`
- B) `"olleh"`
- C) `""`
- D) Error

**Answer: B** — Reverses the string.

---

**23.** What is the output of `"Python"[-3:]`?
- A) `"Pyt"`
- B) `"tho"`
- C) `"hon"`
- D) `"thon"`

**Answer: C**

---

**24.** What does `"  hello  ".strip()` return?
- A) `"  hello  "`
- B) `"hello"`
- C) `"hello  "`
- D) `"  hello"`

**Answer: B**

---

**25.** What is the result of `"abc" * 3`?
- A) `"abc3"`
- B) `"abcabcabc"`
- C) Error
- D) `9`

**Answer: B**

---

**26.** What does `"Hello World".split()` return?
- A) `"HelloWorld"`
- B) `['Hello', 'World']`
- C) `('Hello', 'World')`
- D) `"Hello", "World"`

**Answer: B**

---

**27.** What is the output of `"-".join(['a', 'b', 'c'])`?
- A) `"a-b-c"`
- B) `"abc"`
- C) `['a-b-c']`
- D) `"a-b-c-"`

**Answer: A**

---

**28.** What does `"Hello".lower()` return?
- A) `"HELLO"`
- B) `"hello"`
- C) `"Hello"`
- D) Error (strings are immutable)

**Answer: B**

---

**29.** What is `len("hello")`?
- A) 4
- B) 5
- C) 6
- D) Error

**Answer: B**

---

**30.** What does `"hello".replace("l", "L")` return?
- A) `"heLLo"`
- B) `"heLo"`
- C) `"hello"`
- D) `"HeLLo"`

**Answer: A**

---

**31.** What is the output of `"hello"[10]`?
- A) `""`
- B) `None`
- C) IndexError
- D) `"o"`

**Answer: C** — Index out of range.

---

**32.** What does `"3" + "4"` evaluate to?
- A) `7`
- B) `"34"`
- C) `"7"`
- D) TypeError

**Answer: B** — String concatenation, not addition.

---

**33.** What is `"hello"[2:2]`?
- A) `"l"`
- B) `""`
- C) `"ll"`
- D) Error

**Answer: B** — Empty slice when start == stop.

---

**34.** What does `str.isdigit()` check?
- A) If the string contains any digit
- B) If all characters in the string are digits
- C) If the string is a valid float
- D) If the string is numeric or alphabetic

**Answer: B**

---

**35.** What is the output of `"Hello"[::2]`?
- A) `"Hlo"`
- B) `"Hel"`
- C) `"elo"`
- D) `"Hello"`

**Answer: A** — Every second character starting from index 0.

---

**36.** What does `"  ".isspace()` return?
- A) False
- B) True
- C) None
- D) Error

**Answer: B**

---

**37.** What is the result of `f"{3.14159:.2f}"`?
- A) `"3.14"`
- B) `"3.14159"`
- C) `"3.1"`
- D) Error

**Answer: A** — Formats to 2 decimal places.

---

**38.** What does `"Hello, World!".find("World")` return?
- A) `True`
- B) `7`
- C) `-1`
- D) `"World"`

**Answer: B** — Returns starting index.

---

**39.** What is `"abcdef"[1:5:2]`?
- A) `"bd"`
- B) `"bcde"`
- C) `"ace"`
- D) `"bce"`

**Answer: A** — Start=1, stop=5, step=2: indices 1,3.

---

**40.** What does `"Hello".startswith("he")` return (case-sensitive)?
- A) True
- B) False
- C) None
- D) Error

**Answer: B** — Case-sensitive; "He" ≠ "he".

---

## SECTION 3: Loops & Iterators (Questions 41-60)

**41.** What does `range(5)` generate?
- A) `[1, 2, 3, 4, 5]`
- B) `[0, 1, 2, 3, 4]`
- C) `[0, 1, 2, 3, 4, 5]`
- D) `[1, 2, 3, 4]`

**Answer: B**

---

**42.** What is the output of the following?
```python
for i in range(3):
    print(i, end=' ')
```
- A) `0 1 2`
- B) `1 2 3`
- C) `0 1 2 3`
- D) `1 2`

**Answer: A**

---

**43.** What does the `break` statement do in a loop?
- A) Skips the current iteration
- B) Exits the loop entirely
- C) Restarts the loop
- D) Pauses the loop

**Answer: B**

---

**44.** What does the `continue` statement do?
- A) Exits the loop
- B) Skips the rest of the current iteration and moves to the next
- C) Restarts the entire program
- D) Does nothing

**Answer: B**

---

**45.** What is the output of:
```python
for i in range(5):
    if i == 3:
        break
    print(i, end=' ')
```
- A) `0 1 2 3 4`
- B) `0 1 2`
- C) `0 1 2 3`
- D) `3`

**Answer: B**

---

**46.** What does `else` after a `for` loop execute?
- A) Always after the loop
- B) Only if the loop completes without `break`
- C) Only if the loop is empty
- D) Never

**Answer: B**

---

**47.** What is the output of:
```python
for i in range(3):
    pass
else:
    print("Done")
```
- A) Nothing
- B) `Done`
- C) Error
- D) `0 1 2 Done`

**Answer: B**

---

**48.** What does `iter()` do to a list?
- A) Sorts the list
- B) Returns an iterator object
- C) Reverses the list
- D) Converts it to a tuple

**Answer: B**

---

**49.** What does `next()` do to an iterator?
- A) Skips the next element
- B) Returns the next item from the iterator
- C) Restarts the iterator
- D) Converts iterator to list

**Answer: B**

---

**50.** What happens when `next()` is called on an exhausted iterator?
- A) Returns `None`
- B) Raises `StopIteration`
- C) Returns `0`
- D) Loops back to start

**Answer: B**

---

**51.** What is the output of `list(range(1, 10, 2))`?
- A) `[1, 3, 5, 7, 9]`
- B) `[1, 2, 3, 4, 5, 6, 7, 8, 9]`
- C) `[2, 4, 6, 8]`
- D) `[1, 3, 5, 7]`

**Answer: A**

---

**52.** What does a generator function use instead of `return`?
- A) `stop`
- B) `yield`
- C) `end`
- D) `output`

**Answer: B**

---

**53.** What is the output of:
```python
i = 0
while i < 3:
    print(i, end=' ')
    i += 1
```
- A) `0 1 2`
- B) `0 1 2 3`
- C) `1 2 3`
- D) Infinite loop

**Answer: A**

---

**54.** Which loop type is best suited for iterating a known number of times over a sequence?
- A) `while` loop
- B) `for` loop
- C) Recursive function
- D) `do-while` loop (doesn't exist in Python)

**Answer: B**

---

**55.** What does `list(zip([1,2,3], ['a','b','c']))` produce?
- A) `[(1, 'a'), (2, 'b'), (3, 'c')]`
- B) `[1, 2, 3, 'a', 'b', 'c']`
- C) `{1: 'a', 2: 'b', 3: 'c'}`
- D) Error

**Answer: A**

---

**56.** What is a generator expression?
- A) `[x for x in range(5)]`
- B) `(x for x in range(5))`
- C) `{x for x in range(5)}`
- D) `{x: x for x in range(5)}`

**Answer: B** — Parentheses create a generator.

---

**57.** What is the output of:
```python
for i in range(2):
    for j in range(2):
        print(i, j)
```
- A) `0 0` `0 1` `1 0` `1 1`
- B) `0 1 0 1`
- C) `0 0 1 1`
- D) Error

**Answer: A**

---

**58.** What does `reversed([1, 2, 3])` return?
- A) A list `[3, 2, 1]`
- B) A reverse iterator object
- C) `None`
- D) Error

**Answer: B** — Must be converted with `list()` to see values.

---

**59.** How would you iterate over a dictionary's key-value pairs?
- A) `for k, v in my_dict:`
- B) `for k, v in my_dict.items():`
- C) `for k, v in my_dict.pairs():`
- D) `for (k,v) in my_dict.list():`

**Answer: B**

---

**60.** What is the output of:
```python
x = [1, 2, 3]
it = iter(x)
print(next(it))
print(next(it))
```
- A) `1 2`
- B) `1` then `2` (on separate lines)
- C) `[1, 2, 3]`
- D) Error

**Answer: B**

---

## SECTION 4: Dictionaries (Questions 61-80)

**61.** How do you create an empty dictionary?
- A) `dict = []`
- B) `dict = {}`
- C) `dict = ()`
- D) `dict = set()`

**Answer: B**

---

**62.** What does `my_dict.get("key", "default")` do?
- A) Raises an error if "key" doesn't exist
- B) Returns the value for "key", or "default" if not found
- C) Adds "key" with value "default"
- D) Deletes "key"

**Answer: B**

---

**63.** What happens if you access a non-existent key directly, e.g., `my_dict["missing"]`?
- A) Returns `None`
- B) Returns an empty string
- C) Raises `KeyError`
- D) Returns `0`

**Answer: C**

---

**64.** What does `my_dict.keys()` return?
- A) A list of keys
- B) A view object of keys
- C) A tuple of keys
- D) A set of keys

**Answer: B** — In Python 3, it's a dict_keys view object.

---

**65.** How do you merge two dictionaries in Python 3.9+?
- A) `dict1 + dict2`
- B) `dict1 | dict2`
- C) `dict1.merge(dict2)`
- D) `dict1 & dict2`

**Answer: B** — The `|` operator merges dicts (3.9+).

---

**66.** What does `my_dict.pop("key")` do?
- A) Returns the value and removes the key
- B) Only removes the key without returning
- C) Adds a new key
- D) Raises an error always

**Answer: A**

---

**67.** What is the output of:
```python
d = {"a": 1, "b": 2}
d["c"] = 3
print(d)
```
- A) `{"a": 1, "b": 2}`
- B) `{"a": 1, "b": 2, "c": 3}`
- C) Error
- D) `{"c": 3}`

**Answer: B**

---

**68.** What does `dict.fromkeys(['a', 'b'], 0)` produce?
- A) `{'a': 0, 'b': 0}`
- B) `['a', 'b']`
- C) `{0: ['a', 'b']}`
- D) Error

**Answer: A**

---

**69.** Are dictionary keys required to be unique?
- A) No, duplicates are fine
- B) Yes, duplicate keys overwrite previous values
- C) Only strings must be unique
- D) Yes, and duplicates raise an error

**Answer: B**

---

**70.** What is a dictionary comprehension?
- A) `{k: v for k, v in items}`
- B) `[k: v for k, v in items]`
- C) `(k: v for k, v in items)`
- D) `dict(k, v for items)`

**Answer: A**

---

**71.** What data types can be dictionary keys?
- A) Any mutable type
- B) Any hashable (immutable) type
- C) Only strings
- D) Only integers

**Answer: B** — Keys must be hashable, e.g., strings, numbers, tuples.

---

**72.** What does `len(my_dict)` return?
- A) Number of keys
- B) Number of values
- C) Number of key-value pairs (same as keys)
- D) Total characters in the dict

**Answer: C** — A and C are effectively the same in this context.

---

**73.** What is the output of:
```python
d = {"x": 10, "y": 20}
for k in d:
    print(k)
```
- A) `10 20`
- B) `x y` (on separate lines)
- C) `x: 10, y: 20`
- D) Error

**Answer: B** — Iterating a dict by default gives keys.

---

**74.** What does `my_dict.setdefault("key", "value")` do?
- A) Always overwrites "key" with "value"
- B) Returns existing value if key exists; otherwise sets and returns "value"
- C) Deletes the key
- D) Raises error if key exists

**Answer: B**

---

**75.** What is the output of:
```python
d = {"a": [1, 2], "b": [3, 4]}
print(d["a"][1])
```
- A) `1`
- B) `2`
- C) `[1, 2]`
- D) Error

**Answer: B**

---

**76.** How can you check if a key exists in a dictionary?
- A) `"key" in my_dict`
- B) `my_dict.contains("key")`
- C) `my_dict.hasKey("key")`
- D) `key.in(my_dict)`

**Answer: A**

---

**77.** What does `my_dict.values()` return?
- A) A list of values
- B) A view object of values
- C) A dictionary of values
- D) A set of values

**Answer: B**

---

**78.** What is the output of:
```python
d = {}
d["a"] = d.get("a", 0) + 1
print(d)
```
- A) `{"a": 1}`
- B) `{"a": 0}`
- C) Error
- D) `{}`

**Answer: A** — Common pattern for counting.

---

**79.** How do you delete a key-value pair from a dictionary?
- A) `del my_dict["key"]`
- B) `my_dict.remove("key")`
- C) `my_dict - "key"`
- D) `my_dict.delete("key")`

**Answer: A**

---

**80.** What is the output of:
```python
d1 = {"a": 1}
d2 = {"a": 2, "b": 3}
d1.update(d2)
print(d1)
```
- A) `{"a": 1, "b": 3}`
- B) `{"a": 2, "b": 3}`
- C) `{"a": 1}`
- D) Error

**Answer: B** — `update()` overwrites existing keys.

---

## SECTION 5: Functions (Questions 81-100)

**81.** What keyword defines a function in Python?
- A) `function`
- B) `def`
- C) `func`
- D) `define`

**Answer: B**

---

**82.** What does a function return if there's no explicit `return` statement?
- A) `0`
- B) `""`
- C) `None`
- D) An error

**Answer: C**

---

**83.** What is the output of:
```python
def add(a, b=5):
    return a + b
print(add(3))
```
- A) `3`
- B) `5`
- C) `8`
- D) Error

**Answer: C** — Uses default value `b=5`.

---

**84.** What does `*args` collect in a function definition?
- A) A dictionary of arguments
- B) A tuple of positional arguments
- C) A list of keyword arguments
- D) A single argument

**Answer: B**

---

**85.** What does `**kwargs` collect in a function definition?
- A) A tuple of arguments
- B) A dictionary of keyword arguments
- C) A list of arguments
- D) Nothing

**Answer: B**

---

**86.** What is a lambda function?
- A) A multi-line function with a name
- B) An anonymous, single-expression function
- C) A function that only returns None
- D) A built-in Python method

**Answer: B**

---

**87.** What is the output of:
```python
square = lambda x: x ** 2
print(square(4))
```
- A) `8`
- B) `16`
- C) `4`
- D) Error

**Answer: B**

---

**88.** What is a "closure" in Python?
- A) A function that closes files
- B) A nested function that captures variables from its enclosing scope
- C) A syntax error
- D) A type of loop

**Answer: B**

---

**89.** What does the `global` keyword do inside a function?
- A) Creates a new global variable that shadows local ones
- B) Allows modification of a global variable within the function
- C) Deletes a global variable
- D) Has no effect

**Answer: B**

---

**90.** What is the output of:
```python
def foo():
    return
result = foo()
print(result)
```
- A) Error
- B) `None`
- C) Empty string
- D) `0`

**Answer: B**

---

**91.** What is a "docstring"?
- A) A comment starting with `#`
- B) A string literal used to document a function/class/module (usually triple-quoted)
- C) A special type of variable
- D) An error message

**Answer: B**

---

**92.** What does the `return` statement do when it executes?
- A) Continues the loop
- B) Immediately exits the function and returns a value
- C) Prints the value
- D) Pauses execution

**Answer: B**

---

**93.** What is the output of:
```python
def multi_return():
    return 1, 2, 3
a, b, c = multi_return()
print(b)
```
- A) `1`
- B) `2`
- C) `3`
- D) Error

**Answer: B** — Function returns a tuple, unpacked into a, b, c.

---

**94.** What is a decorator in Python?
- A) A comment style
- B) A function that modifies another function's behavior
- C) A type of loop
- D) A built-in data type

**Answer: B**

---

**95.** What is the correct syntax for using a decorator?
- A) `@decorator_name` above the function definition
- B) `#decorator_name` above the function
- C) `decorator_name()` inside the function
- D) `use decorator_name`

**Answer: A**

---

**96.** What does `functools.reduce()` do?
- A) Sorts a list
- B) Applies a function cumulatively to items in an iterable, reducing to a single value
- C) Filters items from a list
- D) Reduces a string's length

**Answer: B**

---

**97.** What is the output of:
```python
def outer():
    x = 10
    def inner():
        nonlocal x
        x += 5
        return x
    return inner()
print(outer())
```
- A) `10`
- B) `15`
- C) `5`
- D) Error

**Answer: B** — `nonlocal` modifies the enclosing variable.

---

**98.** What happens if you call a function with too few required positional arguments?
- A) It uses `None` for missing arguments
- B) `TypeError` is raised
- C) It runs with default 0 values
- D) `SyntaxError`

**Answer: B**

---

**99.** What is the output of:
```python
def modify_list(lst):
    lst.append(4)
my_list = [1, 2, 3]
modify_list(my_list)
print(my_list)
```
- A) `[1, 2, 3]`
- B) `[1, 2, 3, 4]`
- C) Error
- D) `[4]`

**Answer: B** — Lists are mutable; passed by reference.

---

**100.** What is the correct way to define a function with type hints?
- A) `def add(a: int, b: int) -> int:`
- B) `def add(a, b): int`
- C) `def add(a as int, b as int): int`
- D) `def add<int, int>(a, b):`

**Answer: A**

---

## 📊 Scoring Guide
- **90-100 correct:** Excellent! You're well-prepared.
- **75-89 correct:** Good grasp; review missed topics.
- **60-74 correct:** Moderate; focus on weak areas before the assessment.
- **Below 60:** Recommend deeper review of Python fundamentals.

## 💡 Key Topics to Review by Section
| Section | Core Concepts to Master |
|---|---|
| Pythonic Thinking | List comprehensions, EAFP, `enumerate`, f-strings, `isinstance` |
| Strings & Slicing | Slice notation `[start:stop:step]`, string methods, immutability |
| Loops & Iterators | `for`/`while`, `break`/`continue`, generators, `iter()`/`next()` |
| Dictionaries | `.get()`, `.items()`, comprehensions, merging, `KeyError` handling |
| Functions | `*args`/`**kwargs`, closures, decorators, mutable default pitfalls |

Good luck on your DataAnnotation assessment! 🐍