# Prompt Refinement 1: Python Debugging

## Original Prompt
Fix this Python code.

## Original Response
The model gave a generic answer: “Please share the code so I can help fix it.”

## Improved Prompt
Fix the error in this code and explain the fix in one sentence:
```python
nums = [1, 2, 3]
print(nums[3])
```

## Improved Response
```python
nums = [1, 2, 3]
print(nums[2])
```
Explanation: List indexing starts at 0, so valid indexes are 0 to 2.

## Why Improved Prompt Gives Better Output
The improved prompt includes the actual code and asks for a specific type of explanation. This gives the model enough context to provide a direct and correct fix.