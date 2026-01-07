# Talk About Us

> "They have to be able to talk about us without us." - Anil Dash

A Claude Code plugin that helps you audit content for shareability using [Anil Dash's framework](https://www.anildash.com/2025/12/05/talk-about-us-without-us/). Ensure your website copy, SEO descriptions, and marketing content are so clear and compelling that others can share them authentically in your absence.

## About This Plugin

**Framework:** Created by [Anil Dash](https://www.anildash.com/) - [read the original article](https://www.anildash.com/2025/12/05/talk-about-us-without-us/)
**Plugin implementation:** [Olaf Alders](https://github.com/oalders)
**Status:** Unofficial implementation - Anil Dash is not affiliated with or responsible for this plugin

This is an independent implementation created to make Anil's shareability framework easily accessible in Claude Code. All credit for the framework and principles goes to Anil Dash. Bug reports and plugin issues should be directed to this repository, not to Anil.

## What This Does

This plugin provides a systematic audit framework for content, applying four critical tests:

1. **The Absence Test** - Can someone authentically explain this when you're not there?
2. **The Distinctiveness Test** - Does this say what only YOU can say?
3. **The Emotional Resonance Test** - Is this emotionally gripping or comprehensively technical?
4. **The Values-First Test** - Are values embedded in how people naturally discuss this?

## Installation

### From GitHub

```bash
# Add the marketplace
claude plugin marketplace add oalders/talk-about-us

# Install the plugin
claude plugin install talk-about-us@oalders
```

### For Development

Clone and test locally:

```bash
git clone https://github.com/oalders/talk-about-us.git
cd talk-about-us
claude --plugin-dir .
```

## Usage

Once installed, the Talk About Us skill becomes available to Claude Code. Claude will automatically invoke this skill when you're:

- Reviewing website copy, About pages, or feature descriptions
- Writing SEO titles and meta descriptions
- Auditing marketing content before publication
- Refining messaging that feels generic or jargon-heavy

### Example

```
You: Review the copy on our homepage for shareability

Claude: [Automatically uses the talk-about-us skill]
I'll audit your homepage copy using Anil Dash's shareability framework...

[Performs the four tests and provides specific feedback]
```

You can also explicitly request it:

```
You: Use the shareability audit on this paragraph: "We're passionate about innovation..."

Claude: [Applies the framework and suggests improvements]
```

## What Makes Content Shareable?

Content passes the shareability test when:

- A community member can naturally explain it without you present
- It's distinctive - not a platitude any competitor could claim
- It leads with emotional resonance, not technical details
- Values are embedded in the natural language people use

### Common Fixes

**Before:**
> "MyProduct is a comprehensive event management IDE that optimizes workflow and leverages cutting-edge technology"

**After:**
> "MyProduct helps race directors focus on what matters—delivering great running events"

## Credits

Framework developed by [Anil Dash](https://www.anildash.com/). Read the original article: [They have to be able to talk about us without us](https://www.anildash.com/2025/12/05/talk-about-us-without-us/) (December 5, 2025)

## License

MIT License - see [LICENSE](LICENSE) file for details.

## Contributing

Found a way to improve the audit framework? Suggestions welcome! Please open an issue or submit a pull request.
