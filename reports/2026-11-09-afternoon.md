# The AI Gazette — Afternoon edition, Monday 9 November 2026

*Models, machines, and matters of consequence*

- Issue: 2026-11-09-afternoon
- Issued: 9 Nov 2026, 16:08 CET (Paris)
- Reporting window: 9 Nov 2026, 06:08 CET to 9 Nov 2026, 16:07 CET
- Timezone: Europe/Paris
- Previous issue: 2026-11-09-morning
- Price: Complimentary

## Editor's note

This Monday afternoon edition covers the ten hours since this morning's 06:08 edition and carries **six stories**: one update and five new. Google added **two new TPU systems** for confidential computing and long-context agent work, Nvidia introduced its GR00T 2 robot model at the Conference on Robot Learning, Disney and Adobe agreed to build custom AI models on Disney's own properties, Meta took its AI age estimation for Instagram worldwide, and Automattic launched Spacefast for hosting what people build with their own AI agents. The update: Nvidia's shares fell sharply as its board investigates Jensen Huang. **No new frontier model from a major lab** passed this journal's checks.

## The News

### Automattic launches Spacefast, a home for sites and apps built with the AI agent you already use

*Coding & agents · New*

**Published:** 9 Nov 2026

WordPress.com owner Automattic launched **Spacefast** on 9 November as a new Automattic company. People keep building in their own AI tool, such as ChatGPT, Claude, Claude Code, Codex or Cursor, and Spacefast supplies hosting, custom domains and a database, then puts the work online behind a private link that a team can comment on.

App authentication, transactional email and shared team knowledge are **coming in the next few weeks**, Automattic said. The service is free to start, with a Go plan at **$5 a month** and a Pro plan at $15 a month per member, and it connects through official plugins for Claude, ChatGPT and others, or through an API, a CLI and an MCP server.

TechCrunch reported that Automattic soft-launched the product in September and that it competes with Lovable and Emergent. Its founder, Batuhan İçöz, told TechCrunch that enterprises face IT sprawl as marketing teams turn out landing pages on such services.

**Analysis — why it matters:** *Analysis: bring-your-own-agent hosting bets that the coding agent becomes something users already pay for elsewhere, and that the business is in where the output runs.*

**Caveat:** Product claims come from Automattic's press release; this journal did not test the service.

**Sources:**

