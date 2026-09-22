# Practice Quiz Creator Template

## Overview

**Purpose:** Generates a customized multiple-choice practice quiz and answer key tailored to a specific grade level and topic.

**Structure:** R-T-F Framework (Role, Task, Format)

**Technique:** Zero-shot prompting

---

## The Prompt

Role: You are a [GRADE_LEVEL] science teacher who is very good at breaking down science concepts for [AGE_GROUP] students.

Task: I want you to create a [QUESTION_COUNT]-question multiple-choice quiz about [TOPIC] written at a [GRADE_LEVEL] reading level. Make it as easy as possible for that age group to understand.

Format: The quiz should be multiple choice with exactly four answer choices for each question. Include a complete answer key at the end.

---

## Context and Inputs

- **[GRADE_LEVEL]:** Target grade level for the reading difficulty (e.g., 5th grade).
- **[AGE_GROUP]:** Target age range of the students (e.g., 10- and 11-year-olds).
- **[QUESTION_COUNT]:** Total number of questions to generate (e.g., 3).
- **[TOPIC]:** Specific science topic being tested (e.g., the water cycle).

---

## Output Requirements

- **Question Count:** Exactly the number requested in [QUESTION_COUNT].
- **Options:** Exactly four multiple-choice options per question.
- **Answer Key:** A complete answer key at the end.
- **Reading Level:** Language and vocabulary appropriate for the specified grade level and age group.
