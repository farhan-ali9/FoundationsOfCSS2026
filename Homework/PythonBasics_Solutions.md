# FCSS Python Basics Homework: Tutor Solutions

## Task 1
```python
name = "Cynthia"
study_hours = 3
print(f"{name} studied Python for {study_hours} hours.")
```

## Task 2
```python
score1 = 62
score2 = 75
score3 = 83
average = (score1 + score2 + score3) / 3
print(average)
```

## Task 3
```python
scores = [62, 75, 83, 49]

print(scores[0])
print(scores[-1])

scores.append(91)

print(len(scores))
print(sum(scores) / len(scores))
```

## Task 4
```python
post = {
    "id": "P01",
    "text": "Python practice takes time",
    "likes": 8
}

print(post["text"])
post["likes"] = 12
post["platform"] = "Forum"
print(post)
```

## Task 5
```python
likes = 12

print(likes >= 10)  # True
print(likes == 12)  # True
print(likes < 5)    # False
```

## Task 6
```python
score = 49

if score >= 50:
    print("Pass")
else:
    print("Not yet passed")
```

Test again with 50 and 80.

## Task 7
```python
student = {
    "name": "Alex",
    "scores": [55, 70, 40]
}

average = sum(student["scores"]) / len(student["scores"])
print(f'{student["name"]}: {average:.2f}')

if average >= 50:
    print("Pass")
else:
    print("Not yet passed")
```

## Task 8

### A
```python
name = "Cynthia"
print(name)
```
Text needs quotation marks.

### B
```python
score = 60
if score >= 50:
    print("Pass")
```
The `if` line needs a colon.

### C
```python
age = 22
print(f"Age: {age}")
```
A string and an integer cannot be joined directly with `+` without conversion.

### D
```python
scores = [50, 60, 70]
print(scores[2])
```
The valid indices are 0, 1 and 2. Index 3 is outside the list.
