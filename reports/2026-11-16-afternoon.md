# The AI Gazette — Afternoon edition, Monday 16 November 2026

*Models, machines, and matters of consequence*

- Issue: 2026-11-16-afternoon
- Issued: 16 Nov 2026, 16:10 CET (Paris)
- Reporting window: 16 Nov 2026, 06:07 CET to 16 Nov 2026, 16:10 CET
- Timezone: Europe/Paris
- Previous issue: 2026-11-16-morning
- Price: Complimentary

## Editor's note

Ten hours since the morning edition, and no new frontier model; the one model release is Tencent's low-cost **Hy4 flash**. The largest development is in Washington: the Commerce Department issued an interim rule that requires licences for chips and servers in overseas data centres that supply large amounts of compute to Chinese-headquartered companies, and adds **Malaysia, Singapore, Indonesia, Thailand and Brazil** to the licence list. Security work is the other thread: Google's threat group says it found an attack framework that turned security patches into working exploits **with no human in the loop**, and Anthropic is shortening its disclosure deadlines. OpenAI pushed computer-use agents into healthcare, TensorWave signed a 457-megawatt deal to supply OpenAI, and the Fed's Michael Barr warned that AI agents could speed up bank runs. Vendor claims are labelled as such.

## The News

### Tencent releases Hy4 flash, a cheaper model for everyday office tasks that it says costs a twentieth as much per task as Hy4

*Models · New*

**Published:** 16 Nov 2026

Tencent released **Hy4 flash**, the lowest-cost model in its Hy family, twelve days after the full Hy4. It has 224 billion total parameters, including 64 billion 'Engram' parameters, with **12 billion active**, takes text and images and handles up to one million tokens of context.

List prices are about **US$0.07 per million input tokens** and US$0.281 per million output tokens. Tencent says that on WorkIndex, its own benchmark of slide, document and spreadsheet tasks, Hy4 flash costs one-thirteenth as much per task as Hy4 Preview, one-twentieth as much as Hy4 and one-eighth as much as DeepSeek-V4.1-Flash-1017, and that in a blind test by 85 internal WorkBuddy users its satisfaction came close to Claude Haiku 5.5.

The model is available in Tencent Cloud TokenHub, WorkBuddy, Yuanbao, WeCom, QQ and other Tencent products, free in WorkBuddy and at half price on TokenHub until 30 November. Tencent says it plans to **release the weights** and to add the model to OpenRouter, and recommends the full Hy4 for long software-engineering tasks.

**Analysis — why it matters:** *Analysis: like Alibaba's Qwen4-Max this morning, the pitch is cost per task on in-house office benchmarks rather than a lead on public leaderboards; Chinese labs are competing hard on price for routine agent work.*

**Caveat:** Cost and quality comparisons come from Tencent's internal benchmark and internal users, not independent tests. The weights are promised, not yet released.

**Community reaction (opinion, not verified fact):**

