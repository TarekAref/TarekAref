# IBM SkillsBuild: Troubleshooting Code with IBM Granite

**Completed:** July 31, 2026  
**Platform:** IBM SkillsBuild  
**Topics:** Generative AI, IBM Granite, code troubleshooting, prompt engineering

## Overview

This module covered how IBM Granite large language models can help developers generate, explain, review, and troubleshoot code. Granite models use machine learning and natural language processing to respond to developer instructions and support coding workflows.

## Key concepts

- **Base models** support code generation, completion, and bug fixing.
- **Instruct models** are optimized to follow detailed prompts and automate tasks.
- Granite model sizes discussed in the module included **3B, 8B, 20B, and 34B**.
- IBM watsonx Prompt Lab can be used to test prompts and troubleshoot code with Granite.

## Common code errors

| Error type | What it means | Typical fix |
|---|---|---|
| Syntax error | The code breaks the programming language's grammar or punctuation rules. | Check brackets, parentheses, punctuation, spelling, and indentation. |
| Logical error | The program runs but produces the wrong result. | Review formulas, conditions, loops, and expected outputs. |
| Functional error | The program does not fully perform the required task. | Compare the implementation with requirements and add missing behavior. |
| Name error | A variable, function, or object has not been defined or imported. | Define or import it, then verify spelling and scope. |

## Example: missing return statement

### Problem

```python
def calculate_total(price, quantity):
    total = price * quantity

result = calculate_total(25, 4)
print(result)
```

The function calculates a value but does not return it, so Python outputs `None`.

### Corrected code

```python
def calculate_total(price, quantity):
    total = price * quantity
    return total

result = calculate_total(25, 4)
print(result)  # 100
```

## Example Granite prompt

```text
Review this Python function. Its output is unexpectedly empty.
Check for a missing return statement, explain the problem,
and provide corrected code.
```

## Benefits of using Granite for troubleshooting

- Faster error identification
- Clear explanations of coding problems
- Improved code quality
- Better collaboration through understandable documentation
- More accessible coding support for beginners
- Personalized suggestions based on the supplied code and prompt

## Learning outcomes

After completing this module, I can:

- Identify IBM Granite model types used for code generation
- Explain the benefits of Granite for developers
- Recognize syntax, logical, functional, and name errors
- Write prompts that ask a model to identify, explain, and fix code
- Use IBM watsonx Prompt Lab as part of a troubleshooting workflow

## Reflection

This module strengthened my understanding of how generative AI can support software development without replacing developer judgment. The best results come from giving the model clear context, naming the suspected error type, reviewing the response, and testing the corrected code.
