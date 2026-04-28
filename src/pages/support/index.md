---
title: FAQ & support
description: Find answers to common questions, troubleshooting steps, and how to get help for Adobe for creativity in Claude.
---

# FAQ & support

Find answers to common questions, fix common issues, and learn how to get help when you're stuck.

## Frequently asked questions

### About Adobe for creativity and Getting Started

<AccordionItem slots="heading, text"/>

#### Do I need an Adobe account to use the Adobe for creativity connector?

No, many Adobe tools are available without signing in. More tools are available when you sign in, including Gen Expand and video tools. A few tools require paid subscription.

<AccordionItem slots="heading, text"/>

#### What can I do with the Adobe for creativity connector?  

Access 50+ tools from across Adobe Creative Cloud suite in one conversation. Use skills for complex, multi-step workflows. Edit and retouch images, design from templates, resize photos and videos, and more  

<AccordionItem slots="heading, text"/>

#### Do I need a paid Claude subscription?

Not for the connector itself — any Claude plan works. A paid Claude plan (Pro, Max, Team, or Enterprise) is required to use Cowork and plugins.

<AccordionItem slots="heading, text"/>

### What's the difference between the connector, skills, and the plugin?

* The connector is the bridge that lets Claude call Adobe's tools.
* Skills teach Claude how to do specific creative workflows well.
* The plugin (Cowork only) bundles the connector, skills, and slash commands together so you can install everything at once.

<AccordionItem slots="heading, text"/>

### Do I need to install the skills separately?

If you don't have Claude paid subscription, and would like to use the skills. You can manually install the skills. In Cowork, installing the Adobe for creativity plugin handles both in one step.

<AccordionItem slots="heading, text"/>

### Can I use this on my phone?

You can run workflows you've already set up, but you can't install new connectors, skills, or plugins from the iOS or Android apps. Set up on web or desktop first.

## Functionality

<AccordionItem slots="heading, text"/>

### What Adobe tools and capabilities does Adobe for creativity in Claude provide?

Access 50+ tools across Photoshop, Lightroom, Illustrator, Firefly, Premiere, Express, InDesign, and Adobe Stock — all through natural language, without switching apps. 

<AccordionItem slots="heading, text"/>

### Can I open and edit an existing layered .psd file?

Partial support. Some operations work on layered files; others will output a flattened result. [Confirm specifics with product team.]

<AccordionItem slots="heading, text"/>

### Can I export to a specific file format?

Yes — specify it in your prompt. Supported output formats include [placeholder: list common ones — JPEG, PNG, TIFF, SVG, PDF, MP4, etc.].

<AccordionItem slots="heading, text"/>

### Can this run a full Adobe application on my machine?

