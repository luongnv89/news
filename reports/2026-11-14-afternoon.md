# The AI Gazette — Afternoon edition, Saturday 14 November 2026

*Models, machines, and matters of consequence*

- Issue: 2026-11-14-afternoon
- Issued: 14 Nov 2026, 16:06 CET (Paris)
- Reporting window: 13 Nov 2026, 00:00 CET to 14 Nov 2026, 16:06 CET
- Timezone: Europe/Paris
- Previous issue: 2026-11-14-morning
- Price: Complimentary

## Editor's note

Ten hours since the morning edition, on a quiet Saturday with no new frontier model. Only two stories broke inside that window: **thousands marched in Edinburgh** against AI data centres, and Malaysia's home minister said police have investigated alleged Nvidia chip diversion since April 2025. So this edition widens its window to the start of Friday 13 November to carry six verified stories no earlier edition ran, several of them surfaced by newsletter leads: the Wall Street Journal's account of **how Jensen Huang financed Nvidia's own customers**, banks shutting Chinese and Hong Kong buyers out of Anthropic's IPO, DeepSeek opening its app's tools to developers, the White House AI task force's call for cyber liability relief, Cohere's purchase of cubic, and Moonshot's reported preparations for a Hong Kong listing. Reports and vendor claims are labelled as such.

## The News

### DeepSeek opens its app's web search, file reading, safety checks and voice tools to developers through its API

*Models · New*

**Published:** 13 Nov 2026

DeepSeek announced on Friday afternoon that the capabilities behind its chat app are now available through its API. Its **V4.1-Flash model (deepseek-flash)** now supports built-in web search, deep-thinking search across multi-step reasoning, file input for PDFs, Office files and images, automatic reading of links in user messages, and safety checks, across the Messages, Responses and Chat Completions interfaces, with tool calls handled on DeepSeek's servers.

Search, fetch, OCR, speech recognition and text-to-speech are also offered as standalone APIs, and the company published an **open-source demo chat client** that can import DeepSeek conversation history. The tools are billed on top of token charges. DeepSeek says public-facing apps must enable the safety checks and that developers stay responsible for moderation, model registration and labelling AI-generated content.

**Analysis — why it matters:** *Analysis: DeepSeek is turning its consumer app into a kit that developers can rebuild, bringing it closer to the hosted-tool APIs offered by US model labs.*

**Caveat:** Features and requirements are as described by DeepSeek; the edition did not test the APIs or their prices.

**Sources:**

