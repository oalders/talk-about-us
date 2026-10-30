# Talk About Us for ChatGPT

This guide explains how to use the Talk About Us shareability audit with ChatGPT.

## Recommended: Paste into a conversation

This works wherever you can use ChatGPT and does not require setting up a GPT:

1. Copy the contents of [SKILL.md](../skills/talk-about-us/SKILL.md).
2. Paste them into a new ChatGPT conversation, followed by your request:

```
[Paste SKILL.md contents here]

---

Now audit this content for shareability:

[Your content here]
```

You can add a short summary of the framework to ChatGPT Custom Instructions if you want it considered across your chats. Custom Instructions are account-level preferences and have character limits, so the full skill text may not fit. See [Custom Instructions](https://help.openai.com/en/articles/8096356-chatgpt-custom-instructions) for current limits and setup.

## Custom GPTs (availability varies)

As of October 2026, new GPT creation is unavailable on personal ChatGPT accounts. Creation and publishing in managed workspaces depend on workspace eligibility, settings, and permissions. OpenAI is also transitioning custom GPT workflows to plugins. Check the current [GPT creation and editing guidance](https://help.openai.com/en/articles/8554397-creating-and-editing-gpts) before using this option.

If your account or workspace still allows GPT creation, open the [GPTs area](https://chatgpt.com/gpts), choose **Create**, and add the contents of [SKILL.md](../skills/talk-about-us/SKILL.md) to the GPT's Instructions. Use Preview to check its responses, then save or share it according to the options available to your workspace. Public or link sharing is optional.

For details on account availability and creating or editing GPTs, see OpenAI's [GPT guide](https://help.openai.com/en/articles/8554397-creating-and-editing-gpts).

## Usage Examples

Once the framework is loaded (via Custom GPT or pasted), ask:

**Audit local content:**
```
Review our About page copy for shareability
```

**Audit a URL:**
```
Audit the content on https://example.com using the shareability framework
```

**Quick check:**
```
Apply the four shareability tests to this paragraph: "We leverage innovative solutions..."
```

## What This Does

The framework applies four tests from [Anil Dash's shareability article](https://www.anildash.com/2025/12/05/talk-about-us-without-us/):

1. **The Absence Test** - Can someone authentically explain this when you're not there?
2. **The Distinctiveness Test** - Does this say what only YOU can say?
3. **The Emotional Resonance Test** - Is this emotionally gripping or comprehensively technical?
4. **The Values-First Test** - Are values embedded in how people naturally discuss this?

## Getting Help

- Report issues: https://github.com/oalders/talk-about-us/issues
- Read the full framework: https://github.com/oalders/talk-about-us
