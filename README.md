# UX Writing Skill (UX Writing Knowledge Base)

This skill knowledge base is a professional UX Writing guideline specifically developed for **B2B system products, including Enterprise Resource Planning (ERP), Food and Beverage Management (FBM), Central Reservation Systems (CRS), and Property Management Systems (PMS).** It aims to establish brand language consistency across products and languages while minimizing the risk of UI layout breaks during multilingual translations.

These structured Markdown files serve not only as design guidelines but also directly as an **AI shared skill (Skill Set)**, supporting team members in quickly invoking them across different AI tools.

---

## 📁 File Structure & Purpose

### 1. SKILL.md (Main Instruction File)
* **Core Content**: Includes writing principles, error message formulas, empty state guidelines, and i18n technical specifications.
* **Main Purpose**: Acts as the "brain" of the AI, empowering it with the decision-making capabilities of a professional UX Writer to ensure outputs align with a "professional, clear, and supportive" brand voice.

### 2. references/Frameworks.md (Tone Reference File)
* **Core Content**: Defines the consistent brand Voice and the context-dependent Tone Matrix.
* **Main Purpose**: Assists the AI in adjusting its tone based on the user's current emotional state (e.g., task success, operational error, or onboarding).

### 3. references/Terminology.md (Multilingual Terminology Base)
* **Core Content**: Provides standard operational terminology and message templates for markets such as Taiwan, Japan, North America, and Vietnam.
* **Main Purpose**: Ensures consistency across multilingual interfaces and prevents the AI from generating stiff translations that do not conform to industry conventions.

---

## 🚀 Cross-Platform AI Usage

This knowledge base adopts the universal Markdown format, offering high **portability**. Team members simply need to provide the file content to the AI to enable consistent review standards across different models:

### 🔹 Usage in Claude (Projects)
1. Go to Settings -> Capabilities -> Skills -> Add -> **Upload a skill**.
2. Create a new Project.
3. Ask Claude to confirm if the skill was successfully referenced.
4. Claude will automatically follow these guidelines to provide copy recommendations in the conversation.

### 🔹 Usage in ChatGPT (My GPTs)
1. Create a custom GPT.
2. Upload the files to the **Knowledge** section.
3. Specify in the Instructions: "Please prioritize the guidelines in the Knowledge section to review or write UI copy."

### 🔹 Usage via Direct Prompting
1. Directly copy the contents of `SKILL.md` as the start of the conversation (System Prompt) to assign the AI a professional role.
2. Subsequently, input the UI draft and ask the AI to optimize it based on the guidelines.

### 🔹 Writing Prompts
Please execute the UX Writing task based on the provided knowledge base files (SKILL.md, Frameworks.md, Terminology.md).
1. Product Used: {CRS Reservation Center}
2. Scenario: {Onboarding/Task Success/Help Guide/Error Message/Notification/Empty State - Brief Description}
3. Original Copy: {"Reservation failed! Because {{hotel_name}}'s {{room_type}} has an inventory conflict, please adjust the time or date."}
4. Please review according to the checklist, optimize the copy's tone and wording, and provide suggested button copy. Please output both Traditional Chinese and English versions simultaneously.

---

## 🛠️ Future Roadmap (Automation & Tools)
Future updates will add common vocabulary knowledge for various product lines, such as terms for booking, waitlisting, standby, and hotel terms like C/I, C/O, etc.

To make the guidelines easier to integrate into the development workflow, the `scripts/` folder is slated for the development of the following automation tools:

* **Copy Linter**: Automatically detects errors violating `SKILL.md` guidelines, such as "variables in the middle of a sentence" or "half-width punctuation".
* **Figma Terminology Sync**: Converts `Terminology.md` to JSON format for Figma plugins to call upon, enabling one-click switching of multilingual copy.
* **AI Agent Encapsulation**: Combines the knowledge base with automation scripts to achieve automated reviews and cross-system updates (e.g., syncing to Notion or Slack).
* **Multilingual Layout Breakage Prediction**: Based on the language length differences mentioned in UX Writing.md (e.g., English/Vietnamese is usually longer than Chinese), the script can automatically generate a test list simulating long text to pre-determine if buttons or tables will break due to text expansion.

---

## 📝 Quick Checklist

* [ ] **Clear and Concise**: Can the sentence be shorter? Does it solve only one thing?
* [ ] **Action-Oriented**: Is a clear next step provided (button text as verb + object)?
* [ ] **Empathetic**: Do error messages follow the "Acknowledge the Problem + Solution" formula instead of blaming the user?
* [ ] **Variable Guidelines**: Are variables avoided in the middle of sentences to prevent layout breakage during translation (Label: Value)?
* [ ] **Chinese First**: Are English terms like Email or Address mistakenly used in the Chinese interface?