1. [DeepSeek API Docs: The full DeepSeek App experience, now via API](<https://api-docs.deepseek.com/news/news261113/>) — primary source. Checked: 14 Nov 2026, 16:04 CET
2. [DeepSeek API Docs: Change log, 13 November 2026](<https://api-docs.deepseek.com/updates/>) — primary source. Checked: 14 Nov 2026, 16:04 CET
3. [GitHub: deepseek-ai/chat-demo](<https://github.com/deepseek-ai/chat-demo>) — primary source. Checked: 14 Nov 2026, 16:04 CET

### Cohere buys London AI code-review startup cubic and completes its purchase of AISLE

*Coding & agents · New*

**Published:** 13 Nov 2026

Cohere announced on Friday that it has acquired **cubic, an AI code-review platform**, and completed its acquisition of AISLE, which builds autonomous systems for finding and fixing software vulnerabilities. Terms were not disclosed. Cohere says it has now completed **four strategic acquisitions this year**, following Aleph Alpha and Reliant AI.

cubic's team, led by founder and chief executive Paul Sanglé-Ferrière, will set up a secure-coding unit at Cohere. cubic says its product will keep running and stay fully supported. BetaKit reports that cubic is based in London and that the deal had not been announced before Friday.

**Analysis — why it matters:** *Analysis: Cohere is assembling coding and security tools for customers that need on-premises or air-gapped deployments, a niche the large US labs serve less directly.*

**Caveat:** Cohere's claim that cubic's agents rank among the strongest on code-review benchmarks is a vendor claim and was not checked.

**Sources:**

1. [Cohere: Cohere expands its sovereign AI platform with AISLE and cubic](<https://cohere.com/blog/cohere-expands-its-sovereign-ai-platform-with-aisle-and-cubic>) — primary source. Checked: 14 Nov 2026, 16:04 CET
2. [cubic: cubic joins Cohere](<https://www.cubic.dev/blog/cubic-joins-cohere>) — primary source. Checked: 14 Nov 2026, 16:04 CET
3. [BetaKit: Cohere buys AI code review startup Cubic as acquisition spree continues](<https://betakit.com/cohere-buys-ai-code-review-startup-cubic-as-acquisition-spree-continues/>) — reporting. Checked: 14 Nov 2026, 16:04 CET

### Jensen Huang pushed Nvidia to finance its own customers to absorb a coming chip glut, the Wall Street Journal reports

*Industry & policy · New*

**Published:** 13 Nov 2026

First reported by the Wall Street Journal on Friday evening, Paris time. The paper describes an **August 2026 meeting** at which Nvidia's chief financial officer Colette Kress, now interim chief executive, pushed to rein in the company's "circular financing" of smaller cloud providers and AI firms such as OpenAI and Anthropic, according to Wccftech's account of the report.

According to that account, early talks had floated underwriting about 8 gigawatts of OpenAI computing worth up to $250 billion, and Kress cut Nvidia's signed guarantee cap to **about 4.25 gigawatts, or up to $125 billion**. Huang is reported to have called her "a deer in the headlights" and to have said privately that prepaid TSMC wafers and memory were "coming at him like an avalanche" as large cloud companies moved to their own custom chips. Nvidia reportedly asked TSMC to wind down upcoming orders.

TechCrunch reported separately on Friday that Nvidia took part in **105 startup funding rounds this year**, according to PitchBook, and quoted investors who expect Kress to be more cautious than Huang about such deals.

**Analysis — why it matters:** *Analysis: if the account holds, part of the demand that made Nvidia's chips look scarce was demand Nvidia paid for itself, which matters for how investors read its results on 17 November and for the neoclouds that depend on its money.*

**Caveat:** The Wall Street Journal article is paywalled and was not read; this account comes from Wccftech's summary of it. The report rests on **unnamed sources**, and none of the coverage read includes a response from Nvidia. Claims that Nvidia deliberately engineered a GPU shortage are commentators' interpretations, not findings of the report.

**Community reaction (opinion, not verified fact):**

> “This is third source reporting. WSJ does the original, Wccftech reports that WSJ reports, now Techpowerup reports what Wccftech reports about WSJ reporting.” — [u1hcw9nx on Hacker News](<https://news.ycombinator.com/item?id=50495294>)

> “Because of bottlenecks in the supply chain, Nvidia knows it is going to sell 100% of its inventory.” — [Silfen on Hacker News](<https://news.ycombinator.com/item?id=50495956>)

**Sources:**

1. [Wccftech: Former Nvidia CEO Jensen Huang reportedly financed AI startups to absorb excess silicon (summary of the WSJ report)](<https://wccftech.com/jensen-huang-financed-ai-startups-absorb-excess-silicon/>) — reporting. Checked: 14 Nov 2026, 16:04 CET
2. [TechCrunch: Jensen Huang's departure blasts big hole in AI startup funding, VCs and founders say](<https://techcrunch.com/2026/11/13/jensen-huangs-departure-blasts-big-hole-in-ai-startup-funding-vcs-and-founders-say/>) — reporting. Checked: 14 Nov 2026, 16:04 CET
3. [Hacker News discussion (826 points)](<https://news.ycombinator.com/item?id=50495294>) — community. Checked: 14 Nov 2026, 16:04 CET

### UPDATE: Banks shut Chinese and Hong Kong institutions out of Anthropic's IPO, Bloomberg reports

*Industry & policy · Updated*

**Published:** 13 Nov 2026

Update to the 13 November morning edition, which reported the offering about six times oversubscribed. The new development, first reported by Bloomberg on Friday evening: institutional investors based in **mainland China and Hong Kong have been excluded** from placing orders in Anthropic's initial public offering.

Several banks have refused such orders or consider allocations unlikely, according to people familiar with the matter, and some of them cited the **US International Traffic in Arms Regulations**, The Decoder reports from Bloomberg's story. Anthropic declined to comment. Goldman Sachs and Morgan Stanley lead the offering with 20 other banks; pricing is expected on 18 November and trading on Nasdaq under the ticker ANT after that.

**Analysis — why it matters:** *Analysis: rules written for defence goods are being cited to decide who may own part of a frontier AI lab, extending US-China restrictions from products to shareholdings.*

**Caveat:** Bloomberg's article is paywalled and was not read; the account comes from The Decoder and Yahoo Finance summaries. The exclusion is attributed to unnamed people, and final allocations rest with Anthropic and its banks.

**Sources:**

1. [The Decoder: Banks bar Chinese and Hong Kong investors from Anthropic IPO over US export controls](<https://the-decoder.com/banks-bar-chinese-and-hong-kong-investors-from-anthropic-ipo-over-us-export-controls/>) — reporting. Checked: 14 Nov 2026, 16:04 CET
2. [Yahoo Finance: Anthropic IPO reportedly closed to China, Hong Kong buyers](<https://finance.yahoo.com/markets/stocks/articles/anthropic-ipo-reportedly-closed-china-174510000.html>) — reporting. Checked: 14 Nov 2026, 16:04 CET

### Thousands march in Edinburgh against large AI data centres as Scotland weighs more than 20 proposals

*Industry & policy · New*

**Published:** 14 Nov 2026, 14:25 CET

Thousands of people marched down Edinburgh's Royal Mile to the Scottish Parliament on Saturday to protest against **large-scale AI data centres**, the BBC reports. Some came to oppose particular sites, including Cockenzie in East Lothian and Larbert in Falkirk.

The organisers, a coalition including Friends of the Earth Scotland, say **more than 20 proposals** for hyperscale AI data centres have been submitted in Scotland and want a public consultation before any are approved. According to the BBC, more than 70 protests against data centres are taking place in 15 European countries this month. A planned site at Chapelcross in Dumfries and Galloway would have a capacity of 1,000 MW, against about 12 MW for what is thought to be Scotland's largest today.

The Scottish government said it would publish new planning guidance on data centres before the end of the year and now requires an environmental impact assessment for any new data centre above 50 MW. Innovation minister Alyn Smith called some of the debate "wild".

**Analysis — why it matters:** *Analysis: local opposition to data centres is now organised across Europe and is pressing directly on planning decisions.*

**Caveat:** Crowd size is the BBC's description; no official count was published in the sources read.

**Sources:**

1. [BBC News: Thousands turn out in Edinburgh to protest against AI data centres](<https://www.bbc.co.uk/news/articles/c8n50w445zgpo>) — reporting. Checked: 14 Nov 2026, 16:04 CET
2. [Friends of the Earth Scotland: Thousands expected to join march against AI data centres in Edinburgh (15 October)](<https://foe.scot/press-release/thousands-expected-to-join-march-against-ai-data-centres-in-edinburgh/>) — primary source. Checked: 14 Nov 2026, 16:04 CET

### White House AI task force urges at least 12 months of regulatory liability relief for companies that report cyber incidents in good faith

*Industry & policy · New*

**Published:** 13 Nov 2026

In a statement after its second meeting, held on Thursday 12 November and reported on Friday, the Trump administration's AI task force urged federal agencies to **"implement limitations on regulatory liability"** for good-faith voluntary reporting of cybersecurity vulnerabilities and incidents, where that is lawful, practical and consistent with public health and safety, Cybersecurity Dive reports.

The flexibility should last **at least 12 months**, with possible extension. The task force said organisations that recently had reasonable protections are now more vulnerable as AI changes the threat landscape, and that prior enforcement standards "may be outdated". It also backed long-term reauthorisation of the 2015 Cybersecurity Information Sharing Act, which is due to expire in December, and discussed a voluntary process for companies to report AI-related incidents.

**Analysis — why it matters:** *Analysis: Washington is choosing incentives over penalties to get AI-era breaches reported, at the moment the legal shield for sharing threat data is about to lapse.*

**Caveat:** This is a **recommendation, not a rule**: no agency has yet said it will adopt it, and the CISA Act renewal needs Congress. The task force's statement was read through press reports, not on a government site.

**Sources:**

1. [Cybersecurity Dive: White House task force says companies deserve liability relief for AI-fueled cyberattacks](<https://www.cybersecuritydive.com/news/ai-white-house-task-force-cybersecurity-regulation/874679/>) — reporting. Checked: 14 Nov 2026, 16:04 CET
2. [AI Affairs: Trump's AI task force weighs protections for reporting cyberattacks (Reuters account)](<https://www.aiaffairs.com/government/trump-ai-task-force-cyberattack-reporting-protections/>) — reporting. Checked: 14 Nov 2026, 16:04 CET

### Kimi maker Moonshot AI is dismantling its offshore holding company ahead of a planned Hong Kong listing, the Wall Street Journal reports

*Industry & policy · New*

**Published:** 13 Nov 2026

First reported by the Wall Street Journal on Friday. Moonshot AI is wrapping up a restructuring in which it **deactivates its Cayman Islands holding company** and moves dollar investors' stakes into its main operating company in China, buying back their offshore shares so the money can be reinvested onshore, according to accounts of the report by PANews and Finanzen100.

According to Finanzen100's account, the company could list in Hong Kong **as early as 2027**, raising up to $5 billion, after a pre-IPO round valued it at about $50 billion; Beijing has been pressing companies to drop offshore structures before listing, and rival StepFun has already done so. Moonshot declined to comment.

**Analysis — why it matters:** *Analysis: Chinese model labs are lining up onshore-friendly listings in Hong Kong while US labs list in New York, splitting the AI capital market along the same line as chips and models.*

**Caveat:** The Wall Street Journal article is paywalled and was not read; the details come from secondary accounts of it and rest on **unnamed sources**. Timing and size of any listing are not confirmed by Moonshot.

**Sources:**

1. [PANews: WSJ: Moonshot AI undergoing restructuring to pave way for IPO](<https://panews.io/articles/01a1d422-1d14-773d-bf61-a76f257139c9>) — reporting. Checked: 14 Nov 2026, 16:04 CET
2. [Finanzen100 (Wallstreet-Online): Chinas KI-Hoffnung Moonshot plant Milliarden-Börsengang](<https://www.finanzen100.de/news/chinas-ki-hoffnung-moonshot-plant-milliarden-boersengang_a5425730-7423-458a-977b-6f1b83f08f0a.html>) — reporting. Checked: 14 Nov 2026, 16:04 CET
3. [TokenPost: Moonshot AI begins offshore restructuring as it weighs 2027 Hong Kong IPO](<https://www.tokenpost.com/news/business/56492>) — reporting. Checked: 14 Nov 2026, 16:04 CET

### UPDATE: Malaysia says its police have investigated alleged diversion of Nvidia AI chips through the country since April 2025

*Industry & policy · Updated*

**Published:** 14 Nov 2026

Update to this week's editions on the Nvidia scandal and chip smuggling. The new development: Malaysia's home minister, **Saifuddin Nasution Ismail**, said on Saturday that police opened an investigation in **April 2025** into US allegations that Malaysia was used as a transit hub, or that local proxy companies were set up, to get restricted AI chips, including Nvidia's, past US export controls.

The probe runs under the Strategic Trade Act 2010, with the trade ministry as lead agency and the central bank, tax authority, communications regulator and customs involved, he told reporters. He would not say whether evidence has been found, calling it a very complex investigation, and said progress is being passed to the trade ministry to convey to the US, which lodged the complaint.

**Analysis — why it matters:** *Analysis: the minister's account dates Malaysia's inquiry well before the Huang scandal broke, as Washington moves to close third-country routes for advanced chips.*

**Caveat:** The minister did not say whether the allegations have been substantiated, and no charges have been announced.

**Sources:**

1. [The Edge Malaysia: Malaysia probing alleged Nvidia AI chip diversion since April 2025, home minister](<https://theedgemalaysia.com/node/825768>) — reporting. Checked: 14 Nov 2026, 16:04 CET
2. [Free Malaysia Today: Police probing alleged Nvidia chip diversion since April 2025, says Saifuddin](<https://www.freemalaysiatoday.com/category/nation/2026/11/14/police-probing-alleged-nvidia-chip-diversion-since-april-2025-says-saifuddin>) — reporting. Checked: 14 Nov 2026, 16:04 CET

## Key patterns (editorial analysis)

- The Nvidia story has moved from scandal to business model, with the WSJ describing **customer financing to absorb a chip glut**.
- US-China lines now run through capital markets too: **China excluded from Anthropic's IPO** while Moonshot readies a Hong Kong listing.
- Opposition to AI's physical footprint is organising, from **thousands in Edinburgh** to more than 70 protests across Europe this month.

## Source coverage

- Engine version: 3.31.0
- Engine ran this edition: yes
- Engine look-back: 2 days

### Source status

- reddit: ok, partial (22 threads; 24 sub-requests blocked with HTTP 403 and 4 archive queries failed with HTTP 422; Arctic Shift archive supplied posts)
- hackernews: ok (30 stories)
- github: ok (9 items)
- devto: ok (12 articles; tags ai and llm)
- youtube: not searched (yt-dlp not available on this machine)
- polymarket: not used: blocked in France (ANJ)
- x: not searched (no consent-free source configured)

### Notes

- The installed last30days engine finished with 73 evidence items from Reddit, Hacker News, dev.to and GitHub; its top new cluster was the Nvidia financing report carried here. Most stories were found with 16 Google News RSS queries, publisher feeds, post-engine web supplements and the source pages. Item counts are not counts of verified developments.
- Window: widened to start at midnight on 13 November, about 40 hours before this edition, to carry stories from Friday that no earlier edition ran, including newsletter leads. Only the Edinburgh march and the Malaysian minister's statement fall inside the normal window since the morning edition.
- Polymarket not used: blocked in France (ANJ). X not searched. YouTube not searched (not available on this machine). Reddit returned results, but 24 of its sub-requests were blocked (HTTP 403), so Reddit coverage was partial. Missing coverage does not mean nobody discussed these stories.
- Paywalled and not read: the Wall Street Journal's reports on Nvidia's financing and on Moonshot AI, and Bloomberg's report on Anthropic's IPO, each read through the secondary accounts cited. TechPowerUp's summary refused automated reading (HTTP 403) and is not cited.
- Newsletter leads from the Iris mail bot: carried here are the WSJ Nvidia financing report, the White House task force recommendation and Cohere's purchase of cubic. Not carried: the reported theft of $11.4 million of Nvidia hardware in transit, not primarily an AI story; earlier leads were carried by previous editions.
- Not carried: Microsoft winding down its Oracle cloud deal (reported 6 November), John Langford's departure from Microsoft and the Gemini Chromebook lawsuit (both from early November), Humain's $667 million financing (signed 9 November), Liquid AI's LiquidCodec (12 November), and resurfaced coverage of Claude Code Projects and Gemini 4 Hydrogen.
- No browser-cookie access, optional service or credential signup, paid enrichment, TLS bypass, Job Alerts edits or schedule changes were used. Research logs and full provenance remain private.

### Engine footer (verbatim)

```text
---
✅ All agents reported back!
├─ 🟠 Reddit: 22 threads │ 12,976 upvotes │ 2,197 comments
├─ 🟡 HN: 30 stories │ 3,338 points │ 2,463 comments
├─ 👩‍💻 dev.to: 12 articles │ 325 reactions │ 125 comments
├─ 🐙 GitHub: 9 items │ 48 reactions │ 124 comments
├─ 🗣️ Top voices: r/artificial, r/singularity, r/OpenAI
---
```
