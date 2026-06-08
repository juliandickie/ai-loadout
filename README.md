# AI Loadout

![AI Loadout - equip Claude Code with the right plug-ins for the mission](assets/hero.png)

**Gear up Claude Code for the work you actually do.**

Out of the box your AI is a generalist, and you are the one left wiring up tools, repeating the same prompts, and grinding through work a specialist should own.

AI Loadout is the armoury. A growing set of advanced marketing, sales, and automation plug-ins for [Claude Code](https://www.anthropic.com/claude-code) by Julian Dickie, each one built for real work, not demos. Copywriting, email sequences, social content, AI creative, Google Workspace, SEO, ads, and commerce, all driven by natural-language conversation.

Pick the mission. Equip the plug-ins it needs. Ship like you brought a team of specialists.

## What's here

This is a marketplace catalog repo. The actual plugins live in their own repos and are referenced via `marketplace.json`. Adding this one marketplace gives you all of them.

![The AI Loadout kit](assets/kit.jpg)

| Plugin | Description |
|---|---|
| [ac-builder](https://github.com/juliandickie/ac-builder) | Build ActiveCampaign email sequences from markdown via MJML. Rendering, validation, V1 campaign creation, V3 click-action wiring, theme-driven multi-brand workflows. |
| [linkedin-post-studio](https://github.com/juliandickie/linkedin-post-studio) | Profile-driven LinkedIn content - posts, carousels, hooks, polls, video scripts, newsletters, calendars, repurposing. |
| [creators-studio](https://github.com/juliandickie/creators-studio) | AI image and video Creative Director powered by Gemini Nano Banana, Kling v3, VEO 3.1, ElevenLabs, and Lyria. |
| [scribe](https://github.com/juliandickie/scribe-plugin) | Google Workspace orchestration - Gmail, Calendar, Drive, Docs, Sheets, Slides, Contacts, Tasks, Forms, Chat. 14 cross-service workflow commands plus 10 service skills. |
| [spiffy](https://github.com/juliandickie/spiffy-plugin) | Talk to the Spiffy checkout platform - customer lookup, MRR, affiliate, and churn reports, customer notes, one-off promo codes. Works with any Spiffy account. |
| [clickup](https://github.com/juliandickie/clickup-plugin) | Talk to ClickUp - token-disciplined task access, gated single and bulk writes, and a large-job batch runner with deeper API coverage than the stock connector. Works with any ClickUp workspace. |
| [vimeo](https://github.com/juliandickie/vimeo-plugin) | Push Descript exports from Google Drive into your Vimeo library - multi-language captions and subtitles, title and description sync, and a gated source-file replace. Driven by a Google Sheet manifest read through the Scribe plugin. |
| [descript](https://github.com/juliandickie/descript-plugin) | Full programmatic access to the Descript API - import media, Underlord AI agent edits, publish compositions, inspect jobs, and run bulk video pipelines. Node CLI wrapped by skills with an optional MCP shim. Supply your own Descript API token. |
| [stripe](https://github.com/juliandickie/stripe-plugin) | Full multi-account Stripe API access - every endpoint the pinned stripe-node SDK exposes, standalone keys and Stripe Connect. Binary-enforced read, mutating, and destructive safety tier with live-mode arming, read-only multi-account fan-out, and the bundled Stripe CLI for webhooks. Replaces the single-account MCP connector. Supply your own Stripe keys. |
| [epub-for-agents](https://github.com/juliandickie/epub-for-agents) | Convert EPUBs to YAML-headed Markdown with per-chapter byte and line offsets so agents read books token-efficiently. Independent wrapper around prime-radiant-inc/books-for-bots. Requires the Rust toolchain (cargo). |
| [wp-index](https://github.com/juliandickie/wp-index) | Extract and index any WordPress site via its REST API - per-item Markdown, CSV, a JSON archive, and a Claude knowledge-base file. Standard-library Python, zero install, any post type via a flag. Supply your own site URL and optional Application Password. |
| [claude-seo](https://github.com/juliandickie/claude-seo) | Comprehensive SEO analysis and on-page optimisation - local SEO (Google Business Profile, citations, reviews, map pack), technical SEO, Schema.org generation, Core Web Vitals, AI search, sitemaps, and content quality across 25 sub-skills and 18 sub-agents. Fork of AgriciDaniel/claude-seo. |
| [claude-blog](https://github.com/juliandickie/claude-blog) | Full-lifecycle blog content engine - strategy, briefs, SERP-informed outlines, writing, and 100-point quality scoring, dual-optimised for Google rankings and AI citations. Native output for Astro and WordPress, per-client brand and voice profiles, 12 templates, 30 sub-skills. Fork of AgriciDaniel/claude-blog. |
| [pro-marketing-ads](https://github.com/juliandickie/pro-marketing-ads) | Paid advertising audit and AI ad creative generation - 250+ checks across Google, Meta, YouTube, LinkedIn, TikTok, Microsoft, Apple, and Amazon Ads with weighted scoring, 12 industry templates, PPC math, A/B test design, and PDF reports. Ad image generation handed to the creators-studio plugin. Fork of AgriciDaniel/claude-ads. |

## Install

In Claude Code, add the marketplace:

```
/plugin marketplace add juliandickie/ai-loadout
```

Then install any plugin from it:

```
/plugin install <plugin-name>@loadout
```

For example:

```
/plugin install scribe@loadout
```

```
/plugin install spiffy@loadout
```

Each plugin has its own setup (some need OAuth or an API key). Follow the install prompts or the plugin's own README.

![Gear up and ship the mission](assets/command.jpg)

## Author

Julian Dickie - [github.com/juliandickie](https://github.com/juliandickie)

## License

This catalog (the marketplace.json and README) is MIT licensed. Each plugin has its own license; see the individual plugin repos.