> “Every day that passes makes me wonder if I should just use Chinese ai models.” — [ThePumpkinGod](<https://news.ycombinator.com/item?id=50517592>)

> “suprised by how cheap it is” — [amarcheschi](<https://news.ycombinator.com/item?id=50517224>)

**Sources:**

1. [Tencent: Tencent Launches Hy4 flash to Power High-Speed, Cost-Efficient AI Deployment for Everyday Workflows](<https://www.tencent.com/tencent-launches-hy4-flash-to-power-high-speed-cost-efficient-ai-deployment-for-everyday-workflows/>) — primary source. Checked: 16 Nov 2026, 16:07 CET
2. [TechNode: Tencent launches Hy4 flash, cutting AI task costs by 95% in internal tests](<https://technode.com/2026/11/16/tencent-launches-hy4-flash-cutting-ai-task-costs-by-95-in-internal-tests/>) — reporting. Checked: 16 Nov 2026, 16:09 CET
3. [Hacker News discussion](<https://news.ycombinator.com/item?id=50517461>) — community. Checked: 16 Nov 2026, 16:07 CET

### OpenAI opens computer-use agents to healthcare teams, with CVS Health, Cigna, Abridge and Ambience as early users

*Coding & agents · New*

**Published:** 16 Nov 2026, 07:00 CET

OpenAI said its **computer-use agents for healthcare** are available now through the OpenAI API, ChatGPT for Healthcare and ChatGPT for Clinicians. The agents click, type and move between applications such as electronic health records and insurers' portals, for tasks like prior authorisations, referrals, discharge planning and outreach between visits.

On clinician inbox tasks, OpenAI says physicians rated **99% of 325 reviewed tasks** by GPT-6 Astra as clinically safe, and rated its work very or extremely helpful in 93% of 646 assessments. On HealthAdminBench, an administrative benchmark from Stanford researchers, it reports 94.3% of rubric points for GPT-6 Astra and 91.8% for GPT-6 Luna, which it says costs 8.5 cents per task.

OpenAI says CVS Health uses the agents in production for referrals and consults and is **open-sourcing an Agent Kit** built with OpenAI's Agents SDK, that Cigna Healthcare case managers use them to gather information from more than 10 systems, and that Abridge and Ambience are building on them. It says organisations can set approvals, limit agent access and keep audit logs, and that HIPAA workflows need a Business Associate Agreement.

**Analysis — why it matters:** *Analysis: much hospital work runs through systems without good APIs, which is where agents that drive the screen could matter most, and also where an unreviewed click carries the most risk.*

**Caveat:** Safety, helpfulness and benchmark figures are OpenAI's own evaluations, and its demonstration used synthetic patient data; partner results are as described by OpenAI and the partners, not independently audited.

**Sources:**

1. [OpenAI: Advancing computer-use agents for healthcare teams](<https://openai.com/index/advancing-computer-use-for-healthcare-teams>) — primary source. Checked: 16 Nov 2026, 16:03 CET

### Google's threat group says attackers ran an AI framework that turned security patches into working exploits with no human in the loop

*Research · New*

**Published:** 16 Nov 2026

Google Threat Intelligence Group published its quarterly AI threat tracker on Monday. It says that in the past quarter it found threat actors using AI frameworks to **fully automate vulnerability discovery and exploitation** without a human in the loop, for the first time in its reporting.

The evidence is an exposed staging server hosting a multi-agent framework the operators called **exploit\_agent**, which works with several frontier and local models. Google says it compares the code of popular web applications before and after security updates, finds the likely flaw, drafts an exploit and runs it automatically. The server also held data taken from victims and scripts for reconnaissance, brute-forcing and installing webshells; its configuration comments were in Russian, and victim data suggested the operator was targeting **French websites** in media, entertainment and education.

The report also says threat actors are using open-source agentic penetration-testing frameworks such as CAIRN, CyberStrikeAI and PentAGI in live intrusions, and that CAIRN was used against targets including the **US aerospace sector**. It describes 'LLM Mixers', underground storefronts that resell access to AI models through stolen credentials.

**Analysis — why it matters:** *Analysis: if patches can be turned into exploits automatically, the time organisations have to install a fix shrinks further; the report adds that these tools currently trade stealth for speed and leave detectable traces.*

**Caveat:** The findings are Google's own threat-intelligence assessment; the victims, the operator's identity and the scale of the exploit\_agent campaign are not independently confirmed.

**Community reaction (opinion, not verified fact):**

> “What is the future of security if AI was used in tandem with exploits and fooling even other AI models.” — [serk\_official](<https://news.ycombinator.com/item?id=50517833>)

**Sources:**

1. [Google Cloud blog: GTIG AI Threat Tracker: Agentic Threat Activity Crosses a Significant Threshold](<https://cloud.google.com/blog/topics/threat-intelligence/agentic-threat-activity-crosses-a-significant-threshold>) — primary source. Checked: 16 Nov 2026, 16:04 CET
2. [The Register: Google: AI agent turned a security patch into a working exploit with no human help](<https://www.theregister.com/research/2026/11/16/google-ai-agent-turned-a-security-patch-into-a-working-exploit-with-no-human-help/5309926>) — reporting. Checked: 16 Nov 2026, 16:03 CET
3. [Hacker News discussion](<https://news.ycombinator.com/item?id=50517797>) — community. Checked: 16 Nov 2026, 16:07 CET

### US issues a rule requiring licences for overseas data centres that supply large amounts of AI compute to Chinese-headquartered companies

*Industry & policy · New*

**Published:** 16 Nov 2026

The US Commerce Department's Bureau of Industry and Security released an **interim final rule on remote access** to advanced AI chips and servers. Its summary says it sets new restrictions on exports, reexports and in-country transfers to overseas data centres that remotely supply significant volumes of compute to companies headquartered in Macau or in Country Group D:5, which includes China.

The rule makes it an offence to knowingly supply such chips to a data centre anywhere in the world that gives companies headquartered in those places access to **more than 12,000,000 aggregate TPP**, a measure of computing power, either at one site or across linked data centres. TechCrunch puts that at roughly the computing power of about 750 Nvidia H100 or H200 chips. Data centres already providing that service must obtain a licence **within 90 days** of the rule taking effect if they want to continue, and data centres, foreign foundries and chip exporters must check their customers' direct and indirect ownership.

A second part adds a licence requirement for advanced chips sent to **Indonesia, Malaysia, Singapore, Thailand and Brazil**, which the rule describes as countries with a higher-than-normal risk of diversion. According to TechCrunch, the requirement does not apply to chips destined for US-headquartered companies in those countries. Commercial recommender systems, such as those used by online retailers and social media companies, are excluded from the remote-access licence.

The rule also formally rescinds the Biden administration's AI Diffusion Rule of January 2025, including its controls on model weights; the department says that rule was never enforced. BIS says the rule was written by and at the direction of the Treasury Department and the National Security Council. It takes effect on publication in the Federal Register, with 60 days for comments.

**Analysis — why it matters:** *Analysis: until now US controls covered where chips were shipped, not who rented them; this rule reaches the cloud route that Chinese AI developers have used to train on US chips abroad, and it lands days after the Nvidia and Megaspeed affair put that route in the news.*

**Caveat:** The BIS press release is dated 15 November, but the rule document was produced and reported on Monday 16 November; it had not yet been published in the Federal Register when this edition was checked, so its effective date is still open. The 750-chip comparison is TechCrunch's estimate, not the rule's.

**Sources:**

1. [Bureau of Industry and Security: BIS Issues Rule Addressing Remote Access to American Super Intelligence Technology](<https://www.bis.gov/press-release/bis-issues-rule-addressing-remote-access-american-super-intelligence-technology>) — primary source. Checked: 16 Nov 2026, 16:04 CET
2. [Bureau of Industry and Security: interim final rule, Addressing Remote Access to Advanced Semiconductors (PDF)](<https://www.bis.gov/media/documents/rin-0694-ak50.pdf>) — primary source. Checked: 16 Nov 2026, 16:04 CET
3. [TechCrunch: US tightens AI chip export controls to deter Chinese companies from accessing compute remotely](<https://techcrunch.com/2026/11/16/us-tightens-ai-chip-export-controls-to-deter-chinese-companies-from-accessing-compute-remotely/>) — reporting. Checked: 16 Nov 2026, 16:03 CET

### Anthropic shortens the deadline before it discloses vulnerabilities found by Claude from 90 days to 30 for severe bugs

*Industry & policy · New*

**Published:** 16 Nov 2026

Anthropic is shortening the disclosure window in its coordinated vulnerability disclosure policy from 90 days to **30 days for high- and critical-severity issues**, and to 45 days for all other issues. The new timelines apply to vulnerabilities reported on or after **1 January 2027**; reports already in progress keep their deadlines.

It will also escalate to an external vulnerability coordinator after 15 days instead of 30 if a maintainer does not respond, and wait 30 days instead of 45 after a patch before publishing full technical details. The seven-day window for vulnerabilities under active exploitation is unchanged.

Anthropic says it is giving maintainers of high- and critical-severity bugs it reported more than 90 days ago, and that are now past its current deadline, **another 30 days** before it publishes them on its dashboard. It argues that disclosure norms assumed fixes moved at human speed and that independent rediscovery was unlikely, and says it is seeing a higher rate of rediscovery as AI models improve.

**Analysis — why it matters:** *Analysis: Anthropic reports thousands of Claude-found vulnerabilities to open-source projects, so a shorter clock puts more pressure on volunteer maintainers; the company says it will keep sending patches with its reports and agreeing a pace with each project.*

**Sources:**

1. [Anthropic: Updating our coordinated vulnerability disclosure policy timelines](<https://www.anthropic.com/research/coordinated-vulnerability-disclosure-timelines>) — primary source. Checked: 16 Nov 2026, 16:07 CET

### TensorWave signs a six-year deal to supply OpenAI with 457 megawatts of AMD-based computing capacity

*Industry & policy · New*

**Published:** 16 Nov 2026

TensorWave, a cloud provider that runs only AMD chips, said it has signed a **six-year agreement with OpenAI** to deliver 457 megawatts of dedicated AI infrastructure across several US data centre sites, its largest deployment to date.

It will deploy **AMD Instinct MI455X GPUs** in AMD Helios rack-scale systems, with the first capacity expected online in the first half of 2027 and the full deployment by early 2028. TensorWave says it is the first publicly announced 'neocloud' provider supporting the OpenAI and AMD partnership announced in October 2025, and that it has more than 2 gigawatts of long-term data centre capacity secured. No financial terms were given.

**Analysis — why it matters:** *Analysis: it is a concrete piece of OpenAI's 6-gigawatt AMD plan placed with a third-party operator rather than AMD itself, at a time when investors are questioning how the AI build-out is financed.*

**Caveat:** Announced by TensorWave; OpenAI's own statement was not found when this edition was checked.

**Sources:**

1. [TensorWave: TensorWave to Provide OpenAI with 457 Megawatts of AMD-Powered AI Infrastructure](<https://tensorwave.com/blog/tensorwave-to-provide-openai-with-457-megawatts-of-amd-powered-ai-infrastructure>) — primary source. Checked: 16 Nov 2026, 16:07 CET

### Fed governor Michael Barr warns that AI agents could speed up bank runs and says banks already see agents acting in customer accounts

*Industry & policy · New*

**Published:** 16 Nov 2026

Federal Reserve governor Michael Barr, speaking at an AI-in-finance conference in Milan, said AI agents **may accelerate deposit outflows** during stress periods, because they could detect yield differences or stability signals and move funds at high speed, 'potentially accelerating runs that unfold in minutes'.

Barr said **major banks now report finding AI agents** attempting to take actions in retail customer accounts without the bank being able to verify authenticity, consent and alignment with customer instructions. He called for strict authentication, explicit consent for specific actions and technical limits on what agents can do. He also said he understood generative AI is not yet used for autonomous trading at large scale.

The speech follows the Fed's Financial Stability Report of Friday, which this newspaper covered on 14 November and which focused on debt used to finance the AI build-out.

**Analysis — why it matters:** *Analysis: the warning lands the same week as agent payment products such as ChatGPT Wallet; regulators are starting to treat agent-initiated transactions as a stability question, not only a fraud one.*

**Caveat:** These are one governor's views, not a Federal Reserve rule or policy decision.

**Sources:**

1. [Federal Reserve Board: Speech by Governor Barr, Some Potential Financial Stability Implications of Artificial Intelligence](<https://www.federalreserve.gov/newsevents/speech/barr20261116a.htm>) — primary source. Checked: 16 Nov 2026, 16:07 CET

## Key patterns (editorial analysis)

- Washington moved from chips to compute: the remote-access rule targets **rented capacity abroad**, not only shipments.
- AI security work is speeding up on both sides: Google reports exploits built from patches **without a human**, and Anthropic answers with **30-day disclosure deadlines**.
- Agents are moving into regulated work, from hospital portals to bank accounts, and the controls named are approvals, audit logs and consent checks.
- Chinese model releases keep competing on **cost per task**, measured on the vendors' own benchmarks.

## Source coverage

- Engine version: 3.31.0
- Engine ran this edition: yes
- Engine look-back: 2 days

### Source status

- reddit: ok, partial (20 threads; 23 requests blocked with HTTP 403 and 9 archive queries failed with HTTP 422; Arctic Shift archive supplied posts)
- hackernews: ok (30 stories)
- github: ok (13 items)
- devto: ok (12 articles; tags ai and llm)
- youtube: not searched (yt-dlp not available on this machine)
- polymarket: not used: blocked in France (ANJ)
- x: not searched (no consent-free source configured)

### Notes

- The installed last30days engine finished (exit 0) with 75 evidence items from Reddit, Hacker News, dev.to and GitHub; its top clusters were general discussion rather than verified developments. Most stories here were found with 16 Google News RSS queries, publisher feeds, the Hacker News search API, post-engine web supplements and the source pages. Item counts are not counts of verified developments.
- Window: from 06:07 on Monday 16 November, when the morning edition closed, to this edition; it was not widened.
- Polymarket not used: blocked in France (ANJ). X not searched. YouTube not searched (not available on this machine). Reddit returned results, but 23 of its requests were blocked (HTTP 403), so Reddit coverage was partial. VentureBeat's feed answered HTTP 429. Missing coverage does not mean nobody discussed these stories.
- Read through a non-direct route: OpenAI's pages were read through the host's page-extraction tool; its publication time comes from OpenAI's RSS feed. No source needed the anti-bot fetch script.
- Paywalled and not read: The Information's report that OpenAI explored buying Goodfire for at least 5 billion dollars (not carried), and the Wall Street Journal and Bloomberg reports on the campaign to bring back Jensen Huang.
- Newsletter leads from the Iris mail bot: today's file held four leads, all carried or ruled out by the morning edition; no 15:00 additions were present.
- Not carried: Microsoft's preliminary report on last week's Microsoft 365 outage (published on X, read only through The Register), Senator Cantwell's letter on chip sales, the LVMH and King's Trust partnerships with OpenAI, and India's reported draft rules for testing AI models before launch, which no primary source confirmed in time.
- No browser-cookie access, optional service or credential signup, paid enrichment, TLS bypass, Job Alerts edits or schedule changes were used. Research logs and full provenance remain private.

### Engine footer (verbatim)

```text
---
✅ All agents reported back!
├─ 🟠 Reddit: 20 threads │ 26,617 upvotes │ 4,938 comments
├─ 🟡 HN: 30 stories │ 1,579 points │ 854 comments
├─ 👩‍💻 dev.to: 12 articles │ 196 reactions │ 31 comments
├─ 🐙 GitHub: 13 items │ 44 reactions │ 124 comments
├─ 🗣️ Top voices: r/artificial, r/LocalLLaMA, r/singularity
---
```
