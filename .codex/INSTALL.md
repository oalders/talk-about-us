# Installing Talk About Us for Codex

Codex discovers skills from skill directories containing a `SKILL.md` file. For a user skill, install it under `~/.agents/skills`; `~/.codex/skills` remains supported for compatibility. See the [Codex skills guide](https://developers.openai.com/codex/skills).

## Installation

Clone the repository alongside your other user skills, then link the skill directory itself:

```bash
mkdir -p ~/.agents/skills
git clone https://github.com/oalders/talk-about-us.git ~/.agents/skills/talk-about-us-repo
ln -s ~/.agents/skills/talk-about-us-repo/skills/talk-about-us ~/.agents/skills/talk-about-us
```

If you set `CODEX_HOME` to a custom Codex home and prefer its legacy skill location, replace `~/.agents/skills` above with `"${CODEX_HOME:-$HOME/.codex}/skills"`.

## Usage

Ask Codex to audit your content:

```
Review the copy on our homepage for shareability using the talk-about-us skill
```

Or reference it directly:

```
Use the talk-about-us skill to audit this paragraph: "We're passionate about innovation..."
```

Restart Codex after installing so it discovers the new skill. The skill can then be invoked by asking Codex to use `talk-about-us`.

## Updating

```bash
cd ~/.agents/skills/talk-about-us-repo
git pull
```

## About

This skill implements [Anil Dash's shareability framework](https://www.anildash.com/2025/12/05/talk-about-us-without-us/) to audit whether your content can be authentically shared by others without you present.

## Attribution

The skill format follows the [Agent Skills specification](https://agentskills.io/specification); Codex discovery and locations are documented in the [Codex skills guide](https://developers.openai.com/codex/skills).
