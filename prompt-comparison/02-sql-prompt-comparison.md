# Prompt Comparison 2: SQL

## Prompt
Write an SQL query to find the second highest salary from an Employee table.

## ChatGPT Response
```sql
SELECT MAX(salary) AS second_highest_salary
FROM Employee
WHERE salary < (SELECT MAX(salary) FROM Employee);
```

## Google Gemini Response
```sql
SELECT DISTINCT salary
FROM Employee
ORDER BY salary DESC
LIMIT 1 OFFSET 1;
```

## Comparison
- Both methods are common and valid in many SQL engines.
- ChatGPT query is simple and readable.
- Gemini query is compact but depends on `LIMIT/OFFSET` support.

## Evaluation Table
| Criteria | ChatGPT | Gemini | Notes |
|---|---|---|---|
| Accuracy | 5/5 | 4/5 | Gemini may vary by SQL dialect |
| Clarity | 5/5 | 4/5 | ChatGPT easier to explain |
| Completeness | 4/5 | 4/5 | Both solve core task |
| Relevance | 5/5 | 5/5 | Matches prompt |
| Instruction Following | 5/5 | 5/5 | Both follow instruction |
| Reasoning | 4/5 | 4/5 | Correct approach |
| Overall Quality | 4.7/5 | 4.3/5 | ChatGPT safer cross-dialect |

## Final Observation
ChatGPT’s method is more interview-friendly for beginners due to better compatibility.