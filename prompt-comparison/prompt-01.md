# Prompt Comparison 01: Python Task

## Prompt
Write a Python function to check whether a number is even or odd.

## ChatGPT Response
```python
def check_even_odd(n):
    if n % 2 == 0:
        return "Even"
    else:
        return "Odd"
```

## Google Gemini Response
```python
def even_or_odd(number):
    return "Even" if number % 2 == 0 else "Odd"
```

## Comparison
Both responses are correct. ChatGPT gives a more step-by-step style that beginners usually find easier. Gemini gives a shorter one-line return, which is concise but slightly less beginner-friendly.

## Evaluation Table
| Criteria | ChatGPT | Gemini | Notes |
|---|---|---|---|
| Accuracy | 5/5 | 5/5 | Both are correct |
| Clarity | 5/5 | 4/5 | ChatGPT is simpler for beginners |
| Completeness | 4/5 | 4/5 | Could include sample input/output |
| Relevance | 5/5 | 5/5 | Both match prompt |
| Instruction Following | 5/5 | 5/5 | Fully followed |
| Reasoning | 4/5 | 4/5 | Logic is straightforward |
| Overall Quality | 4.7/5 | 4.6/5 | Both are strong |

## Final Observation
For interview explanation, ChatGPT’s version is easier to walk through line by line.