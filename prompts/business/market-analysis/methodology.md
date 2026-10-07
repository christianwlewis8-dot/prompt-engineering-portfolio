# Design Methodology: Local Business Market Analyzer

## Design Goal

Help a new local service-business owner assess customers, competition, pricing, opportunities, challenges, and financial risks. The existing test examines a mobile car-detailing business in Bluffdale, Utah.

---

## Design Approach: Structure and Technique

**Structure I used:** Modified R-T-F Framework (Role, Context, Task, Format)

**Why this structure fits my task:**

- Market analysis depends on business details, so Context adds location, budget, customers, and services.
- Role, Task, and Format specify the advisor perspective, analytical scope, and required deliverables.

**Technique I used:** Zero-shot chain-of-thought prompting

**Why this technique fits my task:**
Zero-shot chain-of-thought prompting was selected because market analysis requires the model to consider several connected factors. The instruction to think through the market step by step encourages more careful analysis without requiring a worked example.


**Example of modifying a framework:**
I started from R-T-F (Role, Task, Format) and added Context. This section supplies the location, startup budget, target customers, and services that the plain framework left unspecified. My final structure was Role, Context, Task, Format.

---

## Part-by-Part Justification

| Part | What I put here | Why the prompt needs it |
|------|-----------------|-------------------------|
| Role | A small-business advisor. | Sets the advisory perspective. |
| Context | Business type, location, starting budget, customers, and services. | Makes the analysis specific to the proposed business. |
| Task | Demand, competition, prices, opportunities, challenges, risks, and a step-by-step instruction. | Defines the factors to consider and the reasoning technique. |
| Format | Summary, SWOT, price ranges, five actions, conclusion, word limit, and accuracy rules. | Keeps the answer organized, concise, and explicit about assumptions. |

---

## Testing and Iteration

**Baseline I compared against:**
```text
Analyze the market for a mobile car-detailing business in Bluffdale, Utah, and tell me whether it could be successful.
```

| Version | Result / score | What changed |
|---------|----------------|--------------|
| Naive baseline | Recorded score: 25/100 | Plain request without the designed structure or technique. |
| Version 1 | Recorded score: 100/100 | Added business background, budget, customers, services, labeled sections, a reasoning instruction, and output constraints. |
| Final | Same as Version 1; no separate retest documented | No further prompt revision is recorded. This formatting update does not constitute a new test. |

**What testing showed:** Adding the location, budget, customers, services, and required output format improved the score by 75 points. The designed prompt produced a more organized and practical answer with a SWOT analysis, price ranges, action steps, and a clear conclusion. It also satisfied the portfolio requirement to use a technique beyond standard zero-shot prompting.

The existing records contain one baseline and one designed run. They do not document a subsequent revision and retest. See [`examples/`](./examples/) for the saved prompts and outputs.

Existing baseline evaluation record:
- **Score:** 25/100
- **Rubric Breakdown:**
  - Clarity & Specificity: 15/30
  - Structure & Framework Use: 0/30
  - Context & Inputs: 10/20
  - Output Requirements: 0/20
- **Evaluator Feedback:** The request identified the business and location, but it lacked analytical boundaries, a prompting framework, important business details, and output requirements.

Existing designed evaluation record:
- **Score:** 100/100
- **Rubric Breakdown:**
  - Clarity & Specificity: 30/30
  - Structure & Framework Use: 30/30
  - Context & Inputs: 20/20
  - Output Requirements: 20/20
- **Evaluator Feedback:** The labeled Role, Context, Task, and Format sections provided clear analytical expectations, business background, required deliverables, a length limit, and factual guardrails. The step-by-step instruction also clearly demonstrated zero-shot chain-of-thought prompting.


**What I learned:** The R-T-F framework was expanded with a **Context** section because a useful market analysis depends on details about the location, startup budget, customers, and services. The **Role** places the model in the position of a business advisor. The **Task** identifies the areas that must be analyzed, and the **Format** controls how the final response is organized.

---

## Strengths and Limitations

The observations below describe the current prompt and saved example; they are not additional test results.

**Works well when:** The owner supplies a clear location, starting budget, target customers, and service list.

**Struggles when:** Verified local data is unavailable. The prompt prohibits invented exact statistics, but that does not verify broader claims about demand or pricing; the saved output still makes confident market claims.

**Would improve next:** Require clearer separation of supported facts, assumptions, and estimates, then test whether conclusions become better supported.
