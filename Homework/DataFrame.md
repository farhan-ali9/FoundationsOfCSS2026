# FCSS Homework: DataFrames and Social-Media Analysis

Use `social_media_posts.csv`.

## Task 1
Load the CSV, show the first 5 rows, print the columns, and print the shape.

## Task 2
Display only `post_id`, `platform`, and `likes`.

## Task 3
Show posts with at least 12 likes. Display only `post_id` and `likes`.

## Task 4
Show Forum posts with at least 10 likes.

## Task 5
Create:
```python
df["engagement"] = df["likes"] + df["comments"]
```
Display `post_id` and `engagement`.

## Task 6
Create:
```python
df["word_count"] = df["text"].str.split().str.len()
```
Find posts with at least 6 words.

## Task 7
Calculate average likes, average comments, maximum engagement, and minimum engagement.

## Task 8
Calculate average likes for each platform.

## Task 9
Sort from highest to lowest likes and show the top 3 posts.

Hint:
```python
df.sort_values("likes", ascending=False)
```

## Task 10
Create a bar chart of comments per post with a title and y-axis label.

## Task 11
Find posts with at least 12 likes, at least 3 comments, and at least 5 words. Display `post_id`, `platform`, `likes`, `comments`, `word_count`, and `engagement`.

## Task 12: Fix the errors

A
```python
df = pd.read_csv(social_media_posts.csv)
```

B
```python
df["post_id", "likes"]
```

C
```python
df[df["likes" >= 10]]
```

D
```python
df[(df["likes"] >= 10) and (df["comments"] >= 3)]
```

For each, fix the code and explain the problem in one sentence.
