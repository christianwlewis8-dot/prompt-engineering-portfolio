# Methodology & Prompt Design

## Design Choices

- **Structure:** Modified R-T-F (Role, Context, Task, Format) Framework
- **Technique:** Zero-shot chain-of-thought prompting
- **Target User:** A new local service-business owner

### Rationale

The R-T-F framework was expanded with a **Context** section because a useful market analysis depends on details about the location, startup budget, customers, and services. The **Role** places the model in the position of a business advisor. The **Task** identifies the areas that must be analyzed, and the **Format** controls how the final response is organized.

Zero-shot chain-of-thought prompting was selected because market analysis requires the model to consider several connected factors. The instruction to think through the market step by step encourages more careful analysis without requiring a worked example.

---

## Evaluation & Iteration Results

### Naive Prompt (Baseline)

> Analyze the market for a mobile car-detailing business in Bluffdale, Utah, and tell me whether it could be successful.

- **Score:** 25/100
- **Rubric Breakdown:**
  - Clarity & Specificity: 15/30
  - Structure & Framework Use: 0/30
  - Context & Inputs: 10/20
  - Output Requirements: 0/20
- **Evaluator Feedback:** The request identified the business and location, but it lacked analytical boundaries, a prompting framework, important business details, and output requirements.

### Designed Prompt (Modified R-T-F)

> **Role:** You are a business advisor who is good at helping people understand whether a small business idea could be successful.
>
> **Context:** I am looking at starting a mobile car-detailing business in Bluffdale, Utah, with a starting budget of $1,000. The business would mainly serve busy families and other vehicle owners in Bluffdale and nearby areas. It would offer interior details, exterior details, and full detailing packages.
>
> **Task:** I want you to analyze the market for this business and tell me if it would be a good idea. Think through it step by step before answering. Look at the target customers, demand, competition, possible prices, opportunities, challenges, and financial risks.
>
> **Format:** Start with a short summary and then make a SWOT analysis showing the strengths, weaknesses, opportunities, and threats. Include reasonable price ranges, five things the owner should do to help the business succeed, and a final conclusion. Use simple language, clear headings, and keep it under 700 words. Do not make up exact statistics, and explain any assumptions you make.

- **Score:** 100/100
- **Rubric Breakdown:**
  - Clarity & Specificity: 30/30
  - Structure & Framework Use: 30/30
  - Context & Inputs: 20/20
  - Output Requirements: 20/20
- **Evaluator Feedback:** The labeled Role, Context, Task, and Format sections provided clear analytical expectations, business background, required deliverables, a length limit, and factual guardrails. The step-by-step instruction also clearly demonstrated zero-shot chain-of-thought prompting.

---

## Key Takeaways

Adding the location, budget, customers, services, and required output format improved the score by 75 points. The designed prompt produced a more organized and practical answer with a SWOT analysis, price ranges, action steps, and a clear conclusion. It also satisfied the portfolio requirement to use a technique beyond standard zero-shot prompting.
