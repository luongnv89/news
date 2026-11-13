# The AI Gazette — Afternoon edition, Friday 13 November 2026

*Models, machines, and matters of consequence*

- Issue: 2026-11-13-afternoon
- Issued: 13 Nov 2026, 16:08 CET (Paris)
- Reporting window: 13 Nov 2026, 06:10 CET to 13 Nov 2026, 16:08 CET
- Timezone: Europe/Paris
- Previous issue: 2026-11-13-morning
- Price: Complimentary

## Editor's note

Since this morning's edition, the Nvidia affair moved deeper into documents and Congress: Bloomberg traced **banned Nvidia servers to a Shanghai data centre** linked to Alice Huang, a Reuters review counted **more than $3 billion** of Chinese projects built around restricted Nvidia chips, and Commerce Secretary Howard Lutnick agreed to testify to the Senate Banking Committee on **10 December**. The US Department of War renamed its AI office the **Super Intelligence Office**, llama.cpp reached version 1.0, Reuters reported an Amazon plan to gather data on nearly every product sold anywhere, Claude suffered two outages, and EU leaders held their first summit devoted to AI. There is no new frontier model in this window.

## The News

### llama.cpp reaches version 1.0.0 and promises semantic versioning for its local-inference libraries

*Coding & agents · New*

**Published:** 13 Nov 2026, 11:20 CET

The ggml-org project released **llama.cpp v1.0.0** and ggml v1.0.0 on 13 November. In a Hugging Face blog post, the maintainers say both libraries now follow semantic versioning, so **breaking changes to the public C API** will bring a major-version bump.

The release notes say v1.0.0 removes 35 deprecated functions, adds FP8 key-value caches and a host-memory cache for mixture-of-experts weights, and adds support for new models including Kimi-K3.1-Pro. It also hardens llama-server against SSRF, CORS and DNS-rebinding attacks and adds an OpenAI-compatible speech endpoint.

**Analysis — why it matters:** *Analysis: llama.cpp sits underneath many local AI apps; a **stable, versioned API** makes it safer for them to build on and to upgrade.*

**Caveat:** Developers upgrading from earlier builds must adapt to the **removed deprecated functions**. Performance gains are the project's own description, not independently measured here.

**Sources:**

