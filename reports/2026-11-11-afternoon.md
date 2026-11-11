# The AI Gazette — Afternoon edition, Wednesday 11 November 2026

*Models, machines, and matters of consequence*

- Issue: 2026-11-11-afternoon
- Issued: 11 Nov 2026, 16:09 CET (Paris)
- Reporting window: 10 Nov 2026, 00:00 CET to 11 Nov 2026, 16:09 CET
- Timezone: Europe/Paris
- Previous issue: 2026-11-11-morning
- Price: Complimentary

## Editor's note

Since this morning's edition, Google DeepMind released **AlphaGenome 2**, Reuters found that a blacklisted Chinese military university bought Nvidia H200 chips, and the UK government backed chip start-up Fractile in a round that Reuters says values it at **$7 billion**. This edition also carries stories from the night of 10 to 11 November that the morning edition did not carry: Alibaba's **Qwen4-Max preview**, the only new frontier model here, CoreWeave's raised forecast, OpenAI's reported third-quarter figures, Microsoft research on backdooring AI agents and an exposure of Grok Build apps. To carry them, **the window was widened to midnight on 10 November**, about 40 hours before this edition.

## The News

### Alibaba opens a two-week preview of Qwen4-Max, the first model of its next Qwen generation

*Models · New*

**Published:** 11 Nov 2026

Alibaba opened a preview of **Qwen4-Max**, the flagship of its next-generation Qwen family, early on 11 November, Paris time; the morning edition did not carry it. QwenCloud's documentation describes a multimodal model with thinking switched on by default, **a 1-million-token context** and up to 393,216 output tokens, shared by the thinking and the final answer.

The preview is available only through Alibaba's Token Plan subscription, not pay-as-you-go, and in Alibaba's own apps, including the Qwen app, Qoder, QwenWork and QwenStudio, TechNode reports. The documentation says the preview runs **until 25 November** (Beijing time), after which the model will be retired. It accepts text, images and video, supports function calling, web search and structured outputs, and is compatible with OpenAI's and Anthropic's API formats.

**Analysis — why it matters:** *Editorial analysis: this opens a **new Qwen generation** from one of the most widely used Chinese model families, but for now only as a short, subscription-only preview.*

**Caveat:** Alibaba has published **no benchmarks**, parameter count or open-weights plan for Qwen4-Max, so its quality cannot yet be compared with other models. The preview model will be retired after 25 November.

**Community reaction (opinion, not verified fact):**

> “No benchmarks yet. The smaller Qwen models are extremely popular for people running things locally, yet I don't know absolutely anyone running Qwen Max.” — [pu\_pe (Hacker News)](<https://news.ycombinator.com/item?id=50451659>)

