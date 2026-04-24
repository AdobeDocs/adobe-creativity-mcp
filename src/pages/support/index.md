# FAQ & support

Find answers to common questions, fix common issues, and learn how to get help when you're stuck.

**Jump to:**

* [Frequently asked questions](https://file+.vscode-resource.vscode-cdn.net/Users/sarahxu/Downloads/files%202/04-faq-and-support.md#frequently-asked-questions)
* [Troubleshooting](https://file+.vscode-resource.vscode-cdn.net/Users/sarahxu/Downloads/files%202/04-faq-and-support.md#troubleshooting)
* [Still stuck?](https://file+.vscode-resource.vscode-cdn.net/Users/sarahxu/Downloads/files%202/04-faq-and-support.md#still-stuck)

## Frequently asked questions

[Placeholder note: review every answer below with Adobe legal/product before publishing — especially pricing, data handling, and credits.]

## Getting started

**Do I need an Adobe account to use this?** No — you can use the connector as a guest with a limited set of tools. Signing in with an Adobe account unlocks more tools, persistent storage, and full Firefly and Stock capabilities. See access tiers.

**Do I need a paid Claude subscription?** Not for the connector itself — any Claude plan works. A paid Claude plan (Pro, Max, Team, or Enterprise) is required to use Cowork and plugins.

**What's the difference between the connector, skills, and the plugin?**

* The connector is the bridge that lets Claude call Adobe's tools.
* Skills teach Claude how to do specific creative workflows well.
* The plugin (Cowork only) bundles the connector, skills, and slash commands together so you can install everything at once.

**Do I need to install the skills separately?** In Claude chat and Claude Desktop, yes — install the connector first, then browse the skills directory for Adobe-tagged skills. In Cowork, installing the Adobe for creativity plugin handles both in one step.

**Can I use this on my phone?** You can run workflows you've already set up, but you can't install new connectors, skills, or plugins from the iOS or Android apps. Set up on web or desktop first.

## Pricing and limits

**How much does this cost?** The Adobe for creativity connector is [placeholder: free / included with X / priced at Y]. Your usage may be limited by:

* Your Claude plan's message and tool-call limits
* Your Adobe plan's generative credits (for Firefly) and Stock licensing allowance

**Does using Firefly here consume my Firefly generative credits?** If you're signed in to a paid Adobe account, generations count against your plan's credits. [Confirm exact behavior with Adobe.]

**Does licensing a Stock asset here charge my Stock subscription?** Yes — licensing flows through your own Adobe Stock subscription. You must be signed in to a paid Stock plan for full licensing. Guest and free users can preview but not license.

**Are there rate limits?** Claude has per-plan usage limits. The Adobe APIs behind the connector may also have their own rate limits on high-volume operations. If you hit one, Claude will let you know and you can retry after a short wait.

## Privacy and data

**Are my uploads used to train AI models?** [Placeholder — this is the most important question to answer clearly and correctly. Work with Adobe and Anthropic privacy teams to write this. Cover: Anthropic's training policy, Adobe's training policy for files processed through Firefly, and anything different about Stock searches.]

**Where are my files stored?**

* Guest users: Files exist only for the current session and are not persisted.
* Signed-in users: Assets are saved to your Adobe Creative Cloud Files (or the relevant Adobe storage for the tool used). Claude does not maintain a separate copy.
* Chat transcripts: Stored by Claude per your account settings.

**Who can see my work?** Only you, unless you explicitly share it. Connector permissions follow your Adobe account permissions.

**Can I delete my data?** Yes. Remove files from Creative Cloud through Adobe, and clear Claude chats from Claude. [Link to Adobe's data deletion and Anthropic's data deletion docs.]

## Functionality

**What Adobe apps does this cover?** Photoshop, Lightroom, Illustrator, Firefly, Premiere, Express, InDesign, and Adobe Stock. Not every feature of every app is exposed — see known limitations.

**Can I open and edit an existing layered .psd file?** Partial support. Some operations work on layered files; others will output a flattened result. [Confirm specifics with product team.]

**Can I export to a specific file format?** Yes — specify it in your prompt. Supported output formats include [placeholder: list common ones — JPEG, PNG, TIFF, SVG, PDF, MP4, etc.].

**Can this run a full Adobe application on my machine?** No. The connector calls Adobe's cloud services and APIs. It doesn't launch or drive the desktop apps directly. (In Cowork, Claude can access local files and coordinate with the Adobe cloud, but it doesn't control your installed Adobe software.)

**Can I use this with my company's Adobe team or enterprise account?** Yes. Sign in with the account that has the entitlements you need. Enterprise admins can also provision the connector org-wide — see Cowork setup.

## Skills

**Which skills should I install?** The Adobe for creativity bundle ships with six skills covering the most common creative workflows: batch photo editing, social variations, designing from a template, quick video cuts, resizing photos and videos, and portrait retouching. We recommend starting with the ones that match the work you do most often. See the full list in the getting started guide.

**Do skills work automatically, or do I invoke them?** Both. Claude loads a skill automatically when it detects a matching task. You can also name a skill in your prompt ("use the portrait retouching skill...") to be explicit.

**Can I build my own skill for my team's workflow?** Yes. Skills are file-based (a SKILL.md plus any supporting files, zipped together) and can be uploaded through Customize → Skills → + → Create skill. See Anthropic's skills documentation for the format.

**Can I share skills with my team?** On Team and Enterprise plans, yes. Individual skills can be shared with colleagues, and owners can provision skills org-wide. In Cowork, entire plugins can be distributed through organizational marketplaces.

## Troubleshooting

Most issues fall into a few categories. Try the fixes below before contacting support.

### Installation issues

**"I can't find 'Adobe for creativity' in the connectors directory"**

* Confirm you're on a supported platform. The directory is not browsable on iOS or Android — use claude.ai or Claude Desktop.
* Make sure your Claude account is signed in.
* On Team or Enterprise plans, an owner may need to enable connectors for your organization before you can install new ones.

**"Install fails or hangs"**

* Check your internet connection.
* Try signing out of Claude and back in, then retry the install.
* Clear your browser cache and reload claude.ai.

**"The Cowork plugin isn't available"**

* Plugins require a paid Claude plan (Pro, Max, Team, or Enterprise).
* Cowork is desktop-only — you need Claude Desktop on macOS or Windows.
* On organization plans, confirm with your admin that Cowork and Skills are both enabled.

### Authentication issues

**"I'm signed in to Adobe but tools are limited to guest mode"**

1. Go to Customize → Connectors → Adobe for creativity.
2. Click Disconnect, then Connect again.
3. Complete the Adobe sign-in flow, paying attention to which account you pick if you have multiple.
4. Start a new chat and try again.

**"It's asking me to reauthenticate every session" This can happen if your Adobe session cookies are blocked. Make sure third-party cookies are allowed for claude.ai and adobe.com, or try a different supported browser.**

**"It says my Adobe account doesn't have access to a feature"**

* Firefly generations, Stock licensing, and some cloud features require a paid Adobe subscription with the right entitlement.
* For enterprise accounts, your admin controls which Adobe services are enabled.

### Skills and tools issues

**"The connector says it's installed but I don't see Adobe tools in my chat"**

* Make sure the connector is enabled for this conversation: click + in the lower-left of the chat, hover over Connectors, and toggle Adobe for creativity on.
* Confirm Code execution and file creation is enabled in your Claude settings.

**"Claude isn't using the skill I installed"**

* Confirm the skill is toggled on under Customize → Skills.
* Confirm Code execution and file creation is enabled:
  * Free, Pro, Max: Settings → Capabilities.
  * Team, Enterprise: an owner must enable this at the organization level.
* Name the skill explicitly in your prompt: "Use the portrait retouching skill on these photos."

**"Claude is trying to use the wrong tool" Be more specific about outcome and constraints. "Give me a 9:16 version of this video at 1080p with captions" is far more reliable than "resize this for social."**

**"A tool I expected isn't available" Not every Adobe capability is exposed yet. See known limitations. If a specific tool is missing, let us know — [link to feedback form].**

### Output quality issues

**"The generated result doesn't match what I asked for"**

* Attach reference images or past work showing the style you want.
* Specify dimensions, file type, color palette, mood, and platform.
* Iterate: "closer — but make it warmer and remove the text at the bottom."

**"The output is lower resolution than expected"**

* Source resolution matters. Attach the highest-resolution file you have.
* Explicitly request dimensions: "export at 4000px on the long edge."
* Some operations produce derived outputs that are lower resolution than the source — check the known limitations.

**"Colors look different from my original"**

* Your display's color profile may differ from the profile Claude's output uses. Request a specific color space: "export in sRGB" or "export in Adobe RGB."
* Use Lightroom color correction tools in the prompt to lock down white balance and tone.

### File and upload issues

**"My file is too large to upload" There are size limits on both Claude and Adobe sides. If you hit one:**

* Compress the source if appropriate (for example, ship a TIFF as a high-quality JPEG).
* In Cowork, reference the file by path instead of uploading it directly.

**"The final file didn't save to my Creative Cloud folder"**

* Confirm you're signed in to Adobe.
* Check your Adobe storage quota — if you're at your storage cap, saves will fail silently.
* Ask Claude where the file was saved: "Where did that export go?"

### Still stuck?

* Browse community discussions at [link to forum or community].
* Contact Adobe support: [link] for Adobe account, Firefly credits, Stock licensing, and Creative Cloud storage issues.
* Contact Claude support: support.claude.com for Claude account, connector installation, and billing issues.
* Report a bug or request a feature: [link to feedback form]

## Give feedback

If something isn't working or you have an idea, we want to hear it. [Embed feedback form or link.]

Was this page helpful? 👍 👎