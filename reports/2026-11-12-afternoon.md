# The AI Gazette — Afternoon edition, Thursday 12 November 2026

*Models, machines, and matters of consequence*

- Issue: 2026-11-12-afternoon
- Issued: 12 Nov 2026, 16:11 CET (Paris)
- Reporting window: 11 Nov 2026, 00:00 CET to 12 Nov 2026, 16:05 CET
- Timezone: Europe/Paris
- Previous issue: 2026-11-12-morning
- Price: Complimentary

## Editor's note

Since this morning's edition, **Jensen Huang has resigned as Nvidia's chief executive**, and chief financial officer Colette Kress is running the company while the board looks for a successor. Reuters reports that Chinese AI firms are rushing to rent Nvidia capacity abroad before Washington can close that route. Google opened pre-orders for its **Gemini glasses from $395**, Baidu launched a model marketplace and two ERNIE models, Nebius beat revenue forecasts but trimmed its 2026 outlook, and France announced an international defence AI centre in Rennes. There is no new frontier model in this window. To carry two 11 November items no earlier edition ran, AWS's agent-built emulator and the EU's rules for AI sandboxes, **the window was widened to midnight on 11 November**, about 40 hours before this edition.

## The News

### Google opens pre-orders for Gemini-powered Intelligent Eyewear from Warby Parker and Gentle Monster, from $395

*Models · New*

**Published:** 12 Nov 2026, 15:00 CET

Google opened pre-orders on 12 November for **Intelligent Eyewear**, glasses with Gemini built in, designed with Warby Parker and Gentle Monster and engineered by Samsung. They go on sale in stores and online on **10 December**, for Google accounts in the United States and South Korea.

Warby Parker's three styles start at **$395** and Gentle Monster's six designs at **$449**, with prescription options. Google says the frames weigh about 41 grams, have a 12-megapixel camera, open-ear speakers and up to nine hours of battery life, and work with recent Pixel, Samsung and iPhone models.

Users say "Hey Gemini" or tap the frame for help about what they see, Maps directions and Translate speech translation across more than 70 languages. Google says camera images sent to Gemini are not kept in Gemini history or used for training or ads, and that bystanders' faces are blurred automatically before Gemini processes them; a light shows when the glasses record.

**Analysis — why it matters:** *Editorial analysis: this puts **Google's assistant in a camera worn on the face** against Meta's glasses, and its privacy promises will be tested in public.*

**Caveat:** Battery life, face redaction and the privacy protections are Google's own claims; the glasses were not independently tested for this edition. Some features, including Guided Vision and Audible, work only with Android phones at launch.

**Sources:**