1. [Automattic via PR Newswire](<https://www.prnewswire.com/news-releases/automattic-launches-spacefast-a-new-company-that-gets-apps-and-websites-live-in-seconds-302933038.html>) — primary source. Checked: 9 Nov 2026, 16:07 CET
2. [TechCrunch](<https://techcrunch.com/2026/11/09/automattic-debuts-a-platform-to-deploy-vibe-coding-apps-amid-a-changing-internet>) — reporting. Checked: 9 Nov 2026, 16:05 CET

### Nvidia introduces GR00T 2, an open world action model that teaches robots from human video, at the Conference on Robot Learning

*Research · New*

**Published:** 9 Nov 2026

At the Conference on Robot Learning in Austin, Nvidia on 9 November introduced **GR00T 2**, which it describes as an open frontier world action model built on its Cosmos platform. Its research page says the model predicts future video and robot actions together, and was pretrained on **402,730 hours of egocentric human video**, 10,184 hours of handheld-gripper demonstrations and 23,500 hours of robot teleoperation. Nvidia says 100,000 hours of that human video are openly available on Hugging Face.

Nvidia claims that on 50 tasks never demonstrated on the target robot, GR00T 2 completed 40 at least once without task-specific demonstrations, and that five demonstrations per task raised success to **95% after a 30-minute fine-tune** on a single RTX 5090. A smaller GR00T 2 Turbo runs on the Unitree G1 humanoid itself, at 124 milliseconds per prediction, according to the research page.

Nvidia also announced Isaac Lab 3.0 and new open benchmarks at the conference, and said two of its papers, GRAIL and RoboTTT, are among six finalists for the Best Paper award.

**Analysis — why it matters:** *Analysis: robot data from teleoperation is slow and expensive to collect, so learning manipulation from ordinary human video is the shortcut the field is chasing. If transfer results like these hold up outside Nvidia's labs, data rather than hardware becomes the cheaper lever for robot makers.*

**Caveat:** All results are **Nvidia's own evaluations**, reported in a company whitepaper that has not been peer-reviewed. The blog and the research page describe the zero-shot result differently (40 of 50 tasks completed at least once, against a 40% success rate). This journal did not check the model's licence terms.

**Sources:**

1. [NVIDIA Blog: Practice Makes Precise, at CoRL](<https://blogs.nvidia.com/blog/robotics-simulation-advancements-corl/>) — primary source. Checked: 9 Nov 2026, 16:05 CET
2. [NVIDIA Research: GR00T 2 project page](<https://research.nvidia.com/labs/gear/gr00t-2/>) — primary source. Checked: 9 Nov 2026, 16:06 CET

### Google adds two eighth-generation TPU systems: TPU 8tx for confidential inference and the dual-chip TPU 8i Max for long contexts

*Industry & policy · New*

**Published:** 9 Nov 2026

Google said on 9 November that it has expanded its eighth-generation TPU line with **two new systems, TPU 8tx and TPU 8i Max**, joining the TPU 8t and TPU 8i it introduced in April. It is the first time Google has introduced four TPU systems in one year. In a post by Amin Vahdat, Google said TPUs now have **nearly 100 customers**, including frontier labs, trading firms, retailers and universities.

TPU 8tx uses the same silicon as TPU 8t, paired with AMD CPU hosts, and is aimed at regulated enterprises and governments. Google says it keeps sensitive data and model weights protected and isolated **even while in active use**, and claims up to 2x lower latency than TPU 8t with a near-zero performance penalty. Google pitches it for private fine-tuning, distillation and reinforcement learning on one system.

TPU 8i Max puts **two TPU 8i chips on a single package**. Google says that doubles compute, SRAM and HBM bandwidth over TPU 8i within the same rack footprint, for workloads such as many agents working across a whole codebase or hours of video. Google also said its Cloud Pathways runtime and GKE dynamic slicing are now generally available.

**Analysis — why it matters:** *Analysis: neither system is a new chip. Google is repackaging this year's silicon for two kinds of buyer that Nvidia also courts, regulated customers who need confidential computing and agent builders who run into memory limits, and it did so on a day when Nvidia's shares were falling over the investigation into its chief executive.*

**Caveat:** Latency and density figures are **Google's own claims**, published without test conditions. Google's post gives no availability date, pricing or regions for either system.

**Sources:**

1. [Google: Our newest TPUs, 8tx and 8i Max](<https://blog.google/innovation-and-ai/infrastructure-and-cloud/global-network/tpu-8i-max-and-8tx/>) — primary source. Checked: 9 Nov 2026, 16:05 CET
2. [Google Cloud blog (same post, full text)](<https://cloud.google.com/blog/topics/ai-infrastructure/tpu-8tx-and-tpu-8i-max>) — primary source. Checked: 9 Nov 2026, 16:07 CET

### UPDATE: Nvidia shares fall more than 6% as its board investigates Jensen Huang, and China calls the spy claims unsubstantiated

*Industry & policy · Updated*

**Published:** 9 Nov 2026, 10:05 CET

Update to this morning's edition, which reported that Nvidia's board had opened an independent investigation after reports that Jensen Huang was the target of a foreign intelligence effort, and that Huang had admitted an affair in an email to staff. The new development: on Monday **Nvidia's stock fell more than 6%**, CNBC reported, as investors weighed leadership risk around Huang. IBTimes said the shares had already lost 13% through Friday since the first reports about the relationship.

China's Foreign Ministry spokesperson Guo Jiakun said on Monday that the so-called Chinese spy narrative was **unsubstantiated**, CNBC reported, citing Reuters.

IBTimes also reported that three House committee chairs asked Huang, in a letter dated 4 November, for a closed-door briefing on **18 November** about his interactions with Alice Huang and Nvidia's protections against foreign espionage, and gave him until 11 November to reply. Nvidia has said Huang will keep leading the company during the investigation, according to IBTimes.

**Analysis — why it matters:** *Analysis: the market is now putting a price on a governance question at the company at the centre of AI spending, while rivals such as Google use the moment to push their own chips.*

**Caveat:** The espionage allegations have not been established in any public legal proceeding, and Nvidia's board has said it has no reason to believe national security or company secrets were compromised. The share move was intraday when this edition checked it.

**Sources:**

1. [CNBC](<https://www.cnbc.com/2026/11/09/nvidia-jensen-huang-chinese-spy-investigation.html>) — reporting. Checked: 9 Nov 2026, 16:05 CET
2. [IBTimes](<https://www.ibtimes.com/nvidia-stock-falls-huang-board-investigation-3809545>) — reporting. Checked: 9 Nov 2026, 16:05 CET
3. [Nvidia: Statement from the board of directors (8 November)](<https://nvidianews.nvidia.com/news/statement-from-nvidia-board-of-directors>) — primary source. Checked: 9 Nov 2026, 06:05 CET

### Disney and Adobe agree a multi-year deal to build custom generative AI models trained on Disney's own properties

*Industry & policy · New*

**Published:** 9 Nov 2026

Disney and Adobe announced on 9 November a **multi-year deal** to co-develop custom generative AI models for Disney, Reuters reported. Using **Adobe Firefly Foundry**, which lets companies build and deploy their own models, the two will train models on Disney's intellectual property; the models will be private and proprietary to Disney.

The work starts with Disney's Experiences division, which runs its theme parks, resorts and cruise lines, and with concept exploration at StudioLAB, the innovation hub of Walt Disney Studios. Adobe will also work with ESPN on fan engagement and its content archive. Walt Disney Imagineering has already deployed a custom image model and a **sketch-to-image model** that turns hand-drawn sketches into rendered concept art.

Kyle Laughlin, Disney's senior vice president of R&D technology and engineering, told Reuters the tools cut work that took months to hours and days, and were "in no way meant to replace" roles at Imagineering. Reuters noted a Bloomberg report earlier this month that Disney was considering cutting thousands of jobs.

**Analysis — why it matters:** *Analysis: large rights holders are opting for models trained only on their own catalogues, which sidesteps the copyright fights around general-purpose image models but leaves the question of creative jobs open.*

**Caveat:** Financial terms were not disclosed. Adobe's press release on Business Wire could not be read (HTTP 403 on every route tried), so this story relies on Reuters' report, read through a syndicated copy.

**Sources:**

1. [Reuters, via CNA](<https://www.channelnewsasia.com/business/disney-adobe-co-develop-custom-ai-models-tailored-media-giant-6536291>) — reporting. Checked: 9 Nov 2026, 16:06 CET

### Meta takes its AI age estimation worldwide to move millions more teens into Instagram's Teen Accounts

*Industry & policy · New*

**Published:** 9 Nov 2026

Meta said on 9 November that it is **expanding its AI age-estimation technology globally** to place millions more teens on Instagram into Teen Account protections, even when they gave an adult birthday. Teen Accounts limit who can contact teens, the content they see and their time on the apps.

Meta said it is still rolling the technology out on Facebook and will begin launching similar technology globally on Threads **later this year**. In Australia it has started using **Apple's age-range signal** as an extra method, and parents in the US will see an in-feed video on Instagram this month explaining the approach.

Meta tied the expansion to its commitments under an agreement with 52 bipartisan attorneys general. The Verge reported that the system looks at signals such as the profiles and content a user interacts with and the birthday messages they receive, and that it launched in the US, the EU and Brazil last year.

**Analysis — why it matters:** *Analysis: AI classification is becoming the industry's default answer to age assurance. Meta is also using the announcement to argue for app-store-level age verification, which would shift much of the burden to Apple and Google.*

**Caveat:** Meta did not publish accuracy or error rates, so how many adults are misclassified as teens, or how many teens are missed, is not known.

**Sources:**

1. [Meta: Expanding Teen Account protections to teens around the world](<https://about.fb.com/news/2026/11/expanding-teen-account-protections-to-teens-around-the-world/>) — primary source. Checked: 9 Nov 2026, 16:05 CET
2. [The Verge](<https://www.theverge.com/tech/1029627/meta-instagram-ai-age-assurance-global-expansion>) — reporting. Checked: 9 Nov 2026, 16:06 CET

## Key patterns (editorial analysis)

- The chip contest moved on two fronts in one day: Google added **two TPU systems** while Nvidia's shares fell over the investigation into its chief executive.
- Custom, owned models are spreading beyond tech: Disney will **own models trained on its own characters**, and Nvidia's GR00T 2 trains robots largely on human video.
- Agents are becoming the interface others build around, from Spacefast's **bring-your-own-agent hosting** to Google pitching TPUs for agent workloads.

## Source coverage

- Engine version: 3.31.0
- Engine ran this edition: yes
- Engine look-back: 2 days

### Source status

- reddit: ok, partial (21 threads; 23 sub-requests blocked with HTTP 403, 2 failed with HTTP 422)
- hackernews: ok (25 stories)
- github: ok (15 items)
- devto: ok (12 articles; tags ai and llm)
- youtube: not searched (yt-dlp not available on this machine)
- polymarket: not used: blocked in France (ANJ)
- x: not searched (no consent-free source configured)

### Notes

- The installed last30days engine finished in about two minutes with 73 evidence items from Reddit, Hacker News, dev.to and GitHub. Its top items were general commentary and stories already covered; it surfaced none of this edition's stories. Stories were found with 16 Google News RSS queries, publisher feeds, three post-engine web supplements and the source pages. Item counts are not counts of verified developments.
- No community quotes: the engine returned no relevance-qualified comments on these stories.
- Polymarket not used: blocked in France (ANJ). X not searched. YouTube not searched (not available on this machine). Reddit returned results, but 23 of its sub-requests were blocked (HTTP 403) and two failed (HTTP 422), so Reddit coverage was partial. Missing coverage does not mean nobody discussed these stories.
- Sources not read: Adobe's Business Wire release (HTTP 403) and Reuters' report on a US permitting bill and data centres (HTTP 401). For both, the anti-bot fetch script found no route (direct and Chrome-like requests refused, local stealth Chrome not installed, no Internet Archive snapshot). The Disney and Adobe story is cited through a Reuters syndicated copy; the permitting-bill report was not carried. Bloomberg's reports on Google's TPUs and Deutsche Telekom were not read (paywalled). VentureBeat's feed returned HTTP 429.
- Newsletter leads from the Iris mail bot: today's file still holds the four leads handled this morning, none of them new in this window, so none is carried and the window was not widened.
- Not carried because they fall before this window: OpenAI's GPT-6 Cyber (5 November), Personal Finance in Claude (5 November), Google removing Pro models from its AI Plus plan (announced in October, effective 13 November), Abu Dhabi's work with OpenAI (reported 6 November) and Apiiro's research on secrets saved by Claude Code's permission prompt (8 November).
- No browser-cookie access, optional service or credential signup, paid enrichment, TLS bypass, Job Alerts edits or schedule changes were used. Research logs and full provenance remain private.

### Engine footer (verbatim)

```text
---
✅ All agents reported back!
├─ 🟠 Reddit: 21 threads │ 1,799 upvotes │ 1,137 comments
├─ 🟡 HN: 25 stories │ 1,912 points │ 1,876 comments
├─ 👩‍💻 dev.to: 12 articles │ 103 reactions │ 67 comments
├─ 🐙 GitHub: 15 items │ 55 reactions │ 130 comments
├─ 🗣️ Top voices: r/artificial, r/ClaudeAI, r/singularity
---
```
