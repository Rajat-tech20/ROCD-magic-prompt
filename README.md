# ✨ Magic Prompt

**Turn rough ideas into clear, structured, copy-ready prompts, using the ROCD framework.**

Magic Prompt is an open-source [Claude Skill](https://docs.claude.com) that helps you write better prompts without starting from a blank page. Describe what you want in your own words, and it organizes your request into a prompt you can paste straight into Claude (or any AI assistant).

---

## Table of Contents

- [The ROCD Framework](#the-rocd-framework)
- [Features](#features)
- [Example](#example)
- [Installation](#installation)
- [Usage](#usage)
- [Prompt Template](#prompt-template)
- [Repository Structure](#repository-structure)
- [Contributing](#contributing)
- [License](#license)

---

## The ROCD Framework

Every strong prompt answers four questions:

| Letter | Element | Question it answers | Example |
|:------:|---------|---------------------|---------|
| **R** | **Role** | Who should the AI act as? | "Act as a beginner-friendly Python tutor." |
| **O** | **Objective** | What should it accomplish? | "Teach me Python through step-by-step lessons." |
| **C** | **Context** | What background, constraints, or preferences matter? | "I have 30 minutes a day and no prior experience." |
| **D** | **Data** | What inputs, examples, or reference material should it use? | "Here is my current code: ..." |

Magic Prompt walks you through these four pieces so nothing important is left out.

## Features

- **Guided prompt building** using the ROCD framework
- **Clarifying questions** when your request is vague or ambiguous
- **Copy-ready output** with clear structure and sensible formatting
- **Prompt improvement**: paste an existing prompt and have it refined
- **Task-aware guidance** with examples for different kinds of work (writing, coding, learning, analysis, and more)
- **Privacy- and safety-minded**: avoids unsupported assumptions and reminds you not to include sensitive data you don't need to share

## Example

**Rough request**

> Help me learn Python.

**Prompt created with Magic Prompt**

> **Role:** Act as a beginner-friendly Python tutor.
>
> **Objective:** Help me learn Python through practical, step-by-step lessons that build gradually from fundamentals.
>
> **Context:** I can study for about 30 minutes per day. Explain concepts in simple language and include short exercises after each lesson.
>
> **Data:** Ask me about my current experience first if it would help personalize the learning path.

> *This is an illustrative example. Your results will depend on the details you provide.*

## Installation

The Skill itself lives in [`SKILL.md`](./SKILL.md).

1. Download or clone this repository.
2. Open `SKILL.md` and review the instructions.
3. Add the Skill using the method supported by your Claude environment (for example, uploading it as a custom Skill).
4. Try it with a rough request, such as *"Use Magic Prompt to help me write a cover letter prompt."*

```bash
git clone https://github.com/<your-username>/magic-prompt.git
```

> **Note:** Supported Skill installation methods can change over time. Check Claude's official documentation for the current steps for your environment.

## Usage

1. **Describe your goal** in your own words. Rough is fine.
2. **Add details** such as audience, tone, constraints, format, or source material.
3. **Let Magic Prompt apply ROCD** and ask follow-up questions if something is unclear.
4. **Review and tweak** the generated prompt before using it.

You can ask Magic Prompt to:

- Create a prompt from scratch
- Improve or tighten a prompt you already have
- Adapt a prompt for a different audience, tone, or output format

## Prompt Template

Use this as a starting point if you prefer to write prompts by hand:

```text
Role: Act as [who/what the AI should be].

Objective: [What you want accomplished, stated clearly.]

Context: [Background, audience, constraints, tone, length, format.]

Data: [Inputs, examples, or reference material to use.]
```

## Repository Structure

```text
magic-prompt/
├── SKILL.md              # The Skill instructions
├── README.md             # Project overview (this file)
├── LICENSE               # License terms
└── tests/
    └── test-cases.md     # Optional: prompt evaluation cases
```

## Contributing

Contributions are welcome. Ways to help:

- Report bugs or confusing behavior by opening an issue
- Suggest new examples or task-specific guidance
- Add test cases to `tests/test-cases.md`
- Improve the documentation

Please open an issue to discuss larger changes before submitting a pull request.

## License

Released under the terms of the [LICENSE](./LICENSE) file in this repository.
