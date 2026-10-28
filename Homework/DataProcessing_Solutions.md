# FCSS Data Processing Homework: Tutor Solutions

## Task 1
```python
numbers = [3, 7, 10, 15]

for number in numbers:
    print(number)

for number in numbers:
    print(number * 2)
```

## Task 2
```python
for number in numbers:
    if number >= 10:
        print(number)
```

## Task 3
```python
students = [
    {"name": "Ana", "score": 72},
    {"name": "Ben", "score": 45},
    {"name": "Cara", "score": 88},
    {"name": "David", "score": 50}
]

for student in students:
    print(student["name"], student["score"])
```

## Task 4
```python
for student in students:
    if student["score"] >= 50:
        print(student["name"])
```

## Task 5
```python
def passed(score):
    return score >= 50
```

## Task 6
```python
for student in students:
    if passed(student["score"]):
        print(student["name"], "Pass")
    else:
        print(student["name"], "Not passed")
```

## Task 7
```python
passed_students = []

for student in students:
    if passed(student["score"]):
        passed_students.append(student["name"])

print(passed_students)
```

## Task 8
```python
posts = [
    {"id": "P01", "text": "Python is useful", "likes": 7},
    {"id": "P02", "text": "Learning Python takes regular practice", "likes": 18},
    {"id": "P03", "text": "Loops save repeated work", "likes": 12}
]

def count_words(text):
    return len(text.split())

for post in posts:
    if post["likes"] >= 10 and count_words(post["text"]) >= 4:
        print(post["id"])
```

## Task 9

A: add `:` after `numbers`.

B: indent the loop body.

C: use the existing key `"score"` instead of `"scores"`.

D: add `return number * 2`.
