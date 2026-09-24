# Resume Bullet Improver

> *Turns a basic description of work experience into concise, professional resume bullets without inventing details.*

## Overview

This prompt uses the C-A-R-E (Context, Action, Result, Example) framework to improve a weak resume bullet. It gives the AI background about the applicant, explains the requested revision, defines the required output, and provides an example of the desired style.

**Best for:**

- Improving resume bullets for part-time jobs
- Highlighting responsibilities and transferable skills
- Creating multiple concise options without fake metrics

**Structure:** C-A-R-E Framework (Context, Action, Result, Example)

**Technique:** Few-shot prompting

**Output:** Three professional, one-sentence resume bullets under 30 words each.

---

## Quick Start

1. Enter the applicant's background, target job, original bullet, and actual responsibilities.
2. Replace the placeholders in the prompt.
3. Paste the completed prompt into an AI model.

```text
Context: I am a [APPLICANT_DESCRIPTION] creating a resume for [TARGET_JOB]. My original resume bullet is: "[ORIGINAL_BULLET]." My actual responsibilities included [RESPONSIBILITIES].

Action: Rewrite this into a stronger resume bullet that clearly explains my responsibilities and skills. Use a strong action verb and focus on skills that would matter to an employer. Do not make up numbers, ratings, or responsibilities.

Result: Give me three different resume-bullet options. Keep each option to one sentence, use a professional but natural tone, and keep each one under 30 words.

Example: A weak bullet such as "Mowed lawns for people" could become "Managed recurring lawn-care jobs for local customers while maintaining dependable scheduling, clear communication, and consistent work quality."
```
