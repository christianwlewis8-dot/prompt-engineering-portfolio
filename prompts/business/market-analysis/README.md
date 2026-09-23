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

1. Choose the business type, location, budget, target customers, and services.
2. Replace the placeholders in the prompt template.
3. Paste the completed prompt into an AI model.

```text
Role: You are a business advisor who is good at helping people understand whether a small business idea could be successful.

Context: I am looking at starting a [BUSINESS_TYPE] in [LOCATION] with a starting budget of [STARTING_BUDGET]. The business would mainly serve [TARGET_CUSTOMERS]. It would offer [SERVICES].

Task: I want you to analyze the market for this business and tell me if it would be a good idea. Think through it step by step before answering. Look at the target customers, demand, competition, possible prices, opportunities, challenges, and financial risks.

Format: Start with a short summary and then make a SWOT analysis showing the strengths, weaknesses, opportunities, and threats. Include reasonable price ranges, five things the owner should do to help the business succeed, and a final conclusion. Use simple language, clear headings, and keep it under 700 words. Do not make up exact statistics, and explain any assumptions you make.
```
