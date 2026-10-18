# FCSS Homework: Data Processing with Python

## Task 1: Basic loop

```python
numbers = [3, 7, 10, 15]
```

Use a `for` loop to print every number.

Then print each number multiplied by `2`.

## Task 2: Loop + condition

Print only numbers that are at least `10`.

Expected:

```text
10
15
```

## Task 3: Process dictionaries

```python
students = [
    {"name": "Ana", "score": 72},
    {"name": "Ben", "score": 45},
    {"name": "Cara", "score": 88},
    {"name": "David", "score": 50}
]
```

Print the name and score of every student.

## Task 4: Loop + dictionary + condition

Print only the names of students whose score is at least `50`.

Expected:

```text
Ana
Cara
David
```

## Task 5: Write a function

Create:

```python
def passed(score):
    ...
```

Return `True` if the score is at least `50`, otherwise `False`.

Test with `49`, `50`, and `80`.

## Task 6: Use the function in a loop

Print:

```text
Ana Pass
Ben Not passed
Cara Pass
David Pass
```

## Task 7: Store results

Create:

```python
passed_students = []
```

Append the name of every student who passed.

Expected:

```python
['Ana', 'Cara', 'David']
```

## Task 8: Combined challenge

```python
posts = [
    {"id": "P01", "text": "Python is useful", "likes": 7},
    {"id": "P02", "text": "Learning Python takes regular practice", "likes": 18},
    {"id": "P03", "text": "Loops save repeated work", "likes": 12}
]
```

Create `count_words(text)`.

Then print the ID of every post that:
- has at least `10` likes,
- contains at least `4` words.

Expected:

```text
P02
P03
```

## Task 9: Fix the errors

### A
```python
for number in numbers
    print(number)
```

### B
```python
for number in numbers:
print(number)
```

### C
```python
student = {"name": "Ana", "score": 72}
print(student["scores"])
```

### D
```python
def double(number):
    number * 2

print(double(5))
```

For each:
1. fix the code,
2. explain the problem in one sentence.

## Optional extension

Create your own list of dictionaries and:
1. loop through it,
2. filter with an `if`,
3. store matching results in a list.

