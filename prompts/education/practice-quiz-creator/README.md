# Practice Quiz Creator

> *Generates tailored multiple-choice science practice quizzes with answer keys for elementary students.*

## Overview

This prompt uses the R-T-F (Role, Task, Format) framework to create a customized science practice quiz. It defines the teacher's role, identifies the quiz topic and intended grade level, and gives clear requirements for the questions and answer key.

**Best for:**

- Quickly creating practice quizzes for science topics
- Matching the vocabulary and difficulty to a specific grade level
- Reviewing important concepts before a test

**Structure:** R-T-F Framework (Role, Task, Format)

**Technique:** Zero-shot prompting

**Output:** A multiple-choice quiz with four choices per question and a complete answer key.

---

## Quick Start

1. Open [`prompt.md`](./prompt.md) and copy the template.
2. Replace the placeholders:
   - `[GRADE_LEVEL]`: Target grade level for the reading difficulty (e.g., 5th grade).
   - `[AGE_GROUP]`: Target age range of the students (e.g., 10- and 11-year-olds).
   - `[QUESTION_COUNT]`: Total number of questions to generate (e.g., 3).
   - `[TOPIC]`: Specific science topic being tested (e.g., the water cycle).
3. Paste it into your AI model of choice and run it.
4. Review the output and adapt it to what you need.

---

## Examples

See the [`examples/`](./examples/) folder for filled-in demonstrations showing the prompt and the resulting output.

---

## Customization Tips

- **Want more detail?** Increase [QUESTION_COUNT] for a longer quiz.
- **Want it shorter?** Reduce [QUESTION_COUNT] for a shorter quiz.
- **Different context?** Change [GRADE_LEVEL], [AGE_GROUP], and [TOPIC] for another science class.

---

## Technical Details

- **Structure:** R-T-F Framework (Role, Task, Format)
- **Technique:** Zero-shot prompting
- **Best models:** No comparison across models has been documented.
- **Placeholders:** 4 inputs: `[GRADE_LEVEL]`, `[AGE_GROUP]`, `[QUESTION_COUNT]`, `[TOPIC]`.