No. The connector calls Adobe's cloud services and APIs. It doesn't launch or drive the desktop apps directly. (In Cowork, Claude can access local files and coordinate with the Adobe cloud, but it doesn't control your installed Adobe software.)

<AccordionItem slots="heading, text"/>

### Can I use this with my company's Adobe team or enterprise account?

Yes. Sign in with the account that has the entitlements you need. Enterprise admins can also provision the connector org-wide — see Cowork setup.

## Skills

<AccordionItem slots="heading, text"/>

### Which skills should I install?

The Adobe for creativity bundle ships with six skills covering the most common creative workflows: batch photo editing, social variations, designing from a template, quick video cuts, resizing photos and videos, and portrait retouching. We recommend starting with the ones that match the work you do most often. See the full list in the getting started guide.

<AccordionItem slots="heading, text"/>

### Do skills work automatically, or do I invoke them?

Both. Claude loads a skill automatically when it detects a matching task. You can also name a skill in your prompt ("use the portrait retouching skill...") to be explicit.

<AccordionItem slots="heading, text"/>

### Can I build my own skill for my team's workflow?

Yes. Skills are file-based (a SKILL.md plus any supporting files, zipped together) and can be uploaded through Customize → Skills → + → Create skill. See Anthropic's skills documentation for the format.

<AccordionItem slots="heading, text"/>

### Can I share skills with my team?

On Team and Enterprise plans, yes. Individual skills can be shared with colleagues, and owners can provision skills org-wide. In Cowork, entire plugins can be distributed through organizational marketplaces.



### Learn More about Adobe creative agents

<AccordionItem slots="heading, text"/>

#### Is Adobe for creativity connector powered by Adobe’s creative agent? 

Yes, it is powered by Adobe's creative agent, that brings tools across Adobe Creative Cloud, informed by decades of understanding of creative workflows.

<AccordionItem slots="heading, text"/>

#### It looks like many of the same tools available in the Firefly AI Assistant are also accessible through this connector in Claude. What’s the advantage of using the Firefly AI Assistant instead of relying on this connector in Claude?

Both FF AI Assistant and Adobe for creativity bring together tools from across the Adobe creative suite to execute creative workflows.
The FF AI Assistant enables a richer experience with greater visibility and control into how assets evolve at every step of the workflow. 
FF AIA includes a wider variety of creative tools. FF AIA offers generative tools such as text to image and Gen Fill as well as a wide choice of image and video generation models from across the industry. And easy access to assets in the Creative Cloud, smoother transitions to Adobe apps, and saved creative preferences 



## Troubleshooting

Most issues fall into a few categories. Try the fixes below before contacting support.

#### Installation issues

<AccordionItem slots="heading, text"/>

### "I can't find 'Adobe for creativity' in the connectors directory"

Confirm you're on a supported platform. The directory is not browsable on iOS or Android — use claude.ai or Claude Desktop.\<br /\>\<br /\> Make sure your Claude account is signed in.\<br /\>\<br /\> On Team or Enterprise plans, an owner may need to enable connectors for your organization before you can install new ones.

<AccordionItem slots="heading, text"/>

### "Install fails or hangs"

* Check your internet connection.
* Try signing out of Claude and back in, then retry the install.
* Clear your browser cache and reload claude.ai.

<AccordionItem slots="heading, text"/>

### "The Cowork plugin isn't available"

* Plugins require a paid Claude plan (Pro, Max, Team, or Enterprise).
* Cowork is desktop-only — you need Claude Desktop on macOS or Windows.
* On organization plans, confirm with your admin that Cowork and Skills are both enabled.

#### Authentication issues

<AccordionItem slots="heading, text"/>

### "I'm signed in to Adobe but tools are limited to guest mode"

* Go to Customize → Connectors → Adobe for creativity.
* Click Disconnect, then Connect again.
* Complete the Adobe sign-in flow, paying attention to which account you pick if you have multiple.
* Start a new chat and try again.

<AccordionItem slots="heading, text"/>

### "It's asking me to reauthenticate every session"

This can happen if your Adobe session cookies are blocked. Make sure third-party cookies are allowed for claude.ai and adobe.com, or try a different supported browser.

<AccordionItem slots="heading, text"/>

### "It says my Adobe account doesn't have access to a feature"

* Firefly generations, Stock licensing, and some cloud features require a paid Adobe subscription with the right entitlement.
* For enterprise accounts, your admin controls which Adobe services are enabled.

#### Skills and tools issues

<AccordionItem slots="heading, text"/>

### "The connector says it's installed but I don't see Adobe tools in my chat"

* Make sure the connector is enabled for this conversation: click + in the lower-left of the chat, hover over Connectors, and toggle Adobe for creativity on.
* Confirm Code execution and file creation is enabled in your Claude settings.

<AccordionItem slots="heading, text"/>

### "Claude isn't using the skill I installed"

* Confirm the skill is toggled on under Customize → Skills.
* Confirm Code execution and file creation is enabled:
  * Free, Pro, Max: Settings → Capabilities.
  * Team, Enterprise: an owner must enable this at the organization level.
* Name the skill explicitly in your prompt: "Use the portrait retouching skill on these photos."

<AccordionItem slots="heading, text"/>

### "Claude is trying to use the wrong tool"

Be more specific about outcome and constraints. "Give me a 9:16 version of this video at 1080p with captions" is far more reliable than "resize this for social."

<AccordionItem slots="heading, text"/>

### "A tool I expected isn't available"

Not every Adobe capability is exposed yet. See known limitations. If a specific tool is missing, let us know — [link to feedback form].

#### Output quality issues

<AccordionItem slots="heading, text"/>

### "The generated result doesn't match what I asked for"

* Attach reference images or past work showing the style you want.
* Specify dimensions, file type, color palette, mood, and platform.
* Iterate: "closer — but make it warmer and remove the text at the bottom."

<AccordionItem slots="heading, text"/>

### "The output is lower resolution than expected"

* Source resolution matters. Attach the highest-resolution file you have.
* Explicitly request dimensions: "export at 4000px on the long edge."
* Some operations produce derived outputs that are lower resolution than the source — check the known limitations.

<AccordionItem slots="heading, text"/>

### "Colors look different from my original"

* Your display's color profile may differ from the profile Claude's output uses. Request a specific color space: "export in sRGB" or "export in Adobe RGB."
* Use Lightroom color correction tools in the prompt to lock down white balance and tone.

#### File and upload issues

<AccordionItem slots="heading, text"/>

### "My file is too large to upload"

There are size limits on both Claude and Adobe sides. If you hit one:\<br /\>\<br /\> - Compress the source if appropriate (for example, ship a TIFF as a high-quality JPEG).\<br /\> - In Cowork, reference the file by path instead of uploading it directly.

<AccordionItem slots="heading, text"/>

### "The final file didn't save to my Creative Cloud folder"

* Confirm you're signed in to Adobe.
* Check your Adobe storage quota — if you're at your storage cap, saves will fail silently.
* Ask Claude where the file was saved: "Where did that export go?"

<AccordionItem slots="heading, text"/>

### Still stuck?

* Browse community discussions at [link to forum or community].
* Contact Adobe support: [link] for Adobe account, Firefly credits, Stock licensing, and Creative Cloud storage issues.
* Contact Claude support: support.claude.com for Claude account, connector installation, and billing issues.
* Report a bug or request a feature: [link to feedback form]

## Give feedback

If something isn't working or you have an idea, we want to hear it. [Embed feedback form or link.]

Was this page helpful? 👍 👎
