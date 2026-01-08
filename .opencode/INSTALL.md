# Installing Talk About Us for OpenCode

Add the shareability audit skill to your OpenCode environment.

## Installation

1. **Clone the repository**:
   ```bash
   mkdir -p ~/.config/opencode/skills
   git clone https://github.com/oalders/talk-about-us.git ~/.config/opencode/skills/talk-about-us
   ```

2. **Create a symlink to the skill**:
   ```bash
   ln -sf ~/.config/opencode/skills/talk-about-us/skills/talk-about-us ~/.config/opencode/skills/talk-about-us-skill
   ```

## Usage

Ask OpenCode to audit your content:

```
Review the copy on our homepage for shareability using the talk-about-us skill
```

Or reference it directly:

```
Use the talk-about-us skill to audit this paragraph: "We're passionate about innovation..."
```

## Updating

```bash
cd ~/.config/opencode/skills/talk-about-us
git pull
```

## About

This skill implements [Anil Dash's shareability framework](https://www.anildash.com/2025/12/05/talk-about-us-without-us/) to audit whether your content can be authentically shared by others without you present.

## Attribution

Installation pattern based on [obra/superpowers/.opencode/INSTALL.md](https://github.com/obra/superpowers/blob/main/.opencode/INSTALL.md).
