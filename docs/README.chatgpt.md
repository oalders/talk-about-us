# Talk About Us for ChatGPT

This guide explains how to use the Talk About Us shareability audit with ChatGPT.

## Option 1: Create a Custom GPT

Create a reusable GPT that has the framework built in.

1. Go to [chat.openai.com/gpts/editor](https://chat.openai.com/gpts/editor)
2. Click "Create a GPT"
3. Configure:
   - **Name:** Talk About Us
   - **Description:** Audit content for shareability using Anil Dash's framework
   - **Instructions:** Copy the entire contents of [SKILL.md](../skills/talk-about-us/SKILL.md)
4. Save and publish (public or link-only)

Now you can start conversations with your GPT and it will apply the framework automatically.

## Option 2: Paste into a Conversation

For one-off audits, paste the framework directly into any ChatGPT conversation.

1. Copy the contents of [SKILL.md](../skills/talk-about-us/SKILL.md)
2. Start a new ChatGPT conversation
3. Paste the framework, then add your request:

```
[Paste SKILL.md contents here]

---

Now audit this content for shareability:

[Your content here]
```

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
