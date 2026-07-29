# AI Loadout

![AI Loadout - equip Claude Code with the right plug-ins for the mission](assets/hero.webp)

**Gear up Claude Code for the work you actually do.**

Out of the box your AI is a generalist, and you are the one left wiring up tools, repeating the same prompts, and grinding through work a specialist should own.

AI Loadout is the armoury. A growing set of advanced marketing, sales, and automation plug-ins for [Claude Code](https://www.anthropic.com/claude-code) by Julian Dickie, each one built for real work, not demos. Copywriting, email sequences, social content, AI creative, Google Workspace, SEO, ads, and commerce, all driven by natural-language conversation.

Pick the mission. Equip the plug-ins it needs. Ship like you brought a team of specialists.

## What's here

This is a marketplace catalog repo. The actual plugins live in their own repos and are referenced via `marketplace.json`. Adding this one marketplace gives you all of them.

![The AI Loadout kit](assets/kit.webp)

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
| [humanise-copy](https://github.com/juliandickie/humanise-copy) | Voice-preserving removal of AI-generation tells in written content - two-tier detection (trigger phrases plus structural and rhythmic patterns), a zero-dependency Python detector with borderline warnings, a whitelist for brand signature phrases and deliberate technique, checks for the damage a repair pass itself introduces, and a ship or do-not-ship verdict gate. Answer-engine structure routes to claude-seo rather than being repaired. |
| [impeccable](https://github.com/pbakaus/impeccable) | Design fluency for frontend development - one skill with 23 commands (/impeccable polish, audit, critique, distill, animate, and more), a PRODUCT.md and DESIGN.md context flow, and curated anti-pattern knowledge from 60 deterministic detector rules. Third-party by Paul Bakaus; installing from the repo gives the skill form without hooks - the detector CLI, hooks, and browser extension live upstream at impeccable.style. |
| [no-ai-slop](https://github.com/juliandickie/no-ai-slop) | Remove 20+ patterns of AI slop from writing without flattening the writer's voice - binary contrasts, throat-clearing openers, colon reveals, importance puffery, weasel attribution, and more - or detect slop without rewriting. Fork of petergyang/no-ai-slop packaged as a Claude Code plugin, tracking upstream. Complements humanise-copy. |
| [power-design](https://github.com/juliandickie/power-design) | Decks and websites that do not look AI-made - Brand DNA (live URL extraction via Firecrawl or 72+ pre-built brand systems) combined with 20 research-backed slide rules and 20 web rules, each with numeric thresholds. Fork of ItsssssJack/power-design packaged as a Claude Code plugin, tracking upstream. |
| [ui-ux-pro-max](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) | UI/UX design intelligence - searchable offline database of 84 UI styles, 192 colour palettes, 74 font pairings, 25 chart types, and UX guidelines across 22 stacks, plus companion skills for brand, design systems, slides, banner design, and UI styling. Third-party by Next Level Builder. |

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

![Gear up and ship the mission](assets/command.webp)

## Author

Julian Dickie - [github.com/juliandickie](https://github.com/juliandickie)

## License

This catalog (the marketplace.json and README) is MIT licensed. Each plugin has its own license; see the individual plugin repos.
