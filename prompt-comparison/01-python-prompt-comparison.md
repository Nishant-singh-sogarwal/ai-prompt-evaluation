# Prompt Comparison 1: Python

## Prompt
Write a Python function to check whether a number is even or odd.

## ChatGPT Response
```python
def check_even_odd(n):
    if n % 2 == 0:
        return "Even"
    return "Odd"
```

## Google Gemini Response
```python
def even_or_odd(number):
    return "Even" if number % 2 == 0 else "Odd"
```

## Comparison
- Both responses are correct.
- ChatGPT version is more explicit for beginners.
- Gemini version is shorter using a ternary expression.

## Evaluation Table
| Criteria | ChatGPT | Gemini | Notes |
|---|---|---|---|
| Accuracy | 5/5 | 5/5 | Both give correct logic |
| Clarity | 5/5 | 4/5 | ChatGPT is easier to read for freshers |
| Completeness | 4/5 | 4/5 | Could include input example |
| Relevance | 5/5 | 5/5 | Matches prompt exactly |
| Instruction Following | 5/5 | 5/5 | Both follow request |
| Reasoning | 4/5 | 4/5 | Logic is implied |
| Overall Quality | 4.7/5 | 4.6/5 | Both useful |

## Final Observation
For interview explanation, ChatGPT’s structure is slightly easier for beginners, while Gemini shows concise style.