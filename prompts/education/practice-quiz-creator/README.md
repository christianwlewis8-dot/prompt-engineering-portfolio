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

1. Choose the grade level, age group, number of questions, and science topic.
2. Replace the placeholders in the prompt.
3. Paste the completed prompt into an AI model.

```text
Role: You are a [GRADE_LEVEL] science teacher who is very good at breaking down science concepts for [AGE_GROUP] students.

Task: I want you to create a [QUESTION_COUNT]-question multiple-choice quiz about [TOPIC] written at a [GRADE_LEVEL] reading level. Make it as easy as possible for that age group to understand.

Format: The quiz should be multiple choice with exactly four answer choices for each question. Include a complete answer key at the end.
```
