# The AI Gazette — Afternoon edition, Wednesday 4 November 2026

*Models, machines, and matters of consequence*

- Issue: 2026-11-04-afternoon
- Issued: 4 Nov 2026, 16:09 CET (Paris)
- Reporting window: 4 Nov 2026, 06:09 CET to 4 Nov 2026, 16:09 CET
- Timezone: Europe/Paris
- Previous issue: 2026-11-04-morning
- Price: Complimentary

## Editor's note

This Wednesday afternoon edition covers the ten hours since this morning's 06:09 edition and carries **six new stories**. US voters backed limits on data centres in almost every local ballot measure, OpenAI agreed to buy Pierre Computer for Codex, and Tencent released Hy4 with open weights promised in days. Oracle dropped a chip lease with Tencent after US objections, according to the FT, Google agreed to backstop Anthropic's leases with TeraWulf, and WIRED traced Britain's £400 billion AI claim to a Google-commissioned report. **No new frontier model from a US lab** passed this journal's checks.

## The News

### Tencent releases Hy4, adding image understanding and computer use, and says open weights will follow in days

*Models · New*

**Published:** 4 Nov 2026, 09:06 CET

Tencent released **Hy4**, the latest generation of its large language model, on Wednesday. It says Hy4 understands images for the first time and can **operate command-line and graphical software**, with special training on tools such as Blender and CAD. Tencent also reports gains in instruction following, long documents and long agent tasks.

The model is live in Tencent products including WorkBuddy, CodeBuddy and Yuanbao, through Tencent Cloud TokenHub and through third-party platforms such as OpenRouter. Pricing is unchanged from the earlier Hy4 Preview at about **$0.90 per million input tokens** and $2.70 per million output tokens. Tencent says it will publish model weights and system cards in the coming days.

Tencent's own figures include a cut in its internal hallucination rate from 12.95% for Hy4 Preview to 7.2%, and first place among open-source models in a blind test of 579 financial tasks with 213 finance professionals, scoring 3.04 against 2.97 for DeepSeek-V4.1-Flash-1017.

**Analysis — why it matters:** *Analysis: Another large Chinese lab is promising open weights for a frontier-class model, keeping **price pressure on paid models**, though the claim to rank among the leading open models cannot be checked until the weights appear.*

**Caveat:** The benchmark and hallucination figures are **Tencent's own evaluations**. At press time the weights had not been published: a check of Hugging Face found no public Hy4 repository.

**Community reaction (opinion, not verified fact):**

