# Local Business Market Analyzer Template

## Overview

**Purpose:** Creates a customized market analysis for a local service business.

**Structure:** Modified R-T-F Framework (Role, Context, Task, Format)

**Technique:** Zero-shot chain-of-thought prompting

---

## The Prompt

**Role:**
You are a business advisor who is good at helping people understand whether a small business idea could be successful.

**Context:**
I am looking at starting a [BUSINESS_TYPE] in [LOCATION] with a starting budget of [STARTING_BUDGET]. The business would mainly serve [TARGET_CUSTOMERS]. It would offer [SERVICES].

**Task:**
I want you to analyze the market for this business and tell me if it would be a good idea. Think through it step by step before answering. Look at the target customers, demand, competition, possible prices, opportunities, challenges, and financial risks.

**Format:**
Start with a short summary and then make a SWOT analysis showing the strengths, weaknesses, opportunities, and threats. Include reasonable price ranges, five things the owner should do to help the business succeed, and a final conclusion. Use simple language, clear headings, and keep it under 700 words. Do not make up exact statistics, and explain any assumptions you make.

---

## Context and Inputs

- **[BUSINESS_TYPE]:** The kind of local service business being considered (e.g., mobile car detailing).
- **[LOCATION]:** The city or service area where the business would operate (e.g., Bluffdale, Utah).
- **[STARTING_BUDGET]:** The money available to launch the business (e.g., $1,000).
- **[TARGET_CUSTOMERS]:** The main customers the business wants to serve (e.g., busy families and vehicle owners).
- **[SERVICES]:** The main services the business would provide (e.g., interior, exterior, and full detailing packages).

---

## Output Requirements

**Format:** Start with a short summary, then a SWOT analysis, reasonable price ranges, five practical action steps, and a final recommendation. Use clear headings.

**Constraints:** Keep the response under 700 words. Do not invent exact statistics, and identify assumptions.

**Tone and Style:** Use simple language suitable for a new local service-business owner.
