# Practice Quiz Creator

> *Makes a science quiz and answer key for elementary students.*

## Overview

Teachers can choose a science topic, grade, student age, and number of questions. The prompt asks for clear questions with four choices and an answer key.

**Best for:**

- Making science practice quizzes
- Choosing words that fit the students' grade
- Reviewing a topic before a test

**Structure:** RTF: Role, Task, Format

**Technique:** Zero shot: gives instructions without an example.

**Output:** A multiple choice quiz with four choices for each question and an answer key.

---

## Quick Start

1. Open [`prompt.md`](./prompt.md) and copy the prompt.
2. Fill in these blanks:
   - `[GRADE_LEVEL]`: The students' grade, such as fifth grade.
   - `[AGE_GROUP]`: The students' ages, such as 10 and 11.
   - `[QUESTION_COUNT]`: The number of questions.
   - `[TOPIC]`: The science topic.
3. Paste the prompt into an AI chat.
4. Read the answer and check it before using it.

---

## Examples

See [`examples/`](./examples/) for saved prompts and answers. The [original example](./examples/output_comparison.md) uses the earlier wording.

---

## Customization Tips

- **Want more detail?** Add more useful details to the inputs.
- **Want it shorter?** Ask for a shorter answer.
- **Different context?** Change the inputs to fit the person or situation.

---

## Technical Details

- **Structure:** RTF: Role, Task, Format
- **Technique:** Zero shot: gives instructions without an example.
- **Best models:** No comparison between AI models has been recorded.
- **Placeholders:** 4 blanks: `[GRADE_LEVEL]`, `[AGE_GROUP]`, `[QUESTION_COUNT]`, `[TOPIC]`.
