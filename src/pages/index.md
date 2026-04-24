---
title: Adobe for Creativity available in Claude 
description: This is the overview page of creativity in Claude
---
<Superhero slots="image, icon, heading, text, buttons" variant="halfWidth" />

![Hero image](./assets/cc.png)

:adobe:

# Adobe for creativity available in Claude

Adobe's professional creative capabilities, directly inside Anthropic's Claude. Create, edit, and design with natural language across Photoshop, Lightroom, Illustrator, Firefly, Premiere, Express, InDesign, and Adobe Stock — all in one conversation. No app switching, no interruptions.

* [Try it in Claude](https://example.com/getting-started)

## What is "Adobe for creativity"?

It's a single Claude connector that bundles creative tools from across the Adobe ecosystem. Ask Claude in natural language to retouch a photo, cut a video, search Adobe Stock, generate with Firefly, or assemble an InDesign layout — and Claude does the work using real Adobe APIs.

Because it's built on the Model Context Protocol (MCP), it works anywhere Claude runs: **Claude chat** (web and mobile), **Claude Desktop** and **Cowork.**

### Connector vs. Skills — what's the difference?

You'll set up two things to get the full experience:

* **The connector** is the bridge between Claude and Adobe's services. Install it once and Claude can call Adobe tools.
* **Skills** are optional add-ons that teach Claude how to use those tools for specific workflows — like a "portrait retouching" skill that knows the right sequence of adjustments, or a "social resize" skill that knows the dimensions for every major platform.

The connector alone gets you a lot. Skills make Claude noticeably better at specific creative tasks.

## Who can use it, and what do they get?

Access scales with your Claude plan and your Adobe sign-in status.

|  | Guest (no Adobe sign-in) | Free Adobe account | Paid Adobe account (Creative Cloud, Firefly, etc.) |
| --- | --- | --- | --- |
| **Tools available** | ~40 standard tools | Expanded tool set (placeholder — confirm exact count) | All available tools |
| **Asset storage** | Session only | Saved to your Creative Cloud Files | Saved to your Creative Cloud Files |
| **Usage limits** | Lower | Higher | Highest |

**How to sign in:** Start a chat with the connector enabled and Claude will prompt you. You can also sign in anytime from Customize → Connectors → Adobe for creativity → Sign in.

## Where you can use it

The Adobe for creativity connector is available in three places:

### 🗨️ Claude chat (web & mobile)

Best for: quick conversational edits, one-off generations, fast iteration on a single asset.

### 🖥️ Cowork (desktop)

Best for: multi-step creative projects, working with local files, combining Adobe with your other tools (Figma, Drive, Slack), and installing plugins that bundle skills together.

### 💻 Claude Desktop

Works the same as Claude chat, with the benefit of local file access.

<InlineAlert slots="text" variant="info" />

Note: New connectors and skills can't be browsed or installed from the iOS or Android apps. Set up on web or desktop first, then use the mobile apps to run the workflows you've installed.

→ [Full setup instructions for every surface](link to the getting started tab)

## What you can do with it

The connector ships with six skills covering the most common creative workflows. Here are example prompts to try:

### Edit and retouch photos

* "Batch edit these photos — even out the exposure, warm up the color, and crop to 4:5."
* "Retouch these three headshots — soften skin without losing texture, brighten eyes, balance tones across all three."

### Design and generate

* "Make an Instagram story for my bakery's weekend sale using a template from my brand library."
* "Create four on-brand variations of this social post — different color palettes, same layout."

### Video

* "Resize this video for YouTube Shorts, Reels, and TikTok."
* "Cut this 2-minute interview into a 30-second highlight reel with fade transitions."

→ [Full prompt library with walkthroughs](link to the prompts and workflows tab)

## Before you start

* A Claude account (Free, Pro, Max, Team, or Enterprise). Some features require a paid Claude plan — see the requirements section on the [getting started page](https://file+.vscode-resource.vscode-cdn.net/Users/sarahxu/Downloads/files%202/02-getting-started.md#technical-requirements).
* An Adobe account is optional but strongly recommended for full functionality.
* Code execution and file creation must be enabled in your Claude settings for skills to work. On Free, Pro, and Max plans this is under Settings → Capabilities. On Team and Enterprise, an owner must enable both Code execution and file creation and Skills at the org level.


## Get help

* Stuck on setup? Have a question? Or want to request a feature? See FAQ & support (link to FAQ tab)