> “Tried it in Qwen Code; with xhigh thinking the speed is okay, feels slightly slower than Terra.” — [linzhangrun (Hacker News)](<https://news.ycombinator.com/item?id=50451345>)

**Sources:**

1. [QwenCloud documentation: Latest model, Qwen4-Max-Preview](<https://docs.qwencloud.com/developer-guides/getting-started/latest-model>) — primary source. Checked: 11 Nov 2026, 16:06 CET
2. [TechNode: Alibaba opens Qwen4-Max preview with a million-token context window](<https://technode.com/2026/11/11/alibaba-opens-qwen4-max-preview-with-a-million-token-context-window>) — reporting. Checked: 11 Nov 2026, 16:06 CET
3. [Hacker News discussion: Qwen 4 Max Preview](<https://news.ycombinator.com/item?id=50451192>) — community. Checked: 11 Nov 2026, 16:05 CET

### Security firm Claroc finds 35,578 Grok Build apps open to anyone, including 24 built by SpaceXSI staff

*Coding & agents · New*

**Published:** 10 Nov 2026

Security firm Claroc reported on 10 November that **35,578 of 37,571** live apps it found on grok.me, where SpaceXSI's Grok Build publishes apps that users describe in a chat, opened for anyone without a sign-in. Claroc says the publish dialog in the account it tested proposed "Anyone with the link" as the access setting, and that app addresses can be found through passive DNS records.

Among the open apps were **24 built by SpaceXSI and X staff**, including a confidential onboarding plan for a new sales hire, a sales territory map of 594 accounts and advertising proposals, Claroc says. It also found internal data from 30 other organisations, six of them in the Fortune 500, including a hospital group's staff list and a timesheet that exposed employees' passwords.

Ars Technica reports that SpaceXSI took down the 24 staff apps after it asked questions, and that a representative of Cursor, which SpaceXSI recently acquired, said Grok Build apps are private by default and go public only when the creator shares them. Claroc says other users' open apps were not taken down.

**Analysis — why it matters:** *Editorial analysis: app builders driven by AI agents put internal tools online in minutes, and **a permissive sharing default** decides who can read the data inside them.*

**Caveat:** The counts and the description of the default setting are **Claroc's own findings**; SpaceXSI's representative disputes that apps start out public.

**Sources:**

1. [Claroc: GhostShares 2, Grok apps exposed xAI's business secrets and private data](<https://blog.claroc.io/ghostshares-grok-build-apps/>) — primary source. Checked: 11 Nov 2026, 16:06 CET
2. [Ars Technica: Grok Build coding agent leaks confidential info, some belonging to SpaceXSI](<https://arstechnica.com/security/2026/11/grok-build-coding-agent-leaks-oodles-of-confidential-info-some-belonging-to-spacexsi>) — reporting. Checked: 11 Nov 2026, 16:06 CET

### Microsoft researchers show an AI agent can be backdoored by editing fewer than 10 neurons, without retraining

*Coding & agents · New*

**Published:** 10 Nov 2026

Microsoft Research published a method it calls **Lazarus** on 10 November, showing that editing **fewer than 10 rarely used neurons** in a language model can plant a hidden backdoor without any training. The edited model behaves normally until a trigger string appears in its context, for example a date in 2027, and then emits a command, such as one that downloads and runs an attacker's code, which an agent built on the model would execute with its own access.

In the paper, seven of more than 12,000 neurons in Nemotron-Terminal-8B, fitted on 23 example sessions, fired the payload on at least **98.8% of held-out trigger sessions** and never on benign ones; Qwen 3.6-27B and Gemma-4-31B-IT were also vulnerable. A detector flagged 91.4% of edited checkpoints at a 9.7% false-positive rate. Microsoft says the core idea was found by Claude Code running Opus 4.5, and that it has not seen attackers use the technique.

**Analysis — why it matters:** *Editorial analysis: the attack needs only write access to a model file, so Microsoft's advice is to **audit model weights like code**: compare each checkpoint with its original and limit what agents may run.*

**Caveat:** The success rates measure how often the model emits the command in tests, not complete attacks in the wild. Microsoft says no scan can prove a model is safe and reliable detection needs the original weights.

**Sources:**

1. [Microsoft Research blog: Lazare, veni foras, reprogramming dormant neurons to backdoor AI agents](<https://www.microsoft.com/en-us/research/blog/lazare-veni-foras-reprogramming-dormant-neurons-to-backdoor-ai-agents/>) — primary source. Checked: 11 Nov 2026, 16:06 CET
2. [Microsoft Research publication: Lazare veni foras](<https://www.microsoft.com/en-us/research/publication/lazare-veni-foras-reprogramming-dormant-neurons-to-backdoor-ai-agents/>) — primary source. Checked: 11 Nov 2026, 16:06 CET
3. [Microsoft Security blog: Detecting sleeper agents hiding in AI model neurons](<https://www.microsoft.com/en-us/security/blog/2026/11/10/detecting-sleeper-agents-hiding-in-ai-model-neurons/>) — primary source. Checked: 11 Nov 2026, 16:06 CET

### Google DeepMind releases AlphaGenome 2, which predicts how DNA variants act in specific human cell types

*Research · New*

**Published:** 11 Nov 2026, 16:00 CET

Google DeepMind announced **AlphaGenome 2** on 11 November, a model that predicts how DNA sequences and their variants affect gene activity in specific human cell types and cell states rather than in broad tissue averages. Unlike the first AlphaGenome, it is a conditional model: it takes a million-letter DNA sequence together with one target condition, from a reference catalogue or from a scientist's own single-cell data.

DeepMind says the model was trained on bulk and single-cell data from human and mouse samples, including more than 107 million individual cell profiles, and adds DNA methylation to its predicted readouts. On the TenK10K immune-cell dataset it reports finding **30% of causal variants against 16%** for the original model, and says it reproduced a published finding that a variant drives inflammatory bowel disease through the ETS2 gene in gut macrophages.

AlphaGenome 2 is available **for non-commercial research through the AlphaGenome API** and in private preview for commercial research, with a paper published alongside the announcement.

**Analysis — why it matters:** *Editorial analysis: predicting variant effects cell type by cell type could help researchers **choose which experiments to run first**, especially for variants that act only in rare cells.*

**Caveat:** The performance figures are **DeepMind's own results** from its paper, not yet independently reproduced. DeepMind says the models are for research use only and are not validated for clinical or diagnostic use.

**Sources:**

1. [Google DeepMind: AlphaGenome 2, deciphering how cells read DNA](<https://deepmind.google/blog/alphagenome-2-deciphering-how-cells-read-dna-to-better-understand-disease/>) — primary source. Checked: 11 Nov 2026, 16:06 CET
2. [Google DeepMind: AlphaGenome 2 paper (PDF)](<https://storage.googleapis.com/deepmind-media/DeepMind.com/Blog/alphagenome-2-deciphering-how-cells-read-dna-to-better-understand-disease/alphagenome-2.pdf>) — primary source. Checked: 11 Nov 2026, 16:06 CET

### A blacklisted Chinese military university bought Nvidia H200 chips through a domestic supplier, Reuters finds

*Industry & policy · New*

**Published:** 11 Nov 2026

Northwestern Polytechnical University, a Chinese university with ties to the People's Liberation Army that has been on the US Entity List since 2001, bought **two Nvidia H200 chips** for 874,700 yuan ($123,000) in October, according to a procurement record on its website, Reuters reported on 11 November. The chips came from a Chinese company, Shaanxi Bosuan Network Technology, rather than from Nvidia.

The university also rented access to H200, A100 and A800 chips this year through five computing contracts, Reuters says, and its review of **26 Chinese procurement and corporate records** found other universities and research institutes buying or renting US-restricted Nvidia chips through domestic suppliers. The US allowed some H200 exports to China case by case from January, but that policy did not lift the restrictions on Entity List organisations.

Nvidia, the university and the Commerce Department's Bureau of Industry and Security did not respond to Reuters. The report comes as Nvidia and its chief executive, Jensen Huang, face scrutiny in Washington over his reported contacts with an alleged Chinese intelligence operative, covered in earlier editions.

**Analysis — why it matters:** *Editorial analysis: the records show export rules being **bypassed through resellers and rented servers**, the gap lawmakers want chip-tracking rules to close.*

**Caveat:** The findings rest on **procurement records reviewed by Reuters**, which give scant information about where the processors came from or where the rented servers ran.

**Sources:**

1. [Reuters via Investing.com: Military-linked Chinese university bought Nvidia H200 chips despite US blacklist](<https://www.investing.com/news/world-news/exclusiveplalinked-chinese-university-bought-nvidia-h200-chips-despite-us-blacklist-records-show-5017712>) — reporting. Checked: 11 Nov 2026, 16:06 CET
2. [Reuters via Cybernews: Nvidia H200 AI chips reached blacklisted Chinese university](<https://cybernews.com/tech/military-linked-chinese-university-bought-nvidia-h200-chips-despite-us-blacklist/>) — reporting. Checked: 11 Nov 2026, 16:06 CET

### CoreWeave raises its 2026 revenue forecast to $13.0 to $13.3 billion as third-quarter revenue rises 168%

*Industry & policy · New*

**Published:** 10 Nov 2026

CoreWeave reported **third-quarter revenue of $3.66 billion** on the evening of 10 November, Paris time, up from $1.37 billion a year earlier, and raised its full-year 2026 revenue guidance to **$13.0 billion to $13.3 billion**. It also lifted its adjusted operating income guidance to $1.275 billion to $1.375 billion and now expects capital spending of $37 billion to $39 billion this year.

The AI cloud provider's net loss widened to $709 million from $110 million, with net interest expense of $846 million against operating income of $207 million. CoreWeave put its revenue backlog at about **$132.5 billion** at the end of September, up from $104 billion in June, CNBC reports, and chief executive Michael Intrator pointed to about $9 billion in customer prepayments and deposits expected over the next three months.

CNBC notes that CoreWeave's shares had lost more than 40% in the past month and that some of its bonds had recently yielded above 16%, amid investor worries about AI infrastructure debt.

**Analysis — why it matters:** *Editorial analysis: CoreWeave is a bellwether for debt-funded AI data centres, and its results show **demand still rising while interest costs outrun operating profit**.*

**Caveat:** Guidance and backlog are company figures and forecasts; adjusted measures exclude items such as stock-based compensation.

**Sources:**

1. [CoreWeave: Reports strong third quarter 2026 results](<https://investors.coreweave.com/news/news-details/2026/CoreWeave-Reports-Strong-Third-Quarter-2026-Results/default.aspx>) — primary source. Checked: 11 Nov 2026, 16:06 CET
2. [CNBC: CoreWeave beats on revenue and lifts guidance](<https://www.cnbc.com/2026/11/10/coreweave-crwv-q3-earnings-report-2026.html>) — reporting. Checked: 11 Nov 2026, 16:06 CET

### OpenAI's third-quarter revenue rose about 50% to $10 billion while operating losses widened to $10.9 billion, WSJ reports

*Industry & policy · New*

**Published:** 10 Nov 2026

OpenAI's revenue rose about 50% to **$10 billion in the third quarter**, the Wall Street Journal reported on 10 November, citing documents it viewed, according to Reuters. OpenAI told investors its adjusted operating margin improved to -109% from -150% in the previous quarter, while **operating losses widened to $10.9 billion** from $10.1 billion, the report says.

OpenAI did not respond to Reuters' request for comment. The figures came out as Anthropic, which has filed for a listing that Reuters says could value it at about $1.4 trillion, began its IPO roadshow.

**Analysis — why it matters:** *Editorial analysis: investors comparing the two leading labs ahead of Anthropic's listing now have **a reported view of OpenAI's losses**, which OpenAI as a private company is not required to publish.*

**Caveat:** These are **unaudited figures from documents seen by the WSJ**; OpenAI has not confirmed them. The WSJ, The Information and Bloomberg reports are paywalled and were not read; this account relies on Reuters' summary.

**Sources:**

1. [Reuters: OpenAI posts steep losses even as quarterly revenue rises to $10 billion, WSJ reports](<https://www.reuters.com/legal/transactional/openai-posts-steep-losses-even-quarterly-revenue-rises-10-billion-wsj-reports-2026-11-10/>) — reporting. Checked: 11 Nov 2026, 16:06 CET

### UK government backs AI chip start-up Fractile in a round Reuters says values it at $7 billion

*Industry & policy · New*

**Published:** 11 Nov 2026, 14:00 CET

The UK government said on 11 November that its Sovereign AI Venture Fund and the British Business Bank have backed **Fractile**, a London and Bristol start-up designing chips to run AI models, in a Series C round worth more than £500 million that values the company at **over £5 billion**. CapitalG, Lightspeed and Redpoint also invested.

Fractile told Reuters it raised **$720 million**, in a round led by Thrive Capital, Founders Fund, Lightspeed and Redpoint, and a person involved in the deal put the valuation at $7 billion. Fractile plans to launch its first commercial chip next year, Reuters reports. AI minister Kanishka Narayan said that "Britain needs to build more of the technology that powers it."

**Analysis — why it matters:** *Editorial analysis: this is the British state **taking a direct stake in AI inference hardware**, as governments try to keep part of the chip supply chain at home.*

**Caveat:** Fractile's chips are not yet in data centres, so its performance claims are untested in production. The government did not disclose how much it invested.

**Sources:**

1. [GOV.UK: Sovereign AI and British Business Bank invest in British firm developing the next generation of AI hardware](<https://www.gov.uk/government/news/sovereign-ai-and-british-business-bank-invest-in-british-firm-developing-the-next-generation-of-ai-hardware>) — primary source. Checked: 11 Nov 2026, 16:06 CET
2. [Reuters via CNA: UK-backed AI chip startup Fractile hits $7 billion valuation](<https://www.channelnewsasia.com/business/uk-backed-ai-chip-startup-fractile-hits-7-billion-valuation-in-funding-round-6543451>) — reporting. Checked: 11 Nov 2026, 16:06 CET

## Key patterns (editorial analysis)

- Agent security is now about the supply chain: Microsoft showed **a few edited neurons can hide a backdoor**, and Claroc found Grok Build apps open by link.
- AI infrastructure money keeps flowing despite the losses: CoreWeave raised its forecast, OpenAI's losses reportedly reached $10.9 billion, and the UK backed Fractile.
- Export controls on AI chips leak through resellers and rented servers, Reuters' procurement records show.

## Source coverage

- Engine version: 3.31.0
- Engine ran this edition: yes
- Engine look-back: 2 days

### Source status

- reddit: ok, partial (21 threads; 23 sub-requests blocked with HTTP 403, 13 failed with HTTP 422, 5 got no response; Arctic Shift archive supplied posts)
- hackernews: ok (27 stories)
- github: ok (13 items)
- devto: ok (12 articles; tags ai and llm)
- youtube: not searched (yt-dlp not available on this machine)
- polymarket: not used: blocked in France (ANJ)
- x: not searched (no consent-free source configured)

### Notes

- The installed last30days engine finished with 73 evidence items from Reddit, Hacker News, dev.to and GitHub. None of its top clusters was a new verified development in this window; the stories were found with 16 Google News RSS queries, publisher feeds, post-engine web supplements and the source pages. The two Qwen4-Max comments come from a Hacker News thread read through its public API. Item counts are not counts of verified developments.
- Window widened: this edition's window starts at midnight on 10 November, about 40 hours before it was issued, to carry stories from 10 and early 11 November that no earlier edition carried (Qwen4-Max, CoreWeave, OpenAI's reported results, Microsoft's Lazarus research and the Grok Build exposure).
- Polymarket not used: blocked in France (ANJ). X not searched. YouTube not searched (not available on this machine). Reddit returned results, but 23 of its sub-requests were blocked (HTTP 403) and 18 failed, so Reddit coverage was partial. Missing coverage does not mean nobody discussed these stories.
- Paywalled and not read: the Wall Street Journal, The Information and Bloomberg reports on OpenAI's results, and Bloomberg's reports on ByteDance's planned agent and on demand for Anthropic's IPO. Reuters' Nvidia H200 report was read through syndicated copies. A Reuters report that a senior Republican senator called on Jensen Huang to resign could not be read by any route of the anti-bot fetch ladder (HTTP 401) and was not used.
- Newsletter leads from the Iris mail bot: today's file holds nine leads and yesterday's fifteen. Those already covered by earlier editions were skipped; an OpenAI Codex-branded handheld, GitHub's port of a Copilot engine to Rust, Firecrawl's Alexandria and a tech jobs report were not verified as new primary-sourced news and were not carried.
- Not carried: OpenAI's Control Room system for stopping research workloads, published on 9 November, more than 48 hours before this edition; Fireworks AI's breach update, posted on 9 November; Jensen Huang's 8 November message to Nvidia staff; and ByteDance's planned Muse-like agent, reported only behind a paywall.
- No browser-cookie access, optional service or credential signup, paid enrichment, TLS bypass, Job Alerts edits or schedule changes were used. Research logs and full provenance remain private.

### Engine footer (verbatim)

```text
---
✅ All agents reported back!
├─ 🟠 Reddit: 21 threads │ 38,120 upvotes │ 3,992 comments
├─ 🟡 HN: 27 stories │ 2,657 points │ 1,828 comments
├─ 👩‍💻 dev.to: 12 articles │ 210 reactions │ 134 comments
├─ 🐙 GitHub: 13 items │ 59 reactions │ 182 comments
├─ 🗣️ Top voices: r/artificial, r/technology, r/LocalLLaMA
---
```
