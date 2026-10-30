# Prompt Structures and Techniques

## Structures

A structure gives each part of a prompt a clear job.

| Name | Parts | Where it is used |
|---|---|---|
| RTF | Role: who the AI should act as. Task: what to do. Format: how to present the answer. | [Quiz creator](../prompts/education/practice-quiz-creator/prompt.md) |
| Modified RTF | Role, Context, Task, Format. Context gives details about the situation. | [Business prompt](../prompts/business/market-analysis/prompt.md) |
| CARE | Context: background. Action: what to change. Result: what the answer should look like. Example: a sample to follow. | [Resume prompt](../prompts/career/resume-bullet-improver/prompt.md) |

## Techniques

A technique is the way a prompt guides the AI.

| Name | What it means | Where it is used |
|---|---|---|
| Zero shot | Gives instructions without examples. | Quiz creator |
| Few shot | Gives examples for the AI to follow. | Resume prompt |
| Zero shot chain of thought | Asks the AI to think through a task step by step without a worked example. | Business prompt |

## Scoring

| Category | Points |
|---|---:|
| Clarity & Specificity | 30 |
| Structure & Framework Use | 30 |
| Context & Inputs | 20 |
| Output Requirements | 20 |
| **Total** | **100** |

Keep scores and comparisons in the methodology and examples files. A score for an earlier prompt is not a score for a changed prompt.
