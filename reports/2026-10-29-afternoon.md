# The AI Gazette — Afternoon edition, Thursday 29 October 2026

*Models, machines, and matters of consequence*

- Issue: 2026-10-29-afternoon
- Issued: 29 Oct 2026, 16:07 CET (Paris)
- Reporting window: 29 Oct 2026, 06:08 CET to 29 Oct 2026, 16:06 CET
- Timezone: Europe/Paris
- Previous issue: 2026-10-29-morning
- Price: Complimentary

## Editor's note

This edition has **five new stories** since this morning's 06:08 issue, and no updates. Mistral put its trillion-parameter Le Chonk model on open download, Deepgram bought the company behind Pipecat, and the AI build-out met its money test: **Alphabet shares fell sharply** on its cash outflow while Microsoft went to the bond market. No new research result cleared the bar this afternoon.

## The News

### Mistral releases the weights of Mistral Large 4, its 1-trillion-parameter 'Le Chonk' model, and pitches it at cyber defenders

*Models · New*

**Published:** 29 Oct 2026, 13:00 CET

Mistral on 29 October published the weights of an improved **Mistral Large 4**, nicknamed Le Chonk, which it first offered as a public preview earlier this month. Mistral describes it as a **1-trillion-parameter**, natively multimodal model trained from scratch in its own European data centres. The weights are on Hugging Face, and the model is also offered through Mistral's API and OpenRouter.

Mistral says three more weeks of reinforcement learning made it the strongest open-weight coding model. It reports 48% on the Artificial Analysis Coding Agent Index, level with Zhipu's GLM-5.3 while using 47% fewer tokens per task, and 41% on Terminal-Bench 4.0. On security, it reports **51% on the Artificial Analysis Cyber Index** and a 96.6% average refusal rate on malicious cyber prompts.

The licence is a modified MIT licence: use, fine-tuning and commercial use are free, but **companies selling the model as a service need a separate licence**. API pricing is **$0.70 per million input tokens and $2.10 per million output tokens**. Mistral also says enterprise partners such as Orange Cyberdefense get preview access to a specialised variant for penetration testing and red-teaming, under vetting and contracts.

**Analysis — why it matters:** *Analysis: A day after Google limited its strongest cyber model to vetted defenders, Mistral has put a model with similar aims on public download. Defenders gain a model they can run on their own systems, and anyone else can download it too.*

**Caveat:** The benchmark figures and refusal rates are **reported by Mistral**. Mistral itself says it saw **potential for uplift to conduct real attacks** in preview traffic and is tightening its guardrails.

**Community reaction (opinion, not verified fact):**

