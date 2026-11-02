# DataFrame Homework: Tutor Solutions

## Task 1
```python
import pandas as pd
df = pd.read_csv("social_media_posts.csv")
print(df.head())
print(df.columns)
print(df.shape)
```

## Task 2
```python
df[["post_id","platform","likes"]]
```

## Task 3
```python
df[df["likes"] >= 12][["post_id","likes"]]
```

## Task 4
```python
df[(df["platform"]=="Forum") & (df["likes"]>=10)]
```

## Task 5
```python
df["engagement"]=df["likes"]+df["comments"]
df[["post_id","engagement"]]
```

## Task 6
```python
df["word_count"]=df["text"].str.split().str.len()
df[df["word_count"]>=6]
```

## Task 7
```python
print(df["likes"].mean())
print(df["comments"].mean())
print(df["engagement"].max())
print(df["engagement"].min())
```

## Task 8
```python
df.groupby("platform")["likes"].mean()
```

## Task 9
```python
df.sort_values("likes",ascending=False).head(3)
```

## Task 10
```python
import matplotlib.pyplot as plt
df.plot(x="post_id",y="comments",kind="bar",legend=False)
plt.ylabel("Comments")
plt.title("Comments per post")
plt.show()
```

## Task 11
```python
result=df[
    (df["likes"]>=12) &
    (df["comments"]>=3) &
    (df["word_count"]>=5)
]
result[["post_id","platform","likes","comments","word_count","engagement"]]
```

## Task 12
A: quote the filename.
B: use double brackets for multiple columns.
C: compare the selected column: `df[df["likes"] >= 10]`.
D: use `&` with parentheses instead of `and`.
