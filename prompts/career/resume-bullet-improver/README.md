# Resume Bullet Improver

> *Turns a basic job description into clear resume bullets without making up details.*

## Overview

This prompt helps someone describe work they have done. It asks for three short options based on the person's real duties and includes an example of the writing style.

**Best for:**

- Describing experience from a part time job
- Showing skills learned at work
- Getting three short ways to describe the same experience

**Structure:** CARE: Context, Action, Result, Example

**Technique:** Few shot: shows an example for the AI to follow.

**Output:** Three resume bullets, each one sentence and fewer than 30 words.

---

## Quick Start

1. Open [`prompt.md`](./prompt.md) and copy the prompt.
2. Fill in these blanks:
   - `[APPLICANT_DESCRIPTION]`: Who is writing the resume, such as a high school student.
   - `[TARGET_JOB]`: The job they want.
   - `[ORIGINAL_BULLET]`: The resume sentence they want to improve.
   - `[RESPONSIBILITIES]`: The work they actually did.
3. Paste the prompt into an AI chat.
4. Read the answer and check it before using it.

---

## Examples

See [`examples/`](./examples/) for saved prompts and answers. The [original example](./examples/output_comparison.md) uses the earlier wording.

---

## Customization Tips

- **Want more detail?** Add more useful details to the inputs.
- **Want it shorter?** Ask for a shorter answer.
- **Different context?** Change the inputs to fit the person or situation.

---

## Technical Details

- **Structure:** CARE: Context, Action, Result, Example
- **Technique:** Few shot: shows an example for the AI to follow.
- **Best models:** No comparison between AI models has been recorded.
- **Placeholders:** 4 blanks: `[APPLICANT_DESCRIPTION]`, `[TARGET_JOB]`, `[ORIGINAL_BULLET]`, `[RESPONSIBILITIES]`.
