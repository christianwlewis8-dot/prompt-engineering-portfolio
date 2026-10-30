# Design Methodology: Resume Bullet Improver

## Design Goal

Help a high school student applying for a part time job describe work clearly without making up experience.

---

## Design Approach: Structure and Technique

**Structure I used:** CARE: Context, Action, Result, Example

**Why this structure fits my task:**

- Context gives the person's experience, and Action explains what to improve.
- Result sets the length and number of options. Example shows the writing style.

**Technique I used:** Few shot: shows an example for the AI to follow.

**Why this technique fits my task:**
The sample shows how a basic sentence can become a clearer resume bullet.

---

## Part by Part Justification

| Part | What I put here | Why the prompt needs it |
|---|---|---|
| Context | Background, target job, original sentence, and real duties. | Gives facts the AI can use. |
| Action | What to improve and what not to invent. | Keeps the rewrite focused on real experience. |
| Result | Three bullets, one sentence each, fewer than 30 words. | Keeps the answer short. |
| Example | A basic lawn care bullet and a clearer version. | Shows the writing style. |

---

## Testing and Iteration

These scores belong to the original prompts saved in [`examples/output_comparison.md`](./examples/output_comparison.md). The simpler wording in the current prompt has not been tested.

**Baseline I compared against:**

```text
Improve this resume bullet: Detailed cars for customers.
```

| Version | Result / score | What changed |
|---|---|---|
| Naive baseline | Original recorded score: 25/100 | A plain request. |
| Version 1 | Original recorded score: 100/100 | Added background, real duties, rules against invented details, a word limit, and an example. |
| Final | Current wording has no new score | The wording was made simpler. No new test is claimed. |

**What testing showed:** The original records list 25/100 for the basic request and 100/100 for the prompt with labeled parts. The basic answer added duties and suggested numbers the user had not provided. The designed answer gave three short options about detailing, scheduling, and customer communication.

Original basic prompt scores:

| Category | Basic prompt |
|---|---:|
| Clarity & Specificity | 15/30 |
| Structure & Framework Use | 0/30 |
| Context & Inputs | 10/20 |
| Output Requirements | 0/20 |

Original designed prompt scores:

| Category | Designed prompt |
|---|---:|
| Clarity & Specificity | 30/30 |
| Structure & Framework Use | 30/30 |
| Context & Inputs | 20/20 |
| Output Requirements | 20/20 |

**What I learned:** Context gives the facts. Action explains the change. Result sets the length and number of options. Example shows the style.

---

## Strengths and Limitations

These points describe the prompt and saved example. They are not extra test results.

**Works well when:** The person gives real duties and the job they want.

**Struggles when:** The duties are vague. The lawn care example adds scheduling and communication that its short starting sentence does not explain.

**Would improve next:** Give the example its own list of real duties and check that the AI does not copy duties into an unrelated resume.
