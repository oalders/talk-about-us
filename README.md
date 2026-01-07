# Talk About Us

> "They have to be able to talk about us without us." - Anil Dash

A Claude Code plugin that helps you audit content for shareability using [Anil Dash's framework](https://www.anildash.com/2025/12/05/talk-about-us-without-us/). Ensure your website copy, SEO descriptions, and marketing content are so clear and compelling that others can share them authentically in your absence.

## About This Plugin

- **Framework:** Created by [Anil Dash](https://www.anildash.com/) - [read the original article](https://www.anildash.com/2025/12/05/talk-about-us-without-us/)
- **Plugin implementation:** [Olaf Alders](https://github.com/oalders)
- **Status:** Unofficial implementation - Anil Dash is not affiliated with or responsible for this plugin

This is an independent implementation created to make Anil's shareability framework easily accessible in Claude Code. All credit for the framework and principles goes to Anil Dash. Bug reports and plugin issues should be directed to this repository, not to Anil.

## What This Does

This plugin provides a systematic audit framework for content, applying four critical tests:

1. **The Absence Test** - Can someone authentically explain this when you're not there?
2. **The Distinctiveness Test** - Does this say what only YOU can say?
3. **The Emotional Resonance Test** - Is this emotionally gripping or comprehensively technical?
4. **The Values-First Test** - Are values embedded in how people naturally discuss this?

## Real-World Example

Here's a small snippet of what the audit found when analyzing https://prettygoodping.com, a monitoring service:

**❌ The Absence Test: FAIL**

Current messaging was too technical: "Monitor SSL/TLS & Domain Expiry, Uptime, and Server Ping"

Problem: Heavy jargon that no one would naturally use when recommending the service. It requires technical knowledge to understand and isn't conversational.

**✅ Recommended Fix:**

**Before:**
> "Monitor SSL/TLS & Domain Expiry, Uptime, and Server Ping"
> "PrettyGoodPing [Beta] is a configurable dashboard for web developers"

**After:**
> "Sleep better knowing your sites are being watched"
> "We monitor your SSL certificates, domains, and uptime - and email you before things break. It's pretty good at it."

*[See the complete audit below](#complete-example-audit)*

## Installation

### From GitHub

```bash
# Add the marketplace
claude plugin marketplace add oalders/talk-about-us

# Install the plugin
claude plugin install talk-about-us@talk-about-us
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

The plugin works with both local content and live URLs:

```
You: Use the talk about us test to audit the content on the front page of https://www.prettygoodping.com/

Claude: [Fetches the URL and applies the shareability framework to the page content]
```

## What Makes Content Shareable?

Content passes the shareability test when:

- A community member can naturally explain it without you present
- It's distinctive - not a platitude any competitor could claim
- It leads with emotional resonance, not technical details
- Values are embedded in the natural language people use

## Complete Example Audit

Below is the full audit of PrettyGoodPing's front page, demonstrating all four tests:

---

### Talk About Us Audit: PrettyGoodPing

**Content Summary**

The front page presents PrettyGoodPing as a monitoring dashboard for web developers, focusing on SSL/TLS certificates, domain expiry, server ping, and uptime checks. The messaging is technical and feature-focused.

---

**❌ 1. The Absence Test: FAIL**

"Can someone authentically explain this when I'm not there?"

Current messaging:
- "Monitor SSL/TLS & Domain Expiry, Uptime, and Server Ping"
- "PrettyGoodPing [Beta] is a configurable dashboard for web developers"

Issues:
- Heavy jargon: "TLS/SSL," "domain registrations," "server uptime," "URL availability"
- No one would naturally say this when recommending the service
- Requires technical knowledge to understand what's being offered
- Very formal, not conversational

What someone might actually say: "It's a tool that watches your website stuff and emails you before things break" - but the current copy doesn't enable this kind of natural explanation.

---

**❌ 2. The Distinctiveness Test: FAIL**

"Does this say what only WE can say?"

Generic phrases that any competitor could use:
- "configurable dashboard for web developers"
- The feature list (SSL, domain, ping, uptime) is standard for monitoring tools
- "optional email alerts" - not distinctive

What IS distinctive:
- The name "PrettyGoodPing" has personality (modest, unpretentious)
- Specific limits (25 certs, 5 domains) are concrete
- "Built with Perl" goes against the grain

Problem: The distinctive personality suggested by the name isn't carried into the copy. The messaging could belong to any monitoring service.

---

**❌ 3. The Emotional Resonance Test: FAIL**

"Is this emotionally gripping or comprehensively technical?"

Current approach: Comprehensively technical
- Lists features and limits without explaining why you should care
- No connection to the pain point (expired certs breaking your site, surprise downtime)
- No emotional benefit (peace of mind, sleeping soundly, avoiding embarrassment)
- Missing the "what problem does this solve" narrative

Missed opportunities:
- The anxiety of discovering an expired SSL cert at 3am
- The relief of proactive monitoring
- The embarrassment of users seeing security warnings
- The simplicity of "set it and forget it"

---

**❌ 4. The Values-First Test: FAIL**

"Are values embedded in how people naturally discuss this?"

The name suggests values: "Pretty Good" implies modesty, pragmatism, honesty (not overpromising "amazing" or "ultimate" monitoring)

The copy suggests different values: Technical precision, comprehensiveness, feature completeness

Disconnect: The personality and values aren't woven into the language. There's an opportunity to embrace the "pretty good" ethos - reliable, unpretentious, does what it says on the tin.

---

**Recommendations**

1. **Lead with the problem/emotion, not features**

   ❌ "Monitor SSL/TLS & Domain Expiry, Uptime, and Server Ping"
   ✅ "Never wake up to an expired SSL certificate again"
   ✅ "Your sites are being watched, so you can sleep"

2. **Use natural, shareable language**

   ❌ "configurable dashboard for web developers focused on monitoring TLS/SSL certificates"
   ✅ "A pretty good way to know when your website stuff is about to expire"
   ✅ "We'll email you before your SSL certs, domains, or servers go sideways"

3. **Embrace the personality from your name**

   The "PrettyGoodPing" name is brilliant - modest, honest, approachable. Carry that through:
   - "We're not fancy, but we're reliable"
   - "Does what it says, and does it pretty well"
   - "Simple monitoring that actually works"

4. **Make it repeatable**

   Test: Can someone explain this at a meetup without sounding robotic?

   ❌ Current: "It's a configurable dashboard for monitoring TLS/SSL certificates, domain registrations, server uptime, and URL availability"

   ✅ Better: "It watches your SSL certificates and domains, and emails you before they expire. Pretty straightforward."

5. **Show concrete value, not just features**

   Instead of listing emoji-decorated features, try:
   - "25 SSL certificates watched 24/7"
   - "Email alerts 10 days before disaster strikes"
   - "Because finding out your cert expired from an angry user email is the worst"

---

**Specific Rewrite Suggestions**

Hero Section (current):
> "Monitor SSL/TLS & Domain Expiry, Uptime, and Server Ping"
> "PrettyGoodPing [Beta] is a configurable dashboard for web developers"

Hero Section (suggested):
> "Sleep better knowing your sites are being watched"
> "We monitor your SSL certificates, domains, and uptime - and email you before things break. It's pretty good at it."

Feature Section (current):
> 🔒 TLS/SSL Cert Expiry
> 🌐 Domain Name Expiry

Feature Section (suggested):
> 🔒 Never miss an SSL renewal - We'll bug you 10 days before it expires
> 🌐 Your domain won't disappear - 3 weeks warning before expiry

---

**Summary Score: 0/4 Tests Passed**

The content is technically accurate but fails all four shareability tests. It's jargon-heavy, generic, emotionally flat, and doesn't embody the personality suggested by the excellent brand name.

**Key insight:** You have a distinctive, personable name ("PrettyGoodPing") but corporate, generic copy. Let the personality shine through in the messaging.

---

## Credits

Framework developed by [Anil Dash](https://www.anildash.com/). Read the original article: [They have to be able to talk about us without us](https://www.anildash.com/2025/12/05/talk-about-us-without-us/) (December 5, 2025)

## License

MIT License - see [LICENSE](LICENSE) file for details.

## Contributing

Found a way to improve the audit framework? Suggestions welcome! Please open an issue or submit a pull request.
