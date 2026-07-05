# Prompt Refinement 01: Python Error Fix

## Original Prompt
Fix this Python code.

## Original Response
The model replied with a generic answer asking for the code snippet.

## Improved Prompt
Fix the error in this code and explain in one sentence:
```python
numbers = [10, 20, 30]
print(numbers[3])
```

## Improved Response
```python
numbers = [10, 20, 30]
print(numbers[2])
```
Explanation: Python list index starts from 0, so the last valid index here is 2.

## Why the Improved Prompt Gives Better Output
The improved prompt includes the exact code and a clear output expectation. This removes ambiguity and helps the model provide a direct, useful fix.