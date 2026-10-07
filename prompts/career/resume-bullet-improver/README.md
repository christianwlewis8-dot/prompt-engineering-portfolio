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

1. Open [`prompt.md`](./prompt.md) and copy the template.
2. Replace the placeholders:
   - `[APPLICANT_DESCRIPTION]`: The applicant's current level or background (e.g., high school student).
   - `[TARGET_JOB]`: The job or type of position being pursued (e.g., part-time customer-service job).
   - `[ORIGINAL_BULLET]`: The basic resume bullet that needs improvement.
   - `[RESPONSIBILITIES]`: Duties and skills the applicant actually performed.
3. Paste it into your AI model of choice and run it.
4. Review the output and adapt it to what you need.

---

## Examples

See the [`examples/`](./examples/) folder for filled-in demonstrations showing the prompt and the resulting output.

---

## Customization Tips

- **Want more detail?** Provide more actual responsibilities in [RESPONSIBILITIES].
- **Want it shorter?** Lower the word limit in the Result section.
- **Different context?** Change [APPLICANT_DESCRIPTION] and [TARGET_JOB] for another applicant or role.

---

## Technical Details

- **Structure:** C-A-R-E Framework (Context, Action, Result, Example)
- **Technique:** Few-shot prompting
- **Best models:** No comparison across models has been documented.
- **Placeholders:** 4 inputs: `[APPLICANT_DESCRIPTION]`, `[TARGET_JOB]`, `[ORIGINAL_BULLET]`, `[RESPONSIBILITIES]`.
