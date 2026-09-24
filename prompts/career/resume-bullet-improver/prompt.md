# Resume Bullet Improver Template

## Overview

**Purpose:** Rewrites a basic work-experience statement into several concise, professional resume bullets.

**Structure:** C-A-R-E Framework (Context, Action, Result, Example)

**Technique:** Few-shot prompting

---

## The Prompt

Context: I am a [APPLICANT_DESCRIPTION] creating a resume for [TARGET_JOB]. My original resume bullet is: "[ORIGINAL_BULLET]." My actual responsibilities included [RESPONSIBILITIES].

Action: Rewrite this into a stronger resume bullet that clearly explains my responsibilities and skills. Use a strong action verb and focus on skills that would matter to an employer. Do not make up numbers, ratings, or responsibilities.

Result: Give me three different resume-bullet options. Keep each option to one sentence, use a professional but natural tone, and keep each one under 30 words.

Example: A weak bullet such as "Mowed lawns for people" could become "Managed recurring lawn-care jobs for local customers while maintaining dependable scheduling, clear communication, and consistent work quality."

---

## Context and Inputs

- **[APPLICANT_DESCRIPTION]:** The applicant's current level or background (e.g., high school student).
- **[TARGET_JOB]:** The job or type of position being pursued (e.g., part-time customer-service job).
- **[ORIGINAL_BULLET]:** The basic resume bullet that needs improvement.
- **[RESPONSIBILITIES]:** Duties and skills the applicant actually performed.

---

## Output Requirements

- **Options:** Exactly three revised resume bullets.
- **Length:** Each option must contain one sentence and fewer than 30 words.
- **Style:** Professional, natural, concise, and action-oriented.
- **Relevance:** Focus on skills that would matter to an employer.
- **Accuracy:** Do not invent numbers, ratings, duties, or accomplishments.