> “Looks like they decided to spend a lot of time/effort on visual, and motion/animation abilities with Hy4.” — [sshah03 (Hacker News)](<https://news.ycombinator.com/item?id=50362313>)

**Sources:**

1. [Tencent](<https://www.tencent.com/tencent-launches-hy4-joining-the-ranks-of-the-worlds-leading-open-source-ai-models/>) — primary source. Checked: 4 Nov 2026, 16:03 CET
2. [Hacker News discussion](<https://news.ycombinator.com/item?id=50362313>) — community. Checked: 4 Nov 2026, 16:02 CET

### OpenAI agrees to buy Pierre Computer, whose code-review tools already run inside Codex

*Coding & agents · New*

**Published:** 4 Nov 2026

OpenAI said on Wednesday that it will acquire **Pierre Computer Company**, the maker of Code Storage and a family of open-source developer tools. Pierre's Trees and Diffs libraries already power file browsing and change review in the Codex app.

Code Storage is a service that lets apps store code and track its history using Git. OpenAI said customers can keep using it after the deal closes while it brings its features into Codex, and that **Pierre's open-source projects will stay open-source**. Financial terms were not disclosed, and the deal still needs regulatory approval.

Axios, which first reported the deal, framed it as a challenge to Microsoft's GitHub as agents write more code; Microsoft owns nearly a quarter of OpenAI, Axios notes. Earlier this week OpenAI revealed Pando, a source-control backend that it says cut the time needed to push code changes by nearly 80%.

**Analysis — why it matters:** *Analysis: Coding-agent makers are moving from writing code to **owning where code is stored and reviewed**, which puts OpenAI in more direct competition with GitHub, owned by one of its largest shareholders.*

**Caveat:** The acquisition has **not yet closed** and is subject to regulatory approvals; until then the two companies remain separate. The Pando figure is OpenAI's own.

**Sources:**

1. [OpenAI](<https://openai.com/index/openai-to-acquire-pierre/>) — primary source. Checked: 4 Nov 2026, 16:03 CET
2. [Axios (Yahoo Finance copy)](<https://finance.yahoo.com/technology/ai/articles/exclusive-openai-targets-microsofts-github-112906674.html>) — reporting. Checked: 4 Nov 2026, 16:09 CET

### US voters back limits on data centres in almost every local ballot measure, in unofficial midterm results

*Industry & policy · New*

**Published:** 4 Nov 2026

Voters in more than 30 localities across nine states backed **moratoriums, outright bans and other limits** on data centres in Tuesday's US midterm elections, Semafor reported. Edgewater, Florida voted to write a data-centre ban into its city charter, and voters in Perry, Ohio approved financial and operating conditions for hyperscale developers that seek tax breaks.

Counts differ by tracker, and every figure is unofficial. Tom's Hardware, citing the Data Centers on the Ballot tracker, said **33 measures restricting development had won**, six more were leading, one measure in Harwood, North Dakota had failed and five had no posted results. Business Insider cited a Redbud Consulting count of 33 restricting measures approved against one allowing data centres, as of 8 a.m. Eastern time.

Business Insider also reported that NBC News' exit poll found **76% of voters would oppose** a new data centre in their community. It quoted Goldman Sachs economists who said Democratic wins at state and local level would likely bring short-term moratoria potentially affecting about 45% of planned US data-centre capacity expansion.

**Analysis — why it matters:** *Analysis: This is the first large test of local opinion on the AI build-out at the ballot box, and the result points one way. Power, land and permits, not only chips, now **limit where AI capacity can go**.*

**Caveat:** All counts are **unofficial and not yet certified**, and the trackers count measures differently. Tom's Hardware notes that it is unclear whether the votes affect projects already under way. The Goldman Sachs figure is an economists' estimate, not a result.

**Community reaction (opinion, not verified fact):**

> “Kevin Oleary's data center is going to be built one hour from my town.” — [twiclo (Hacker News)](<https://news.ycombinator.com/item?id=50366371>)

> “The fact that Americans can be made to vote for NIMBY policies was well known.” — [pj\_mukh (Hacker News)](<https://news.ycombinator.com/item?id=50366365>)

**Sources:**

1. [Semafor](<https://www.semafor.com/article/11/04/2026/us-voters-roundly-reject-data-centers-in-ballot-measures>) — reporting. Checked: 4 Nov 2026, 16:03 CET
2. [Tom's Hardware](<https://www.tomshardware.com/tech-industry/data-centers/ai-data-centers-comprehensively-defeated-at-us-midterm-elections-45-measures-put-on-the-ballot-as-americans-overwhelmingly-vote-against-developments>) — reporting. Checked: 4 Nov 2026, 16:03 CET
3. [Business Insider](<https://www.businessinsider.com/data-centers-hammered-midterms-key-votes-show-how-2026-11>) — reporting. Checked: 4 Nov 2026, 16:04 CET
4. [Hacker News discussion](<https://news.ycombinator.com/item?id=50366371>) — community. Checked: 4 Nov 2026, 16:02 CET

### Oracle drops an estimated $7 billion chip lease with Tencent after US officials object, FT reports

*Industry & policy · New*

**Published:** 4 Nov 2026

Oracle has cancelled a chip-leasing contract with Tencent worth an estimated **$7 billion** after US officials raised concerns about it, the Financial Times reported on Wednesday, citing people familiar with the matter. Reuters said it could not immediately verify the report, and Oracle, Tencent and the White House did not respond to its requests for comment.

Under the five-year lease, first reported by the FT last month, Tencent was to rent capacity in Oracle data centres in Southeast Asia, giving it use of about **100,000 advanced AI chips** that it cannot obtain in China. The FT also reported that officials from Guangdong, where Tencent is based, visited the company and asked it to support domestic Chinese chips.

**Analysis — why it matters:** *Analysis: Following Tuesday's FT report on Nvidia's limit on Chinese cloud customers, this is a second sign that Washington is **closing the overseas rental route** to top AI chips, here through pressure rather than a new rule.*

**Caveat:** The account rests on the FT's **unnamed sources**; no company had confirmed it at press time. The original FT article was not read; this dispatch relies on The Next Web's account of the FT and Reuters reports.

**Sources:**

1. [The Next Web](<https://thenextweb.com/news/oracle-cancels-tencent-ai-chip-lease>) — reporting. Checked: 4 Nov 2026, 16:04 CET

### Google agrees to backstop Anthropic's $19 billion of data-centre leases with TeraWulf in Kentucky

*Industry & policy · New*

**Published:** 4 Nov 2026, 14:15 CET

Data-centre developer TeraWulf said on Wednesday that Google has signed credit support agreements for debt financing tied to about **$19 billion of lease commitments** from Anthropic at its Justified Data Campus in Hawesville, Kentucky. TeraWulf also signed a definitive construction contract with Fluor for three data-centre buildings there.

TeraWulf's filing with the US securities regulator says that if Anthropic defaults on rent or becomes insolvent, Google can **take over the lease** as tenant or, in some cases, pay a termination fee and take an equity stake in the TeraWulf subsidiary that owns the site. The backstop ends once Anthropic holds certain investment-grade credit ratings for at least three months.

The 20-year lease covers about 401 megawatts of critical IT load. TeraWulf expects phased delivery from late 2027 through the second quarter of 2028.

**Analysis — why it matters:** *Analysis: Big cloud companies are now lending their credit ratings to AI labs' landlords. Google, an Anthropic investor and chip supplier, is **underwriting part of the risk** that a fast-growing lab cannot pay its rent.*

**Caveat:** The $19 billion is TeraWulf's figure for contracted lease commitments over the lease term, not money paid to date. Completion dates are **TeraWulf's expectations**.

**Sources:**

1. [TeraWulf (GlobeNewswire)](<https://www.globenewswire.com/news-release/2026/11/04/3395277/0/en/terawulf-secures-google-credit-backstop-for-project-financing-in-support-of-19-billion-anthropic-lease-executes-definitive-fluor-epc-agreement.html>) — primary source. Checked: 4 Nov 2026, 16:04 CET
2. [TeraWulf 8-K filing (Stock Titan copy)](<https://www.stocktitan.net/sec-filings/WULF/8-k-terawulf-inc-reports-material-event-89658a64f514.html>) — primary source. Checked: 4 Nov 2026, 16:07 CET
3. [CNA (Reuters)](<https://www.channelnewsasia.com/business/terawulf-gets-credit-backstop-google-anthropic-data-center-project-6524516>) — reporting. Checked: 4 Nov 2026, 16:04 CET

### WIRED: Britain's '£400 billion from AI' claim came from a Google-commissioned report; the government's own estimate is £120 billion

*Industry & policy · New*

**Published:** 4 Nov 2026, 14:49 CET

For almost two years, British ministers and agencies said AI could give the economy a **£400 billion boost**. WIRED reported on Wednesday that the UK's AI minister, Kanishka Narayan, said in a parliamentary answer last week that the figure came from a 2023 report commissioned by Google and produced by the consultancy Public First, now PF Global.

In the same answer, Narayan said AI adoption and data investment could add £55 billion to £140 billion to the UK economy by 2030, with a **central estimate of £120 billion**, and called even that 'hugely uncertain'. WIRED says ministers have had the lower estimate since at least November 2025, and the answer did not withdraw the £400 billion figure.

PF Global told WIRED the gap partly reflects slower AI adoption than its 2023 model assumed.

**Analysis — why it matters:** *Analysis: Headline economic claims for AI often trace back to **studies paid for by the industry**. Here a government's own number turned out to be under a third of the one it promoted.*

**Caveat:** The minister's answer came last week; WIRED's report linking the figures is dated 4 November. Both estimates are **projections, not measurements**.

**Sources:**

1. [WIRED](<https://www.wired.com/story/uk-officials-said-ai-would-add-400-billion-to-the-economy-that-figure-mainly-came-from-google/>) — reporting. Checked: 4 Nov 2026, 16:04 CET

## Key patterns (editorial analysis)

- Public consent is becoming a limit on AI infrastructure: local voters backed limits in **almost every data-centre measure** on Tuesday's ballots.
- Capital and access are being steered from outside the labs: Google backstopped Anthropic's landlord, and US pressure reportedly **ended Tencent's overseas chip lease**.
- Coding agents are pulling in the plumbing around code, as OpenAI buys Pierre's review and storage tools for Codex.

## Source coverage

- Engine version: 3.31.0
- Engine ran this edition: yes
- Engine look-back: 2 days

### Source status

- reddit: ok (21 threads)
- youtube: ok (3 videos; transcripts for 3 of 3)
- hackernews: ok (11 stories)
- github: ok (24 items)
- devto: ok (12 articles; tags ai and llm)
- polymarket: not used: blocked in France (ANJ)
- x: not searched (no consent-free source configured)

### Notes

- The window runs from this morning's 06:09 CET edition to this edition. Dispatches with only a date carry the date of their primary source or first report. The ballot measures were voted on 3 November; the reports and counts cited are dated 4 November.
- The installed last30days engine finished in 41 seconds with 71 evidence items from Reddit, Hacker News, GitHub, dev.to and YouTube. Its strongest new clusters were the data-centre ballot results and Tencent Hy4; its top YouTube items were commentary and interviews, and Revolut's self-hosting talk (covered this morning as BACKGROUND) was not repeated. Stories were found with Google News RSS, publisher feeds, web searches before and after the engine run and the primary pages. Item counts are not counts of verified developments.
- The community quotes come from the engine's relevance-qualified Hacker News comments. They are anecdotal reactions, not evidence for the figures reported.
- Polymarket not used: blocked in France (ANJ). X was not searched. All five engine sources completed normally. Missing coverage does not mean nobody discussed these stories.
- TeraWulf's GlobeNewswire release returned HTTP 403 and was read live through the fetch ladder's Chrome-like TLS route. A U.S. News copy of Reuters' Oracle report could not be read by any route (timeout, HTTP 403 and an Internet Archive HTTP 429), so the Oracle dispatch relies on The Next Web; the Financial Times original was not read. Axios' Pierre report returned HTTP 403 on axios.com and was read in Yahoo Finance's syndicated copy. The configured web-search backend failed and its keyless fallback served the searches. VentureBeat's feed returned HTTP 429 and Anthropic's news feed HTTP 404.
- Not carried: OpenAI's claim that ChatGPT handles about a fifth of Google's search volume (made on 2 November), the tampered Claude Code extension in Cursor's marketplace (29 October), the Driscoll hire and Goldman Sachs' AI tool limits (covered earlier), Google's health-AI evaluation framework (no new study details found), and a report that Nvidia can meet only 1% of Chinese chip orders, which was not checked against its original source by press time.
- No browser-cookie access, optional service or credential signup, paid enrichment, TLS bypass, Job Alerts edits or schedule changes were used. Research logs and full provenance remain private.

### Engine footer (verbatim)

```text
---
✅ All agents reported back!
├─ 🟠 Reddit: 21 threads │ 13,226 upvotes │ 1,178 comments
├─ 🔴 YouTube: 3 videos │ 2,654,672 views │ 3/3 with transcripts
├─ 🟡 HN: 11 stories │ 1,590 points │ 606 comments
├─ 👩‍💻 dev.to: 12 articles │ 269 reactions │ 49 comments
├─ 🐙 GitHub: 24 items │ 1,829 reactions │ 289 comments
├─ 🗣️ Top voices: r/technology, r/artificial, r/singularity
---
```
