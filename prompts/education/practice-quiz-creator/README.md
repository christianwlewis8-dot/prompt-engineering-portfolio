# Practice Quiz Creator

> Helps elementary teachers make paper quizzes and answer sheets.

## Overview

Teachers enter the topic, grade, question count, question type, and material already taught. The prompt asks for a quiz that stays within that material and uses words that fit the class.

**Best for:**

- Teachers who need to make a simple quiz fast
- Testing simple topics
- Pop Quizzes

**Structure:** RTF: Role, Task, Format.

**Technique:** Zero shot

**Output:** A quiz with name and date lines, numbered questions, and a separate answer sheet.

---

## Quick Start

1. Open [prompt.md](./prompt.md) and copy the prompt.
2. Fill in the blanks:
   - [QUESTION_COUNT]: Number of questions.
   - [TOPIC]: Subject and topic.
   - [GRADE_LEVEL]: Students grade.
   - [QUESTION_TYPE]: Multiple choice, short answer, or fill in the blank.
   - [MATERIAL_TAUGHT]: Notes or specific concepts taught in class.
3. Paste it into an AI chat.
4. Check the questions and answers.

---

## Examples

See [examples/](./examples/) for saved prompts and answers.

Th example uses 10 multiple choice questions about the water cycle for sixth grade.

---

## Customization Tips

- **Want more detail?** Add more class notes to [MATERIAL_TAUGHT].
- **Want it shorter?** Lower [QUESTION_COUNT].
- **Different class?** Change the topic, grade, or question type.

---

## Technical Details

- **Structure:** RTF: Role, Task, Format.
- **Technique:** Zero shot
- **Placeholders:** [QUESTION_COUNT], [TOPIC], [GRADE_LEVEL], [QUESTION_TYPE], and [MATERIAL_TAUGHT].
