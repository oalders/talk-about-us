# Installing Talk About Us for Codex

Add the shareability audit skill to your Codex environment.

## Installation

1. **Clone the repository**:
   ```bash
   mkdir -p ~/.codex/skills/talk-about-us
   git clone https://github.com/oalders/talk-about-us.git ~/.codex/skills/talk-about-us
   ```

2. **Create a symlink to the skill**:
   ```bash
   ln -sf ~/.codex/skills/talk-about-us/skills/talk-about-us ~/.codex/skills/talk-about-us-skill
   ```

## Usage

Ask Codex to audit your content:

```
Review the copy on our homepage for shareability using the talk-about-us skill
```

Or reference it directly:

```
Use the talk-about-us skill to audit this paragraph: "We're passionate about innovation..."
```

## Updating

```bash
cd ~/.codex/skills/talk-about-us
git pull
```

## About

This skill implements [Anil Dash's shareability framework](https://www.anildash.com/2025/12/05/talk-about-us-without-us/) to audit whether your content can be authentically shared by others without you present.

## Attribution

Installation pattern based on [obra/superpowers/.codex/INSTALL.md](https://github.com/obra/superpowers/blob/main/.codex/INSTALL.md).
