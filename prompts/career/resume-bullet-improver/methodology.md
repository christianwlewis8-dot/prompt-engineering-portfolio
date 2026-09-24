# Methodology & Prompt Design

## Design Choices

- **Structure:** C-A-R-E (Context, Action, Result, Example) Framework
- **Technique:** Few-shot prompting
- **Target User:** A high school student creating a resume for a part-time job

### Rationale

The C-A-R-E framework was selected because resume writing requires both personal background and strict output rules. The **Context** supplies the applicant's experience and original bullet. The **Action** explains how the bullet should be improved. The **Result** sets the number, tone, and length of the responses. The **Example** demonstrates the expected style.

Few-shot prompting was selected because the included weak-to-strong example gives the model a pattern to follow. This helps produce concise, action-oriented writing without requiring the model to guess the desired style.

---

## Evaluation & Iteration Results

### Naive Prompt (Baseline)

> Improve this resume bullet: Detailed cars for customers.

- **Score:** 25/100
- **Rubric Breakdown:**
  - Clarity & Specificity: 15/30
  - Structure & Framework Use: 0/30
  - Context & Inputs: 10/20
  - Output Requirements: 0/20
- **Evaluator Feedback:** The task was understandable, but it lacked a framework, job context, responsibility details, and requirements for tone, length, or output structure.

### Designed Prompt (C-A-R-E)

> **Context:** I am a high school student creating a resume for a part-time job. I run a small car-detailing business where I clean vehicle interiors and exteriors, communicate with customers, schedule appointments, and complete jobs independently. My original resume bullet is: "Detailed cars for customers."
>
> **Action:** Rewrite this into a stronger resume bullet that clearly explains my responsibilities and skills. Use a strong action verb and focus on skills that would matter to an employer. Do not make up numbers, customer ratings, or services that I did not provide.
>
> **Result:** Give me three different resume-bullet options. Keep each option to one sentence, use a professional but natural tone, and keep each one under 30 words.
>
> **Example:** A weak bullet such as "Mowed lawns for people" could become "Managed recurring lawn-care jobs for local customers while maintaining dependable scheduling, clear communication, and consistent work quality."

- **Score:** 100/100
- **Rubric Breakdown:**
  - Clarity & Specificity: 30/30
  - Structure & Framework Use: 30/30
  - Context & Inputs: 20/20
  - Output Requirements: 20/20
- **Evaluator Feedback:** The complete C-A-R-E framework supplied relevant background and strict constraints. The example demonstrated the intended style, while the accuracy guardrail prevented invented metrics or responsibilities.

---

## Key Takeaways

Adding the applicant's background, actual responsibilities, output count, word limit, tone, and example improved the score by 75 points. The designed prompt produced three concise bullets that accurately highlighted independence, scheduling, customer communication, and detailing experience.
