# Installing Talk About Us for OpenCode

Add the shareability audit skill to your OpenCode environment. OpenCode reads skills from directories containing `SKILL.md`; see the [OpenCode skills guide](https://opencode.ai/docs/skills) for supported locations and format details.

## Installation

Clone the repository next to your other global OpenCode skills, then link the skill directory itself:

```bash
mkdir -p ~/.config/opencode/skills
git clone https://github.com/oalders/talk-about-us.git ~/.config/opencode/skills/talk-about-us-repo
ln -s ~/.config/opencode/skills/talk-about-us-repo/skills/talk-about-us ~/.config/opencode/skills/talk-about-us
```

Alternatively, copy `skills/talk-about-us` into `.opencode/skills/talk-about-us` in a project to make the skill available only in that project.

## Usage

Load the skill explicitly with `@talk-about-us`:

```
@talk-about-us Review the copy on our homepage for shareability
```

Or reference it directly:

```
@talk-about-us Audit this paragraph: "We're passionate about innovation..."
```

Restart OpenCode after installing so it discovers the skill.

## Updating

```bash
cd ~/.config/opencode/skills/talk-about-us-repo
git pull
```

## About

This skill implements [Anil Dash's shareability framework](https://www.anildash.com/2025/12/05/talk-about-us-without-us/) to audit whether your content can be authentically shared by others without you present.

Skill format and locations follow the [OpenCode skills guide](https://opencode.ai/docs/skills).
