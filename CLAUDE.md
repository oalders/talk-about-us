# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a multi-platform skill that implements Anil Dash's content shareability framework. It audits website copy, SEO descriptions, and marketing content to ensure others can authentically discuss the work without the author present.

**Core principle:** "They have to be able to talk about us without us." - Anil Dash

**Supported platforms:** Claude Code, Codex, OpenCode

## Development Commands

Run the plugin locally for testing:
```bash
claude --plugin-dir .
```

Install from GitHub marketplace:
```bash
claude plugin marketplace add oalders/talk-about-us
claude plugin install talk-about-us@talk-about-us
```

## Architecture

This is a documentation-only skill with no build system, dependencies, or executable code.

```
skills/
└── talk-about-us/
    └── SKILL.md              # The skill definition and audit framework
.claude-plugin/               # Claude Code plugin metadata
.codex/
└── INSTALL.md                # Codex installation instructions
.opencode/
└── INSTALL.md                # OpenCode installation instructions
docs/
├── README.codex.md           # Codex usage guide
└── README.opencode.md        # OpenCode usage guide
```

**How it works:** The AI assistant loads SKILL.md when users work with content that matches the skill's description. The skill guides the assistant through four tests (Absence, Distinctiveness, Emotional Resonance, Values-First) to audit content shareability.

## Key Files

- `skills/talk-about-us/SKILL.md` - The complete audit framework with tests, examples, and verification steps
- `.claude-plugin/plugin.json` - Plugin version and metadata
- `README.md` - User documentation with installation, usage, and a complete real-world audit example