1. [GitHub: llama.cpp release v1.0.0](<https://github.com/ggml-org/llama.cpp/releases/tag/v1.0.0>) — primary source. Checked: 13 Nov 2026, 16:06 CET
2. [Hugging Face blog: llama.cpp v1.0.0, a stronger foundation for the local AI ecosystem](<https://huggingface.co/blog/ggml-org/llama-cpp-v1>) — primary source. Checked: 13 Nov 2026, 16:06 CET

### Claude goes down twice in a day: a login failure, then errors across claude.ai, the API and Claude Code

*Coding & agents · New*

**Published:** 13 Nov 2026, 10:58 CET

Anthropic's status page shows two major incidents on 13 November. At **10:58 Paris time** it began investigating problems with users authenticating to claude.ai and Claude Code; a fix was deployed at 12:05 and the incident was marked resolved at 12:58.

At **14:09** a second incident opened for degraded performance on claude.ai, the Claude API and Claude Code, later widened to connectors including Claude Docs and Claude Sheets. At 15:36 Anthropic reported recovery on claude.ai and the API but said errors could return and that connectors and Claude in Meetings remained degraded. A separate incident affecting the Microsoft 365 connector, opened on 12 November during Microsoft's global outage, was still unresolved.

On Hacker News, users weighed the cost of the morning outage. "Depending on what your job is, this is either the adult equivalent of a snow day or some of the greatest stress in a long time," wrote Topfi. Another user, cmiles8, observed that in an outage this big the severity "almost drops, since everyone is impacted and thus just shrugs their shoulders."

**Analysis — why it matters:** *Analysis: as teams route daily coding and office work through one assistant, its outages stop work, not only chats.*

**Caveat:** Anthropic has not published a cause; the second incident was **still open when this edition was issued**. Hacker News comments are anecdotal.

**Community reaction (opinion, not verified fact):**

> “Depending on what your job is, this is either the adult equivalent of a snow day or some of the greatest stress in a long time.” — [Topfi (Hacker News)](<https://news.ycombinator.com/item?id=50481273>)

> “since everyone is impacted and thus just shrugs their shoulders.” — [cmiles8 (Hacker News)](<https://news.ycombinator.com/item?id=50482174>)

**Sources:**

1. [Claude status: Elevated errors on claude.ai, Claude Code, and platform.claude.com](<https://status.claude.com/incidents/nn11wk485zfn>) — primary source. Checked: 13 Nov 2026, 16:06 CET
2. [Claude status: Elevated errors on claude.ai, the Claude API, and Claude Code](<https://status.claude.com/incidents/34wq7gxnxvvm>) — primary source. Checked: 13 Nov 2026, 16:06 CET
3. [Hacker News discussion of the login incident](<https://news.ycombinator.com/item?id=50481273>) — community. Checked: 13 Nov 2026, 16:06 CET

### UPDATE: Bloomberg traces banned Nvidia servers to a Shanghai data centre linked to Alice Huang, and Lutnick agrees to testify to the Senate

*Industry & policy · Updated*

**Published:** 13 Nov 2026

Update to this morning's edition, which reported that Jensen Huang had agreed to testify behind closed doors to House committees. Three new developments on 13 November. First, Bloomberg reported, from Chinese credit filings and company documents it reviewed, that a company founded by Alice Huang procured **smuggled Nvidia servers installed at a Shanghai data centre**. Engadget, summarising Bloomberg, says the filings list 22 Dell servers with Nvidia H800 chips, banned in China, and 52 Super Micro servers with H100 or H200 chips, pledged as loan collateral by Shanghai Longteng Intelligent Computing, now majority-owned by a woman identified as Alice Huang's sister. Alice Huang left the company in 2017, and the documents do not say whether she was involved in buying the chips.

Second, a Reuters review published on 13 November identified Chinese AI computing projects and equipment agreements that explicitly reference restricted Nvidia H100, H200 and H800 processors, worth more than **23 billion yuan, about $3.2 billion**, according to Crypto Briefing's summary. The records range from planned investments to awarded contracts and facilities already running; one Gansu facility was awarded a 1.16 billion yuan contract in July for 3,072 H100 and H200 processors.

Third, CNBC reports that Senate Banking Committee chair Tim Scott sent letters on Thursday evening asking Huang to testify on 3 December and Lutnick on **10 December**. A Lutnick spokesperson told NBC News that he had agreed to appear voluntarily. Senator Jim Banks said on Fox News that Lutnick appears to have used loopholes to allow some chip sales; that is a lawmaker's accusation, not an established finding.

**Analysis — why it matters:** *Analysis: the affair is turning from a governance story into an **export-control investigation**, and its outcome could decide how much Nvidia hardware still reaches China.*

**Caveat:** Bloomberg's report is **paywalled and was not read**; its details come from Engadget's summary. The Reuters review was read through Crypto Briefing's summary; its total covers plans as well as delivered hardware, so it is **not a count of chips in use**. Megaspeed has denied wrongdoing, and no court or regulator has found that Jensen Huang broke export-control law.

**Sources:**

1. [Engadget: Bloomberg details web of Chinese AI companies with smuggled NVIDIA chips linked to Alice Huang](<https://engadget.com/2315710/bloomberg-details-web-of-chinese-ai-companies-with-smuggled-nvidia-chips-linked-to-alice-huang>) — reporting. Checked: 13 Nov 2026, 16:06 CET
2. [Crypto Briefing: Reuters finds more than $3 billion in Chinese AI projects built on restricted Nvidia chips](<https://cryptobriefing.com/nvidia-chinese-ai-projects-export-controls>) — reporting. Checked: 13 Nov 2026, 16:08 CET
3. [CNBC: Commerce Secretary Lutnick reportedly agrees to testify amid Nvidia scandal](<https://www.cnbc.com/2026/11/13/nvidia-scandal-lutnick-chip-sales.html>) — reporting. Checked: 13 Nov 2026, 16:06 CET

### US Department of War renames its Chief Digital and AI Office the Super Intelligence Office

*Industry & policy · New*

**Published:** 13 Nov 2026

The US Department of War announced on 13 November that its Chief Digital and Artificial Intelligence Office (CDAO) is now the **Department of War Super Intelligence Office (SIO)**. The department says the rebrand follows President Trump's direction to move federal terminology from artificial intelligence to Super Intelligence, and that the office now has a new logo and a new web address, si.mil.

The office's head, Cameron Stanley, said the mission is to harness sovereign Super Intelligence for military superiority. The release says the change will roll out over the coming weeks and that **existing programmes, solicitations and partnerships continue** unchanged; the office supports the Maven Smart System and the War Data Platform.

**Analysis — why it matters:** *Analysis: this is a **change of name, not of law or budget**, but it brings the Pentagon's main AI office in line with the administration's new vocabulary.*

**Caveat:** The release announces no new money, programmes or powers. The war.gov page blocked plain requests (HTTP 403) and was read with a Chrome-like TLS request.

**Sources:**

1. [U.S. Department of War: Department of War Redesignates CDAO as Super Intelligence Office](<https://www.war.gov/News/Releases/Release/Article/4647618/department-of-war-redesignates-cdao-as-super-intelligence-office/>) — primary source. Checked: 13 Nov 2026, 16:06 CET

### Amazon drafted a plan to gather data on nearly every product sold anywhere, partly to counter AI shopping agents, Reuters reports

*Industry & policy · New*

**Published:** 13 Nov 2026

Reuters reported on 13 November, citing an internal document and people familiar with the matter, that Amazon has a plan called **World Product Graph** to gather data on virtually every item for sale, whether Amazon stocks it or not. The document, a PR/FAQ memo, gives an aspirational public date of **1 October 2027**; Reuters could not determine whether or when the plan will be carried out.

According to Reuters, the document says Amazon has signed up Coca-Cola and Bayer to contribute product data and that Amazon would also crawl other retailers' websites. It says many answers from Amazon's shopping assistant Rufus, now Alexa for Shopping, are wrong or incomplete. People familiar with the matter told Reuters that executives see richer data as a way to make outside AI shopping agents come to Amazon.com rather than rival sites.

**Analysis — why it matters:** *Analysis: as agents such as Meta's Muse shop for people, **product data, not ad placement**, decides where purchases go; Amazon already blocks Muse from its store.*

**Caveat:** Amazon told Reuters the document is a **draft, outdated brainstorm** that does not necessarily reflect its plans, that its usage figures are outdated and that Alexa for Shopping is roughly 97% accurate. Reuters' own page blocked automated reading (HTTP 401) and was read through a syndicated copy on Euronext.

**Sources:**

1. [Euronext (Reuters): Exclusive - Amazon's plan to own the world's product data and fight AI shopping agents](<https://live.euronext.com/en/financial-news/exclusive-amazons-plan-own-worlds-product-data-and-fight-ai-shopping-agents>) — reporting. Checked: 13 Nov 2026, 16:06 CET

### EU leaders meet in Dublin for their first summit devoted to AI, briefed by Mistral's Arthur Mensch and Geoffrey Hinton

*Industry & policy · New*

**Published:** 13 Nov 2026

The 27 EU heads of state or government met in Dublin on 13 November for an informal European Council that the Council calls the **first leaders' strategic discussion on AI**: how AI can boost European competitiveness and its effects on society, security and trust. Ukraine was added as a second topic.

Reuters reports that **Mistral AI chief executive Arthur Mensch and Geoffrey Hinton** were to brief the leaders, and that the bloc's plan for seven AI gigafactories has yet to take off amid disputes over the 2028-2034 budget.

**Analysis — why it matters:** *Analysis: an informal summit makes no law, but it sets the agenda for the formal European Council in December.*

**Caveat:** Informal meetings adopt **no binding conclusions**, and no outcome had been published when this edition was issued. The Reuters preview was read through a syndicated copy on WTVB.

**Sources:**

1. [Council of the EU: Informal meeting of heads of state or government, 13 November 2026](<https://www.consilium.europa.eu/en/meetings/european-council/2026/11/13/>) — primary source. Checked: 13 Nov 2026, 16:06 CET
2. [WTVB (Reuters): EU leaders seek to tackle challenges at first ever AI summit](<https://wtvbam.com/2026/11/13/eu-leaders-seek-to-tackle-challenges-at-first-ever-ai-summit>) — reporting. Checked: 13 Nov 2026, 16:06 CET

## Key patterns (editorial analysis)

- The Nvidia affair is now about **export-control enforcement**: documents, a Reuters count of Chinese projects and Senate hearings in December.
- Agents are reshaping commerce and work: Amazon plans **product data to steer shopping agents**, while a Claude outage shows how much work now runs through one assistant.
- Governments are relabelling and debating AI rather than legislating today: a **renamed Pentagon office** and an informal EU summit.

## Source coverage

- Engine version: 3.31.0
- Engine ran this edition: yes
- Engine look-back: 2 days

### Source status

- reddit: ok, partial (18 threads; 24 sub-requests blocked with HTTP 403; Arctic Shift archive supplied posts)
- hackernews: ok (29 stories)
- github: ok (8 items)
- devto: ok (12 articles; tags ai and llm)
- youtube: not searched (yt-dlp not available on this machine)
- polymarket: not used: blocked in France (ANJ)
- x: not searched (no consent-free source configured)

### Notes

- The installed last30days engine finished with 67 evidence items from Reddit, Hacker News, dev.to and GitHub; its top cluster was the Claude login outage carried here. Most stories were found with 16 Google News RSS queries, publisher feeds, post-engine web supplements and the source pages. Item counts are not counts of verified developments.
- Polymarket not used: blocked in France (ANJ). X not searched. YouTube not searched (not available on this machine). Reddit returned results, but 24 of its sub-requests were blocked (HTTP 403), so Reddit coverage was partial. Missing coverage does not mean nobody discussed these stories.
- Paywalled and not read: Bloomberg's report on the Shanghai data centre (read through Engadget's summary) and The Information's report of job cuts on SpaceXSI's Grok Imagine team, which is therefore not carried. Reuters' own pages refused automated reading; its Nvidia review was read through Crypto Briefing's summary, its Amazon report through a syndicated copy on Euronext and its EU summit preview through WTVB. The war.gov release was read through a Chrome-like TLS request after a 403.
- Newsletter leads from the Iris mail bot: seven of today's eight leads were carried by earlier editions; the lead on UFORCE and Agile Robots funding rounds could not be verified against a primary source in time and is not carried.
- Not carried: Cerebras' third-quarter results and Microsoft deal, released on 12 November inside the morning edition's window; the continuing Microsoft 365 outage, not primarily an AI story; and coverage of Gemini 4 Hydrogen, the nonprofits' lawsuit and Anthropic's IPO that adds nothing material to this morning's stories.
- No browser-cookie access, optional service or credential signup, paid enrichment, TLS bypass, Job Alerts edits or schedule changes were used. Research logs and full provenance remain private.

### Engine footer (verbatim)

```text
---
✅ All agents reported back!
├─ 🟠 Reddit: 18 threads │ 39,782 upvotes │ 2,602 comments
├─ 🟡 HN: 29 stories │ 3,348 points │ 2,101 comments
├─ 👩‍💻 dev.to: 12 articles │ 233 reactions │ 181 comments
├─ 🐙 GitHub: 8 items │ 42 reactions │ 121 comments
├─ 🗣️ Top voices: r/technology, r/artificial, r/ClaudeAI
---
```
