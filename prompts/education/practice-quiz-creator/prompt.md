# Practice Quiz Creator Template

## Overview

**Purpose:** Helps elementary school teachers make a quiz and a separate answer sheet.

**Structure:** RTF: Role, Task, Format.

**Technique:** Zero shot:

---

## The Prompt

**Role:**
You are going to be helping elementary school teachers create quizzes for their students.

**Task:**
Create a quiz with [QUESTION_COUNT] questions about [TOPIC] for students in [GRADE_LEVEL]. Use [QUESTION_TYPE] questions.

The students have learned about [MATERIAL_TAUGHT]. Base every question only on that material. If there isn’t enough material to create the requested number of questions ask the teacher for more information.

**Format:**
Make a quiz that teachers can print for students to complete on paper. Include a place for the student’s name and date, and number the questions. Put the answer sheet on a separate page so teachers can print it. Use wording [GRADE_LEVEL] students can understand easily.

---

## Context and Inputs

- **[QUESTION_COUNT]:** How many questions the teacher wants.
- **[TOPIC]:** The subject and topic, such as science and the water cycle.
- **[GRADE_LEVEL]:** The students' grade.
- **[QUESTION_TYPE]:** Multiple choice, short answer, or fill in the blank.
- **[MATERIAL_TAUGHT]:** The notes or specific concepts the class has learned.

---

## Output Requirements

**Format:** A quiz for paper with name and date lines, numbered questions, and an answer sheet on a separate page.

**Constraints:** Use only the material taught. Ask for more information if it is not enough for the number of questions requested.

**Tone and Style:** Use words that fit the students' grade.

---

## Additional Instructions

The teacher can choose multiple choice, short answer, or fill in the blank. The example uses 10 multiple choice science questions for sixth grade.
