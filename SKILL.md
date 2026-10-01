---
name: ux-writing-specialist
description: A UX Writing guideline specifically designed for B2B systems. Suitable for reviewing and optimizing UI copy, with a particular focus on multilingual (i18n) practices for hotels, food & beverage, financial prompts, and onboarding empty states. Ensures copy aligns with a professional, clear, and supportive brand voice.
---

# UX Writing Implementation Guide

## Core Writing Principles
Before writing any interface copy, the following baselines must be met:
- **Clear and Direct**: Prioritize easy-to-understand sentences, reducing fluff and vague adjectives.
- **Action-Oriented**: Ensure users can keep moving forward even in blocking scenarios by clearly providing the next actionable step.
- **Keep it Concise**: Retain only necessary information in each sentence. Each sentence should only solve one thing.
- **Empathy First**: Help users reduce anxiety and quickly return to their task flow. Acknowledge the problem state first, provide actionable advice, and strictly avoid blaming the user.
- **Primary Language First**: Chinese interfaces must use Chinese terminology and not mix in English (e.g., use "電子郵件" instead of "Email").
- **Always Use Arabic Numerals for Numbers**:
   * **Do**: You have **3** messages
   * **Don't**: You have **three** messages

## Standard Error Message Formula
When writing error messages, please follow this structure to reduce anxiety and guide recovery:

**Formula: [Acknowledge the Problem] + [Explain the Reason (if necessary)] + [Provide a Solution/Next Step]**

* **Do**: "There is a system issue, please try again later."
* **Do**: "{Account} has not been filled in, please fill it in and try again."
* **Don't**: "Incomplete data." (Lacks a solution)
* **Don't**: "500 Internal Error." (Too technical)

## Empty States Guidelines
Empty states are opportunities to guide the user to start a task, rather than just informing them of a lack of data.

**Formula: [Title: Describe the State] + [Description: Explain the Benefit/Reason] + [CTA: Guide to Start]**

* **Example**:
    * **Title**: No reports created yet
    * **Description**: Create your first report to track your sales data.
    * **CTA**: [Create Report]

## Notification Modal Buttons
When a modal is only used for **notifying information, informing about system states/permission limits**, or **explaining unchangeable situations**, and does not involve user decision-making or execution actions:

- **Button Text**: Uniformly use **"Got it"** (知道了).
- **Principles**:
    - **Do Not Use**: Neutral or action words like "Confirm", "OK", or "Close".
    - **Single Function**: Acts solely as a closing action after the user has finished reading.
- **Judging Criteria**:
    - If the message is "informational" (e.g., system announcements, permission limit explanations), use "Got it".
    - If it involves "data modification" or "decision confirmation" (e.g., deleting data, submitting applications), an action-oriented button must be used (e.g., "Confirm Deletion").

### Differences Between System Toasts and Modals
- **Toast**: Low-interruption, disappears automatically. Used for real-time operational feedback (e.g., "Saved successfully"). Usually has no buttons.
- **Notification Modal**: High-interruption, requires active clicking. Used for critical information that the user must be aware of. Uniformly use "Got it".

## B2B System & Multilingual (i18n) Practices
- **Avoid In-Sentence Variables**: Different languages have different word orders. Please use a `Label: Value` structure instead (e.g., "Total tables: {{n}}" instead of "A total of {{n}} tables").
- **No Compound Variables**: A sentence must not contain more than one semantic variable to avoid translation conflicts.
- **iPad POS Specific Grammar**:
    * **Question Structure**: Should + V. + O.? (Example: "Should we reprint the receipt?")
    * **Button Structure**: Positive actions are on the right (maintain verbs), reverse/negative actions on the left (cancel).
- **Concrete Vocabulary**: Use "Save", "Update", "Delete", and avoid vague terms like "Process", "Operate", "Some", or "Looks like".

## Language Checklist
- [ ] Is it clear and free of ambiguous meanings?
- [ ] Is the sentence as short as possible?
- [ ] Is the next action provided?
- [ ] Is there any blaming tone?
- [ ] Does it comply with the Primary Language First principle (no mixing of English)?
- [ ] Are variables structured to prevent UI layout breaks during translation?
- [ ] Button semantic check: If it is purely informational (involving no decisions), is the button uniformly set to "Got it"?
- [ ] Component selection check: Does this message require high interruption? If not, should it be changed to a low-interruption Toast?

## Resources
When you need more specific advice on tone adjustments:

1. **references/Frameworks.md** - Use this document to adjust the tone based on the context (user's emotional state, product type, brand voice), or to understand how to adjust language for different situations and emotional states.
2. **references/Terminology.md** - Refer to this glossary when you need multilingual copy translation, or need to ensure interface buttons and state labels match the consistent terminology for markets like Taiwan, Japan, North America, Vietnam, and China.