1. [Google: See our intelligent eyewear lineup and pre-order your pair](<https://blog.google/innovation-and-ai/technology/xr-ar/google-intelligent-eyewear-collections-pre-order/>) — primary source. Checked: 12 Nov 2026, 16:02 CET
2. [Google: Designing for privacy on intelligent eyewear](<https://blog.google/innovation-and-ai/technology/safety-security/intelligent-eyewear-privacy-protections/>) — primary source. Checked: 12 Nov 2026, 16:04 CET

### Baidu launches Token Exchange, a marketplace for models from many suppliers, and two ERNIE models at Baidu World 2026

*Models · New*

**Published:** 12 Nov 2026

At Baidu World 2026 in Beijing on 12 November, founder Robin Li launched **Token Exchange**, a platform where companies buy and call models from many suppliers through one API. Baidu says it runs admission tests, including model fingerprint checks, to keep out swapped models, and gives suppliers credit ratings. Pandaily reports that Baidu says the API supports both OpenAI and Anthropic protocols.

Baidu also released two models on its Qianfan cloud platform: **ERNIE Lightning**, a reasoning model first built for Baidu Search, and **ERNIE-Wizshot-ME**, which turns a still portrait into a 4- to 15-second 1080p talking video. Pandaily reports a list price of 0.7 yuan per second for the video model.

Baidu claims Token Exchange already averages more than **700 billion tokens a day** from over 100 supply resources; its own product page still shows lower figures, 200 billion tokens and 70 models.

**Analysis — why it matters:** *Editorial analysis: China has many cheap model resellers; **Baidu is pitching itself as the referee** that verifies which model is really answering.*

**Caveat:** Usage figures and cost savings are Baidu's claims and have not been independently checked. Baidu has not explained how its fingerprinting or ratings work, nor published benchmarks or sizes for the two models.

**Sources:**

1. [Baidu AI Cloud: Token Exchange product page](<https://cloud.baidu.cn/product-s/token_exchange.html>) — primary source. Checked: 12 Nov 2026, 16:05 CET
2. [Pandaily: Baidu Launches Token Exchange, a Model Marketplace That Fingerprints Models and Rates Suppliers](<https://pandaily.com/baidu-token-exchange-model-marketplace-fingerprinting-supplier-credit-ratings>) — reporting. Checked: 12 Nov 2026, 16:03 CET
3. [Pandaily: Baidu Puts ERNIE Lightning Reasoning Model and ERNIE-Wizshot-ME Expressive Video Model on Qianfan](<https://pandaily.com/baidu-ernie-lightning-wizshot-me-micro-expression-video-models-qianfan>) — reporting. Checked: 12 Nov 2026, 16:04 CET

### AWS releases AWS Emulator, a free local copy of its cloud APIs written entirely by autonomous AI agents

*Coding & agents · New*

**Published:** 11 Nov 2026

Amazon Web Services released **AWS Emulator** on Wednesday 11 November, a free tool that imitates AWS services on a developer's own machine so applications can be tested offline. AWS engineer Matthew Goldberg writes that **every line of its code was written by autonomous agents** and that his team has not written or reviewed any of it. No earlier edition carried this release.

Goldberg says three teams of agents build it: one writes tests checked against the real AWS cloud, one finds discrepancies and one fixes them. The New Stack reports it covers **438 AWS API models across more than 200 services**, is written in Rust and runs on Linux, macOS and Windows without an AWS account. The code is on GitHub under the **CC0 public-domain licence**.

**Analysis — why it matters:** *Editorial analysis: AWS is shipping, and promising to maintain, a sizeable product with no human code review; **its bug backlog will show how well that holds**.*

**Caveat:** Fidelity to the real AWS services is AWS's claim. AWS's own guidance excludes some areas from testing, such as IAM and key policies, according to a Hacker News reader quoting the security page.

**Community reaction (opinion, not verified fact):**

> “Skeptical of using because it's not clear whether this was just an exercise or a real product they are going to ship and maintain.” — [CharlieDigital (Hacker News)](<https://news.ycombinator.com/item?id=50456723>)

> “This will make it even easier for competitors to reliably clone AWS services, which reveals that cloud is fully commoditized at this point” — [resters (Hacker News)](<https://news.ycombinator.com/item?id=50460482>)

**Sources:**

1. [About Amazon: How we built the agents that built AWS Emulator](<https://aboutamazon.com/news/aws/how-autonomous-ai-agents-built-aws-emulator>) — primary source. Checked: 12 Nov 2026, 16:05 CET
2. [The New Stack: AWS had its agents build a free and open emulator for AWS](<https://thenewstack.io/aws-emulator-ai-agents>) — reporting. Checked: 12 Nov 2026, 16:04 CET
3. [SiliconANGLE: Amazon's open-source AWS Emulator lets developers validate their code locally](<https://siliconangle.com/2026/11/11/amazons-open-source-aws-emulator-lets-developers-validate-their-code-locally-without-the-cloud>) — reporting. Checked: 12 Nov 2026, 16:04 CET
4. [Hacker News discussion: AWS emulator](<https://news.ycombinator.com/item?id=50456631>) — community. Checked: 12 Nov 2026, 16:05 CET

### UPDATE: Jensen Huang resigns as Nvidia's chief executive; CFO Colette Kress becomes interim CEO

*Industry & policy · Updated*

**Published:** 12 Nov 2026, 14:48 CET

Update to this morning's edition, which reported that Nvidia's board had met to decide whether to remove Jensen Huang. The new development: on Thursday 12 November Nvidia announced that **Huang has resigned as president, chief executive and director**, effective immediately. TechCrunch, citing a regulatory filing, reports that the board accepted his resignation on Wednesday.

**Colette Kress**, Nvidia's chief financial officer since 2013, becomes **interim chief executive** and keeps the finance job until a permanent successor is named. The board says it will consider internal and external candidates. It also named **Harvey C. Jones**, a former chief executive of Synopsys, as its first-ever chair.

In the company's statement, Jones said the board expects operations, customer commitments and the product roadmap to continue without interruption; Huang is not quoted. Nvidia says it will still report third-quarter results on **17 November** as planned.

The resignation follows Huang's admission on 8 November that he had been unfaithful to his wife, reports that US intelligence believes the woman involved, Alice Huang, was a Chinese intelligence asset, and The New York Times' report of a second relationship with an executive who reports to him. TechCrunch reports Nvidia shares were down more than 11% before the US market opened.

**Analysis — why it matters:** *Editorial analysis: Huang co-founded Nvidia in 1993 and ran it ever since; **a finance chief now leads the main supplier of AI chips** five days before its results and amid a national-security inquiry.*

**Caveat:** The intelligence allegation about Alice Huang is reported, not proven; Reuters says it could not verify it and China denies it. Share-price moves are pre-market figures reported by TechCrunch.

**Community reaction (opinion, not verified fact):**

> “My understanding is that NVidia's organisation is very flat and Huang has his fingers in every pie; he's not the hands off type. Moreover there was no succession plan.” — [skywal\_l (Hacker News)](<https://news.ycombinator.com/item?id=50467179>)

> “I don't know, I just have a feeling he'll be back. Steve Jobs style.” — [kilroy123 (Hacker News)](<https://news.ycombinator.com/item?id=50467202>)

**Sources:**

1. [NVIDIA Newsroom: NVIDIA Announces CEO Transition](<https://nvidianews.nvidia.com/news/nvidia-announces-ceo-transition>) — primary source. Checked: 12 Nov 2026, 16:02 CET
2. [TechCrunch: Nvidia's Jensen Huang resigns, chipmaker names CFO Colette Kress as interim CEO](<https://techcrunch.com/2026/11/12/nvidias-jensen-huang-resigns-chipmaker-names-cfo-colette-kress-as-interim-ceo/>) — reporting. Checked: 12 Nov 2026, 16:03 CET
3. [CNBC: Nvidia CEO Jensen Huang resigns, live updates](<https://www.cnbc.com/2026/11/12/nvidia-jensen-huang-ceo-live-updates.html>) — reporting. Checked: 12 Nov 2026, 16:03 CET
4. [Hacker News discussion: NVIDIA Announces CEO Transition](<https://news.ycombinator.com/item?id=50467087>) — community. Checked: 12 Nov 2026, 16:04 CET

### Chinese AI firms rush to rent Nvidia computing abroad, fearing the Huang scandal will close the remote-access route, Reuters reports

*Industry & policy · New*

**Published:** 12 Nov 2026

Chinese AI companies are trying to **rent Nvidia-powered computing capacity at data centres outside China**, three people familiar with the matter told Reuters in an exclusive report on 12 November. They fear the scandal around Jensen Huang could push Washington to restrict their remote use of advanced processors, which US export rules do not currently block.

According to the sources, a major Chinese cloud provider has discussed locking in overseas Nvidia capacity, some companies have contacted data-centre operators to reserve it, and smaller labs are looking at providers in Southeast Asia. The companies worry the affair adds momentum to the **Remote Access Security Act**, which passed the US House 369 to 22 in January and awaits the Senate.

Separately, Investing.com, summarising a report by The Information, says the **Commerce Department is preparing to finalise a rule** blocking Chinese firms' remote access to advanced AI chips through data centres in other countries, extending controls to seven more countries including Malaysia, Singapore and Thailand. Reuters reports that Alibaba shares fell as much as 7.1% in Hong Kong on Thursday.

**Analysis — why it matters:** *Editorial analysis: renting chips abroad has been the main legal way for Chinese labs to train on top Nvidia hardware; **closing it would cut that supply** at the moment Nvidia loses its chief executive.*

**Caveat:** Both reports rest on unnamed sources; no rule has been published, and Nvidia and the Commerce Department did not respond to Reuters. The Information's original article is paywalled and was not read.

**Sources:**

1. [Euronext (Reuters): Exclusive - Chinese AI firms rush to secure Nvidia chip capacity as spy scandal stirs fear of US curbs](<https://live.euronext.com/en/financial-news/exclusive-chinese-ai-firms-rush-secure-nvidia-chip-capacity-spy-scandal-stirs-fear>) — reporting. Checked: 12 Nov 2026, 16:03 CET
2. [Yahoo Finance (Investing.com): U.S. finalizing rule to block China's remote AI chip access - The Information](<https://finance.yahoo.com/technology/ai/articles/u-finalizing-rule-block-china-042215614.html>) — reporting. Checked: 12 Nov 2026, 16:05 CET

### Nebius revenue rises 571% to $981 million, but capacity delays push its 2026 revenue to the low end and spending rises to $27 billion

*Industry & policy · New*

**Published:** 12 Nov 2026

AI cloud company Nebius reported third-quarter revenue of **$980.8 million**, up 571% from a year earlier, with adjusted EBITDA of $465.8 million and a net loss from continuing operations of $37.5 million. It spent $7.3 billion on equipment and other assets in the quarter.

Reuters, via CNA, reports that Nebius now expects 2026 revenue at the **low end of its $3 billion to $3.4 billion range** because some third-party data-centre capacity slipped to the first half of 2027, and that it raised 2026 capital spending to **about $27 billion**, from $20 billion to $25 billion. For 2027 it forecasts $12 billion to $13 billion of revenue and $40 billion to $45 billion of spending, most of it to be covered by customer prepayments and asset-backed financing, Reuters reports. Its shares fell nearly 12% before the market opened.

**Analysis — why it matters:** *Editorial analysis: two days after CoreWeave raised its forecast, Nebius shows the other side of the build-out: **demand is there, but power and buildings arrive late**.*

**Caveat:** The 2026 low-end outlook and the $27 billion spending figure are as reported by Reuters and CNBC; Nebius's shareholder letter confirms the 2027 revenue range and the 75% to 85% financing coverage. Adjusted EBITDA is a non-GAAP measure.

**Sources:**

1. [Nebius: Nebius reports third quarter 2026 financial results](<https://nebius.com/newsroom/nebius-reports-third-quarter-2026-financial-results>) — primary source. Checked: 12 Nov 2026, 16:10 CET
2. [CNA (Reuters): Nebius pares back 2026 revenue forecast on capacity delays, shares slump](<https://www.channelnewsasia.com/business/nebius-pares-back-2026-revenue-forecast-capacity-delays-shares-slump-6546161>) — reporting. Checked: 12 Nov 2026, 16:05 CET
3. [CNBC: Nebius Q3 earnings report 2026](<https://www.cnbc.com/2026/11/12/nebius-q3-earnings-report-2026.html>) — reporting. Checked: 12 Nov 2026, 16:04 CET
4. [Nebius: Letter to shareholders, Q3 2026 (PDF)](<https://assets.nebius.com/assets/65994da2-e220-40cd-bb5d-72e9654a237d/Q3%202026%20SHL.pdf>) — primary source. Checked: 12 Nov 2026, 16:10 CET

### EU publishes binding rules for AI Act regulatory sandboxes, with free, priority access for small firms

*Industry & policy · New*

**Published:** 11 Nov 2026

The European Commission's **Implementing Regulation (EU) 2026/2487**, adopted on 10 November, was published in the EU's Official Journal on 11 November. It sets common rules for how national authorities set up and run AI regulatory sandboxes under the AI Act, where companies can develop and test AI systems under supervision before putting them on the market. EUR-Lex lists **1 December 2026** as its date of effect. No earlier edition carried it.

Small and medium-sized firms, including start-ups, get **priority and free access** to the authorities' guidance and supervision, though exceptional costs can be recovered; other companies can be charged full cost. Authorities must answer applications within three months, and every project ends with an exit report that other EU authorities must recognise as evidence of the work done.

The regulation states that taking part in a sandbox is **not an approval**: the exit report does not have the legal effect of a declaration of conformity.

**Analysis — why it matters:** *Editorial analysis: the rules replace a patchwork of national designs, but **a sandbox gives guidance, not a compliance pass**.*

**Caveat:** This is an implementing act under the existing AI Act, not new legislation. EUR-Lex marks its entry into force as pending notification.

**Sources:**

1. [EUR-Lex: Commission Implementing Regulation (EU) 2026/2487 on AI regulatory sandboxes](<https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=OJ:L_202602487>) — primary source. Checked: 12 Nov 2026, 16:05 CET

### France will create an international centre for military AI in Rennes, due to open in summer 2027

*Industry & policy · New*

**Published:** 12 Nov 2026

France's armed forces ministry said on 12 November that it will create an **international centre to support the use of AI in defence**, due to open in **summer 2027**, Reuters reports. An official told reporters the ministry hopes NATO will recognise the centre.

Reuters reports that funding and international members are not yet settled, and that other countries have been invited to a conference next week to hear the plans. A Presse Agence notice of 10 November announcing the briefing names the project the **International Center for AI in Defence (ICAID)** and places it in Rennes.

**Analysis — why it matters:** *Editorial analysis: Europe relies heavily on US suppliers such as Palantir for military AI software; **the centre is a bid to build that expertise at home**.*

**Caveat:** Funding, staffing and membership are not final; the ministry's own statement was not found online, so the details come from Reuters and Presse Agence. Ouest-France's article on the centre is paywalled and was not read.

**Sources:**

1. [KELO-FM (Reuters): French army ministry to set up centre for defence-related AI](<https://kelofm.com/2026/11/12/french-army-ministry-to-set-up-centre-for-defence-related-ai>) — reporting. Checked: 12 Nov 2026, 16:05 CET
2. [Presse Agence: IA de defense, le ministere des Armees annonce la creation d'un centre international a Rennes](<https://presseagence.fr/paris-ia-de-defense-le-ministere-des-armees-annonce-la-creation-dun-centre-international-a-rennes/>) — reporting. Checked: 12 Nov 2026, 16:06 CET

## Key patterns (editorial analysis)

- Nvidia's crisis is now an export-control story: **Huang is out**, and Chinese labs are racing to lock in offshore chips before rules tighten.
- AI infrastructure demand is not the constraint: Nebius **sold capacity it could not switch on in time**.
- Agents are now writing shipped products: AWS released an emulator **no human wrote or reviewed**.

## Source coverage

- Engine version: 3.31.0
- Engine ran this edition: yes
- Engine look-back: 2 days

### Source status

- reddit: ok, partial (18 threads; 45 sub-requests blocked with HTTP 403, 4 failed with HTTP 422; Arctic Shift archive supplied posts)
- hackernews: ok (26 stories)
- github: ok (11 items)
- devto: ok (12 articles; tags ai and llm)
- youtube: not searched (yt-dlp not available on this machine)
- polymarket: not used: blocked in France (ANJ)
- x: not searched (no consent-free source configured)

### Notes

- The installed last30days engine finished with 67 evidence items from Reddit, Hacker News, dev.to and GitHub; its top clusters were stories earlier editions had already carried. This edition's stories were found with 16 Google News RSS queries, publisher feeds, post-engine web supplements and the source pages. Community comments come from Hacker News threads read through its public API. Item counts are not counts of verified developments.
- Window widened: this edition's window starts at midnight on 11 November, about 40 hours before it was issued, to carry AWS Emulator and the EU sandbox regulation, both published on 11 November and not carried by an earlier edition.
- Polymarket not used: blocked in France (ANJ). X not searched. YouTube not searched (not available on this machine). Reddit returned results, but 45 of its sub-requests were blocked (HTTP 403) and 4 failed, so Reddit coverage was partial. Missing coverage does not mean nobody discussed these stories.
- Paywalled and not read: The Information's report on a Commerce Department rule for remote chip access (described through Investing.com's summary) and Ouest-France's article on the Rennes defence AI centre (the name and location come from Presse Agence instead). Reuters stories were read through syndicated copies on Euronext, CNA and KELO-FM.
- Newsletter leads from the Iris mail bot: today's file holds eight leads. Anthropic's IPO range, Fractile's round, the Chinese university's H200 purchase and Gemini 4 Carbon's pricing were covered by earlier editions; the other four (an approved H200 recipient's empty office, OpenAI's offline training, a KFC Japan item and ElevenLabs' Scribe v3) were either not new or not verified from readable primary sources and were not carried.
- Not carried: Notion's disclosure that Fireworks AI's breach exposed Notion AI chat transcripts, disclosed by 10 November and reported again by TechCrunch today; Proofpoint's $6.3 billion Varonis deal, announced on 15 October; OpenAI's ChatGPT Ads reseller deal with Aleph in 44 countries, a distribution agreement; and TSMC's approval of up to $1 billion of investment in Anthropic and OpenAI, covered on 10 November.
- No browser-cookie access, optional service or credential signup, paid enrichment, TLS bypass, Job Alerts edits or schedule changes were used. Research logs and full provenance remain private.

### Engine footer (verbatim)

```text
---
✅ All agents reported back!
├─ 🟠 Reddit: 18 threads │ 18,897 upvotes │ 3,471 comments
├─ 🟡 HN: 26 stories │ 2,397 points │ 1,735 comments
├─ 👩‍💻 dev.to: 12 articles │ 225 reactions │ 132 comments
├─ 🐙 GitHub: 11 items │ 55 reactions │ 206 comments
├─ 🗣️ Top voices: r/technology, r/LocalLLaMA, r/artificial
---
```
