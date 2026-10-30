# Design Methodology: Local Business Market Analyzer

## Design Goal

Help a new business owner think through a local service business. The original saved test used a mobile car detailing business in Bluffdale, Utah.

---

## Design Approach: Structure and Technique

**Structure I used:** Modified RTF: Role, Context, Task, Format

**Why this structure fits my task:**

- Context adds the business details needed to make the answer useful.
- Role, Task, and Format explain whose view to take, what to cover, and how to arrange the answer.

**Technique I used:** Zero shot chain of thought: asks the AI to think through the task step by step without a worked example.

**Why this technique fits my task:**
The task asks about several things that affect each other. Asking the AI to think through them step by step is meant to help it consider those connections. This instruction does not prove the answer is correct.

**Example of modifying a framework:**
I added Context to RTF so the prompt has a place for the business details.

---

## Part by Part Justification

| Part | What I put here | Why the prompt needs it |
|---|---|---|
| Role | A business advisor. | Sets the kind of help wanted. |
| Context | Business, location, budget, customers, and services. | Gives details about this business idea. |
| Task | Customers, interest, other businesses, prices, risks, and a step by step instruction. | Tells the AI what to consider. |
| Format | Summary, four lists, prices, five steps, final opinion, and word limit. | Makes the answer easier to read and use. |

---

## Testing and Iteration

These scores belong to the original prompts saved in [`examples/sample-output.md`](./examples/sample-output.md). The simpler wording in the current prompt has not been tested.

**Baseline I compared against:**

```text
Analyze the market for a mobile car-detailing business in Bluffdale, Utah, and tell me whether it could be successful.
```

| Version | Result / score | What changed |
|---|---|---|
| Naive baseline | Original recorded score: 25/100 | A plain request. |
| Version 1 | Original recorded score: 100/100 | Added the business details, budget, labeled parts, step by step instruction, and answer rules. |
| Final | Current wording has no new score | The wording was made simpler. No new test is claimed. |

**What testing showed:** The original records list 25/100 for the basic request and 100/100 for the prompt with labeled parts. The longer prompt produced clear sections, prices, five steps, and a final opinion.

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

**What I learned:** Adding Context gives the AI the location, budget, customers, and services. Task says what to look at. Format tells it how to arrange the answer.

---

## Strengths and Limitations

These points describe the prompt and saved example. They are not extra test results.

**Works well when:** The owner gives the location, budget, customers, and services.

**Struggles when:** The AI does not have checked local facts. The saved answer makes confident claims about demand and prices that still need checking.

**Would improve next:** Ask the AI to separate checked facts from guesses and price estimates.
