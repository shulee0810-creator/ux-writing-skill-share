# Voice, Tone, and Formatting Frameworks

## Brand Voice
Voice is the fixed and unchangeable brand personality:
- **Professional but not cold**: Professional at its core, approachable, not bureaucratic or commanding.
- **Clear and direct**: Reduces the cost of understanding, minimizes fluff.
- **Supportive and solution-oriented**: Provides actionable solutions, reduces anxiety over errors.

## Contextual Tone Matrix
Tone is adjusted based on the user's current state:

| Scenario | Tone Strategy | Guideline Suggestions | Example |
| :--- | :--- | :--- | :--- |
| **Onboarding/Introduction** | Friendly, encouraging | Guide to complete setup, positive statements | Welcome aboard! We'll get you up to speed quickly. |
| **Task Success** | Supportive, positive | Briefly affirm the action, avoid being overly emotional | Settings successfully updated. |
| **Guide/Help** | Clear, patient | Use step-by-step descriptions, avoid abstract explanations | Please select a data source and click "Create". |
| **Notification** | Neutral, informational | Focus on conveying information, do not create tension | Your subscription will renew in 3 days. |
| **Error Message** | Empathetic, reassuring | Provide a solution, strictly avoid blaming | Sorry, the system is temporarily unable to process this. Please try again later. |

## i18n Formatting Guidelines

### 1. Date Formatting
| Region | Format Example | Guideline |
| :--- | :--- | :--- |
| **Taiwan** | 2025/01/01 Mon | Use `/` as a separator, pad MM/DD with zeros |
| **Japan** | 2025/01/01 月曜日 | Order according to local conventions |
| **Vietnam** | 01/01/2025 Thứ Hai | Considered a core guideline for B2B systems |
| **North America** | Mon, 01/01/2025 | Must support Syncfusion standard formatting |
| **China** | 2025-01-01 Mon | |

### 2. Currency Formatting
* **Principles**: Amounts must be **right-aligned** to easily compare digits.
* **Examples**: Taiwan (NT$ 1,000), Japan (¥1,000), Vietnam (1.000 ₫).

### 3. Name Field Structure
* **Taiwan/Japan**: Last Name / First Name (Last name first).
* **North America**: First / Last Name.
* **Vietnam**: FBM systems do not strictly require a three-part name (for efficiency); identity verification systems require the full name.

## Prerequisites for Using Professional Terminology
When the primary users are industry professionals, industry-standard terminology should be prioritized, but must comply with:
1. **Industry-standard**: Not internal company jargon.
2. **Semantic uniqueness**: Only use one term for the same concept.
3. **Consistency**: "Create report" vs. "Add report"—a single verb should be uniformly used.
4. **Copy should use gender-neutral language**: Reduces the risk of cultural misunderstanding and discrimination. For example: Use "User" or "Client" instead of "he/she".
