# Local Business Market Analyzer

> *Helps someone think through a local business idea.*

## Overview

This prompt looks at who might buy a service, what other businesses offer, and what prices might work. It also asks about problems, costs, and steps the owner could take.

**Best for:**

- Thinking through a local business idea
- Looking at customers, other businesses, and prices
- Choosing practical next steps

**Structure:** Modified RTF: Role, Context, Task, Format

**Technique:** Zero shot chain of thought: asks the AI to think through the task step by step without a worked example.

**Output:** A short summary, strengths and weaknesses, chances to grow, outside risks, price ranges, five next steps, and a final opinion.

---

## Quick Start

1. Open [`prompt.md`](./prompt.md) and copy the prompt.
2. Fill in these blanks:
   - `[BUSINESS_TYPE]`: The kind of business, such as mobile car detailing.
   - `[LOCATION]`: The city or area the business will serve.
   - `[STARTING_BUDGET]`: How much money is available to start.
   - `[TARGET_CUSTOMERS]`: The people the business hopes to serve.
   - `[SERVICES]`: The services the business will offer.
3. Paste the prompt into an AI chat.
4. Read the answer and check it before using it.

---

## Examples

See [`examples/`](./examples/) for saved prompts and answers. The [original example](./examples/sample-output.md) uses the earlier wording.

---

## Customization Tips

- **Want more detail?** Add more useful details to the inputs.
- **Want it shorter?** Ask for a shorter answer.
- **Different context?** Change the inputs to fit the person or situation.

---

## Technical Details

- **Structure:** Modified RTF: Role, Context, Task, Format
- **Technique:** Zero shot chain of thought: asks the AI to think through the task step by step without a worked example.
- **Best models:** No comparison between AI models has been recorded.
- **Placeholders:** 5 blanks: `[BUSINESS_TYPE]`, `[LOCATION]`, `[STARTING_BUDGET]`, `[TARGET_CUSTOMERS]`, `[SERVICES]`.
