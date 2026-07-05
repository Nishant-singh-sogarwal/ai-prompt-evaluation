# Prompt Comparison 02: SQL Task

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
Both methods are commonly used. ChatGPT's query is easy to explain and works well in many databases. Gemini’s query is short, but `LIMIT/OFFSET` syntax may vary by SQL engine.

## Evaluation Table
| Criteria | ChatGPT | Gemini | Notes |
|---|---|---|---|
| Accuracy | 5/5 | 4/5 | Gemini depends on SQL dialect |
| Clarity | 5/5 | 4/5 | ChatGPT easier for freshers |
| Completeness | 4/5 | 4/5 | Both solve core problem |
| Relevance | 5/5 | 5/5 | Fully relevant |
| Instruction Following | 5/5 | 5/5 | Followed correctly |
| Reasoning | 4/5 | 4/5 | Good logic |
| Overall Quality | 4.7/5 | 4.3/5 | ChatGPT slightly safer |

## Final Observation
ChatGPT’s version is better for beginner interviews because it is highly readable and less dialect-dependent.