# Methodology & Prompt Design

## Design Choices

- **Structure:** R-T-F (Role, Task, Format) Framework
- **Technique:** Zero-shot prompting
- **Target Audience:** 5th-grade science students (ages 10-11)

### Rationale

The R-T-F framework was selected because educational prompts require a specific persona and clear output formatting to reach the correct reading level. By assigning a clear **Role** (5th-grade science teacher), the model adopts an encouraging, accessible tone. The **Task** specifies the topic and reading-level constraint, while the **Format** defines the question structure and answer-key requirements.

Zero-shot prompting was selected because the instructions fully describe the requested quiz without requiring an example for the model to copy.

---

## Evaluation & Iteration Results

### Naive Prompt (Baseline)

> Make a 3-question multiple-choice quiz about the water cycle with an answer key.

- **Score:** 25/100
- **Evaluator Feedback:** The prompt lacked essential context, grade-level targets, and specific output parameters, forcing the AI to guess the target audience and depth.

### Designed Prompt (R-T-F)

> **Role:** You are a 5th-grade science teacher who is very good at breaking down science concepts for 10- and 11-year-old students.
>
> **Task:** I want you to create a 3-question multiple-choice quiz about the water cycle written at a 5th-grade reading level. Make it as easy as possible for that age group to understand.
>
> **Format:** The quiz should be multiple choice with exactly four answer choices for each question. Include a complete answer key at the end.

- **Score:** 100/100
- **Evaluator Breakdown:**
  - Clarity & Specificity: 30/30
  - Structure & Framework Use: 30/30
  - Context & Inputs: 20/20
  - Output Requirements: 20/20
- **Evaluator Feedback:** Clean execution of the labeled R-T-F structure with actionable detail. By defining the target demographic, question count, choice parameters, and answer-sheet expectations, it removed ambiguity for the AI.

---

## Key Takeaways

Explicitly declaring the audience age, question constraints, and formatting rules improved the score by 75 points. Giving the AI a defined role prevented generic, high-level explanations and matched the vocabulary to a 5th-grade reading level.