> “It's not open weight, it's weights available as they use a modified MIT license that is not OSI.” — [rcr-anti (Hacker News)](<https://news.ycombinator.com/item?id=50289652>)

> “Unrelated to Large 4, but why is it so hard to give money to Mistral?” — [tokai (Hacker News)](<https://news.ycombinator.com/item?id=50289584>)

**Sources:**

1. [Mistral: Mistral Large 4 (Le Chonk) is now open weight](<https://mistral.ai/news/mistral-large-4-oss/>) — primary source. Checked: 29 Oct 2026, 16:03 CET
2. [Hugging Face blog](<https://huggingface.co/blog/mistral-large4>) — reporting. Checked: 29 Oct 2026, 16:03 CET
3. [WIRED](<https://www.wired.com/story/mistral-says-le-chonk-surpasses-chinese-models-cybersecurity/>) — reporting. Checked: 29 Oct 2026, 16:03 CET
4. [Euronews](<https://www.euronews.com/2026/10/29/mistral-releases-latest-ai-model-for-download-giving-companies-more-control-over-their-cyb>) — reporting. Checked: 29 Oct 2026, 16:03 CET
5. [Hacker News discussion](<https://news.ycombinator.com/item?id=50289418>) — community. Checked: 29 Oct 2026, 16:06 CET

### Deepgram buys Daily, maker of the open-source Pipecat voice-agent framework, and promises an independent Pipecat Foundation

*Coding & agents · New*

**Published:** 29 Oct 2026, 14:00 CET

Speech-AI company **Deepgram is acquiring Daily**, the company behind **Pipecat**, a widely used open-source framework for building voice agents, the two companies announced on 29 October. Terms were not disclosed. Daily also runs real-time audio and video network infrastructure, and its team is joining Deepgram.

Both companies say Pipecat will stay open source under its existing BSD licence and vendor-neutral. They are setting up an **independent Pipecat Foundation** which, according to Daily, will be run by a steering committee that includes companies competing with Deepgram.

At its first Speak conference, Deepgram also introduced the **Real-Time Context Standard**, an open protocol written with the Pipecat team. It carries cues such as a whisper or an unclear word from one model to the next, so that a voice agent can ask for clarification or match its tone.

**Analysis — why it matters:** *Analysis: Voice agents are assembled from separate speech, language and voice models. Owning the most popular open framework that joins them gives Deepgram a central place in that stack, which is why the neutrality promises matter to rivals.*

**Caveat:** The foundation's governance has been announced but **not yet published in detail**.

**Sources:**

1. [Deepgram announcement](<https://deepgram.com/blog/daily-pipecat-deepgram>) — primary source. Checked: 29 Oct 2026, 16:05 CET
2. [Daily blog](<https://www.daily.co/blog/deepgram-is-acquiring-daily-and-establishing-an-independent-pipecat-foundation/>) — primary source. Checked: 29 Oct 2026, 16:05 CET
3. [TechCrunch](<https://techcrunch.com/2026/10/29/deepgram-acquires-pipecat-maker-daily-to-bolster-its-voice-ai-infrastructure/>) — reporting. Checked: 29 Oct 2026, 16:03 CET

### Alphabet shares fall 13% in early trading after its AI build-out pushes quarterly free cash flow to minus $9.07 billion

*Industry & policy · New*

**Published:** 29 Oct 2026, 09:35 CET

Alphabet shares fell **13% in early New York trading** on Thursday 29 October, CNBC reported, after third-quarter results released after the market closed on Wednesday. CNBC noted that a close more than 9.77% lower would be the company's worst reaction to earnings since it went public in 2004.

Revenue grew 25% to $127.58 billion but missed analysts' forecasts, as did adjusted earnings of $2.67 a share. Free cash flow was **minus $9.07 billion**, against the minus $2.70 billion analysts expected. Capital spending reached $51.36 billion in the quarter, and Alphabet kept its 2026 forecast of **$195 billion to $205 billion**, saying spending will increase significantly in 2027.

Search advertising grew 12% to $63.35 billion, below expectations. On the earnings call, business chief Philipp Schindler said the growth of AI Mode queries had an impact because they currently earn less than traditional search. Google Cloud revenue more than doubled to $30.7 billion, according to The Decoder.

Microsoft, which also reported on Wednesday, was little changed. Its capital spending including finance leases was $45.2 billion, below forecasts, and its free cash flow stayed positive at $18.63 billion.

**Analysis — why it matters:** *Analysis: Investors are now judging the AI build-out by cash, not only by growth. Alphabet's cloud business is growing fast, but the market punished a quarter in which **spending outran the cash coming in**.*

**Caveat:** Share moves were changing during the trading day; the 13% figure is CNBC's early-trading number, **not a closing price**.

**Sources:**

1. [CNBC: Alphabet stock drops while Microsoft rises](<https://www.cnbc.com/2026/10/29/alphabet-google-microsoft-msft-shares-today-earnings.html>) — reporting. Checked: 29 Oct 2026, 16:05 CET
2. [CNBC: Alphabet Q3 2026 earnings](<https://www.cnbc.com/2026/10/28/alphabet-googl-earnings-q3-2026.html>) — reporting. Checked: 29 Oct 2026, 16:05 CET
3. [The Decoder](<https://the-decoder.com/googles-ai-search-problem-finally-shows-up-in-the-earnings-report-some-investors-believe/>) — reporting. Checked: 29 Oct 2026, 16:03 CET

### Microsoft returns to the US bond market for the first time since 2017, seeking at least $25 billion as AI spending climbs

*Industry & policy · New*

**Published:** 29 Oct 2026, 12:47 CET

Microsoft is selling **at least $25 billion of bonds** in its first US high-grade debt sale since 2017, Bloomberg reported on 29 October, citing a person with knowledge of the matter. The deal has as many as 10 parts, with maturities from 2 to 40 years; Wells Fargo, JPMorgan Chase and UBS are managing it, according to The Next Web.

Microsoft last raised $17 billion in a US bond sale in January 2017. It is one of only two US companies with a AAA credit rating. The sale follows results in which Microsoft's spending on data centres and equipment, including leases, reached **$45.2 billion in the quarter** to September and free cash flow fell 27%. Chief financial officer Amy Hood told analysts: 'We still have demand that exceeds supply.'

**Analysis — why it matters:** *Analysis: Even the companies with the most cash are now **borrowing to pay for AI data centres**. Alphabet and Amazon each raised $25 billion in bond sales earlier this year, according to The Next Web.*

**Caveat:** The size and terms come from **unnamed people** quoted by Bloomberg; the final amount depends on investor demand and had not been announced at the time of writing.

**Sources:**

1. [Bloomberg (paywalled; listing only)](<https://www.bloomberg.com/news/articles/2026-10-29/microsoft-kicks-off-first-us-high-grade-bond-sale-since-2017>) — reporting. Checked: 29 Oct 2026, 16:05 CET
2. [The Next Web](<https://thenextweb.com/news/microsoft-25-billion-bond-sale-first-since-2017>) — reporting. Checked: 29 Oct 2026, 16:05 CET

### New York Times: US officials concluded that an executive close to Nvidia's Jensen Huang was a Chinese intelligence asset

*Industry & policy · New*

**Published:** 29 Oct 2026

US intelligence agencies concluded that **Alice Huang (Huang Le)**, a Chinese citizen and senior executive at the Singapore-based data-centre company Megaspeed, was passing information to Beijing, The New York Times reported on 29 October, citing people briefed on classified surveillance. The surveillance showed she had developed a close relationship with **Nvidia chief executive Jensen Huang**.

According to the report, as summarised by The Decoder, President Trump was **briefed about a year ago and took no action**, and Jensen Huang was not warned; officials believed he was unaware. US authorities already suspected Megaspeed of helping Chinese companies obtain Nvidia chips, and the Times reports that a Malaysian sister company bought at least $4.8 billion of AI hardware with Nvidia chips between June 2024 and February 2026.

Nvidia told The Verge she is one of the thousands of customer executives Huang meets each year, and said Megaspeed does not receive sensitive information. Megaspeed has announced an internal investigation, and the Chinese embassy called the allegations groundless smears.

**Analysis — why it matters:** *Analysis: The report adds a security question to the arguments over how Nvidia's chips reach China, at a time when the company already faces a Justice Department inquiry into its Hugging Face purchase.*

**Caveat:** The account rests on **anonymous sources describing classified intelligence**. It does not accuse Jensen Huang of wrongdoing, and the Times article itself could not be read by this journal.

**Sources:**

1. [The New York Times (paywalled; listing only)](<https://www.nytimes.com/2026/10/29/us/politics/nvidia-china-jensen-huang-trump.html>) — reporting. Checked: 29 Oct 2026, 16:05 CET
2. [The Verge](<https://www.theverge.com/tech/1022060/jensen-huang-and-the-ai-spies>) — reporting. Checked: 29 Oct 2026, 16:05 CET
3. [The Decoder](<https://the-decoder.com/chinese-spies-targeted-nvidia-ceo-jensen-huang-according-to-the-new-york-times/>) — reporting. Checked: 29 Oct 2026, 16:03 CET

## Key patterns (editorial analysis)

- The AI build-out is now being judged by cash: **Alphabet was punished** for negative free cash flow, while Microsoft chose to borrow.
- Cyber-capable models are reaching defenders by two routes: Google keeps Gemini 4 Carbon gated, while **Mistral published Large 4's weights** with its own guardrails.
- Nvidia faces scrutiny on more than one front, from the Justice Department's Hugging Face questions to a reported spy case close to its chief executive.

## Source coverage

- Engine version: 3.28.0
- Engine ran this edition: yes
- Engine look-back: 2 days

### Source status

- reddit: ok (21 threads)
- youtube: ok (2 videos, 1 with a transcript; transcript requests for the other hit HTTP 429)
- hackernews: ok (19 stories)
- polymarket: unreachable (TLS certificate hostname mismatch; not bypassed)
- github: ok (12 items)
- devto: searched with tags ai and llm; 0 articles returned
- x: not searched (no consent-free source configured)

### Notes

- The window runs from this morning's 06:08 CET issue to this edition. Dispatches with only a date carry that date; exact timestamps are given where a source supplied one.
- The installed last30days engine finished with 54 evidence items from Reddit, Hacker News, GitHub and YouTube. Its top item was the Hacker News thread on Mistral Large 4, which supplied the community quotes; most other items were general discussion and videos about an 'AI bubble'. Stories were chosen with Google News RSS, publisher feeds, web searches and checks of primary documents. Item counts are not counts of verified developments.
- Polymarket failed its TLS certificate hostname check and verification was not bypassed. X was not searched. dev.to returned no articles. One YouTube transcript request hit HTTP 429. Failed or missing coverage does not mean nobody discussed these stories.
- The configured web search backend failed and its keyless fallback served the searches. Bloomberg, The New York Times, AP and Orange Cyberdefense refused automated access (HTTP 403), so the Microsoft bond and Huang dispatches rely on pages that could be fetched (The Next Web, The Verge, The Decoder) together with those publishers' text as returned by web search. VentureBeat returned HTTP 429.
- Not carried: Amazon's memo against 'tokenmaxxing' (27 October), Anthropic's purchase of Mithril Medicine (disclosed 27 October), Block's Dessa speech model (23 October), Canadian banks' blocks on personal AI agents (RBC covered on 28 October; the other banks' statements also date from 28 October), new commentary on the exponential time hypothesis proofs (covered on 27 October), and The Information's follow-up on GPT-6 Astra distillation, which adds no company confirmation.
- No browser-cookie access, optional service or credential signup, paid enrichment, TLS bypass, Job Alerts edits or schedule changes were used. Research logs and full provenance remain private.

### Engine footer (verbatim)

```text
---
✅ All agents reported back!
├─ 🟠 Reddit: 21 threads │ 591 upvotes │ 224 comments
├─ 🔴 YouTube: 2 videos │ 1,674,623 views │ 1/2 with transcripts
├─ 🟡 HN: 19 stories │ 944 points │ 602 comments
├─ 🐙 GitHub: 12 items │ 9 reactions │ 20 comments
├─ 🗣️ Top voices: r/artificial, r/OpenAI, r/MistralAI
---
```
