# Talk About Us for OpenCode

This guide explains how to use the Talk About Us shareability audit skill with [OpenCode](https://opencode.ai).

## Quick Install

Tell OpenCode:

> Fetch and follow instructions from https://raw.githubusercontent.com/oalders/talk-about-us/main/.opencode/INSTALL.md

## Manual Installation

See [.opencode/INSTALL.md](../.opencode/INSTALL.md) for step-by-step instructions.

## What This Skill Does

Talk About Us applies [Anil Dash's shareability framework](https://www.anildash.com/2025/12/05/talk-about-us-without-us/) to audit your content. It runs four tests:

1. **The Absence Test** - Can someone authentically explain this when you're not there?
2. **The Distinctiveness Test** - Does this say what only YOU can say?
3. **The Emotional Resonance Test** - Is this emotionally gripping or comprehensively technical?
4. **The Values-First Test** - Are values embedded in how people naturally discuss this?

## Usage Examples

**Audit local content:**
```
@talk-about-us Review our About page copy for shareability
```

**Audit a URL:**
```
@talk-about-us Audit the content on https://example.com
```

**Quick check:**
```
@talk-about-us Apply the shareability audit to this paragraph: "We leverage innovative solutions..."
```

## Skill Location

After installation, OpenCode discovers the skill at:
```
~/.config/opencode/skills/talk-about-us/SKILL.md
```
OpenCode also supports project skills under `.opencode/skills/<skill-name>/SKILL.md`. See the [OpenCode skills guide](https://opencode.ai/docs/skills).

## Getting Help

- Report issues: https://github.com/oalders/talk-about-us/issues
- Read the full framework: https://github.com/oalders/talk-about-us

## Attribution

Skill format and locations follow the [OpenCode skills guide](https://opencode.ai/docs/skills).
