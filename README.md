# Radiology AI Publication Skill

LLM skill for writing publication-ready manuscripts for **Radiology: Artificial Intelligence** (RSNA).

## Installation

### Claude (claude.ai)

1. Clone this repository and delete `README.md`
2. Zip all files, rename the zipped folder to `radiology-ai-manuscript-preparation.skill` (not .zip)
3. Go to your Profile (bottom left) → `Settings` → `Capabilities` → scroll down to the `Skills` section → `+ Add`
4. Alternatively, upload the `.skill` file in any Claude conversation and ask it to add this to your skills

### ChatGPT

ChatGPT does not support skills as explicitly as Claude.

**Custom GPT**
1. Explore GPTs → Create
2. Upload all `.md` files to Knowledge
3. Add to Instructions: *"Use the uploaded files to guide manuscript preparation for Radiology: Artificial Intelligence journal"*

**Project**
1. Create a new Project
2. Add the files to the Project Knowledge

**Conversation**
1. Upload the full folder to ChatGPT in a conversation
2. Explain briefly what these files contain and how ChatGPT should use them


## What it does

- Provides article-type-specific templates and limits
- Applies RSNA formatting rules (statistics, terminology, style)
- Enforces **CLAIM 2024** checklist (44 items) with auto-fill guidance

## Usage

1. Add skill to Claude
2. Specify article type: Original Research, Technical Development, AI in Brief, Review, Data Resources, or Letter
3. Claude applies relevant guidance automatically

## Why use this?

This skill helps your paper adhere to RSNA standards, especially for Radiology: Artificial Intelligence. It ensures correct formatting, word counts, and narrative structure, improving your chances of acceptance. It's a tool designed to help you write a better paper.

## Structure
```
├── SKILL.md              # Universal rules + workflow
├── CLAIM.md              # 44-item checklist, condensed
└── article-types/        # Type-specific guidance
    ├── original-research.md
    ├── technical-development.md
    ├── ai-in-brief.md
    ├── review.md
    ├── data-resources.md
    └── letter.md
```

## License

MIT
