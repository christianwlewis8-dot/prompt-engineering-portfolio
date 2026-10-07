# Local Business Market Analyzer

> *Creates a clear market analysis for a local service business using its location, budget, customers, and services.*

## Overview

This prompt uses a modified R-T-F structure with an added Context section. It helps a new business owner evaluate customers, competition, pricing, opportunities, challenges, and financial risks before deciding whether an idea is worth pursuing.

**Best for:**

- Evaluating a local service-business idea
- Identifying customers, competitors, and pricing opportunities
- Creating a simple SWOT analysis and action plan

**Structure:** Modified R-T-F Framework (Role, Context, Task, Format)

**Technique:** Zero-shot chain-of-thought prompting

**Output:** An executive summary, SWOT analysis, pricing guidance, five action steps, and a final recommendation.

---

## Quick Start

1. Open [`prompt.md`](./prompt.md) and copy the template.
2. Replace the placeholders:
   - `[BUSINESS_TYPE]`: The kind of local service business being considered (e.g., mobile car detailing).
   - `[LOCATION]`: The city or service area where the business would operate (e.g., Bluffdale, Utah).
   - `[STARTING_BUDGET]`: The money available to launch the business (e.g., $1,000).
   - `[TARGET_CUSTOMERS]`: The main customers the business wants to serve (e.g., busy families and vehicle owners).
   - `[SERVICES]`: The main services the business would provide (e.g., interior, exterior, and full detailing packages).
3. Paste it into your AI model of choice and run it.
4. Review the output and adapt it to what you need.

---

## Examples

See the [`examples/`](./examples/) folder for filled-in demonstrations showing the prompt and the resulting output.

---

## Customization Tips

- **Want more detail?** Supply more specific customer and service details in [TARGET_CUSTOMERS] and [SERVICES].
- **Want it shorter?** Lower the word limit in the Format section.
- **Different context?** Replace the business type, location, budget, customers, and services for another local business.

---

## Technical Details

- **Structure:** Modified R-T-F Framework (Role, Context, Task, Format)
- **Technique:** Zero-shot chain-of-thought prompting
- **Best models:** No comparison across models has been documented.
- **Placeholders:** 5 inputs: `[BUSINESS_TYPE]`, `[LOCATION]`, `[STARTING_BUDGET]`, `[TARGET_CUSTOMERS]`, `[SERVICES]`.
