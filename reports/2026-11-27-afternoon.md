# The AI Gazette — Afternoon edition, Friday 27 November 2026

*Models, machines, and matters of consequence*

- Issue: 2026-11-27-afternoon
- Issued: 27 Nov 2026, 16:09 CET (Paris)
- Reporting window: 26 Nov 2026, 10:55 CET to 27 Nov 2026, 16:07 CET
- Timezone: Europe/Paris
- Previous issue: 2026-11-27-morning
- Price: Complimentary

## Editor's note

A quiet Black Friday afternoon, led by the Nvidia affair: Bloomberg says filings place **Nvidia Blackwell racks at a Shanghai site** tied to Alice Huang. Poland has signed a **$300 million, five-year deal** for Palantir's battlefield AI, and Japan's government formally presented its plan to give its AI law penalties. In agents, a Papa John's AI agent paid for pizzas straight from a customer's bank account in a UK regulatory sandbox. In models, Russia's Sber opened the weights of GigaChat 4, a 708-billion-parameter model published on Thursday that no earlier edition carried, so the window was widened back to 10:55 on 26 November. In research, a cryptography preprint claims a deterministic subexponential discrete-logarithm algorithm built on OpenAI's October construction. There is **no new frontier model** from the large US labs. Two of the six stories are labelled updates.

## The News

### Russia's Sber opens the weights of GigaChat 4, a 708-billion-parameter model with a million-token context

*Models · New*

**Published:** 26 Nov 2026, 11:00 CET

Sber announced GigaChat 4 on Habr at 11:00 Paris time on Thursday 26 November, before this edition's normal window; no earlier edition carried it. It is two models: a **708-billion-parameter flagship** that activates about 41 billion parameters per token, released **under the MIT licence**, and a 37-billion-parameter model with about 4 billion active, released under a non-commercial licence for individuals.

Both have a context window of 1,048,576 tokens and switch per request between an instant mode and a reasoning mode, which GigaChat 3.5 split into separate checkpoints, according to the model card. The architecture mixes a mixture-of-experts design with Gated DeltaNet linear-attention layers and DeepSeek Sparse Attention. Weights are on Hugging Face in FP8, BF16, GGUF and base versions, with intermediate checkpoints.

In Sber's own tables, the flagship in reasoning mode scores **80.89% on SWE-bench Verified**, against 81.80% for DeepSeek V4 Flash and 86.67% for GLM-5.3, and 69.66% on Terminal-Bench 2.1, where GLM-5.3 scores 88.70%. It trails on GPQA Diamond, at 82.83% against 91.00% for DeepSeek V4 Flash.

**Analysis — why it matters:** *Analysis: a permissively licensed open-weight model at this scale from outside the US and China is rare; Sber's own figures put it near the leading Chinese open models on coding and behind them on harder reasoning tests.*

**Caveat:** All benchmark scores are **Sber's own, not independently checked**. The window was widened back to 10:55 on 26 November to carry this release.

**Sources:**

1. [Habr (Sber): GigaChat 4: новые агентные навыки и первый миллион](<https://habr.com/ru/companies/sberbank/articles/1112118>) — primary source. Checked: 27 Nov 2026, 16:06 CET
2. [Hugging Face: ai-sage/GigaChat4-708B-A41B model card](<https://huggingface.co/ai-sage/GigaChat4-708B-A41B>) — primary source. Checked: 27 Nov 2026, 16:06 CET
3. [Hugging Face: ai-sage/GigaChat4-37B-A4B model card](<https://huggingface.co/ai-sage/GigaChat4-37B-A4B>) — primary source. Checked: 27 Nov 2026, 16:06 CET
4. [Tproger: Как обучали GigaChat 4 и на каком железе запустить модель](<https://tproger.ru/articles/kak-obuchali-gigachat-4-i-na-kakom-zheleze-zapustit-model>) — reporting. Checked: 27 Nov 2026, 16:06 CET

### A Papa John's AI agent pays for pizzas straight from a customer's bank account in a UK regulatory sandbox, TrueLayer says

*Coding & agents · New*

**Published:** 27 Nov 2026

TrueLayer, a London payments company, says a Papa John's AI agent completed the **first agentic Pay by Bank payment** to a named UK retailer, working with Lloyds inside the Financial Conduct Authority's Supercharged Sandbox. TrueLayer presented the findings at the regulator's showcase on 26 November.

According to TrueLayer's announcement, the agent helps with the order and then pays from the bank account the customer has linked to their Papa John's account. The customer sets a **spending limit with their bank** that no agent can exceed, the bank declines anything above it, and authorisation happens in the customer's banking app, so no credentials are shared with the agent. It was also the first use of Lloyds' variable recurring payment interfaces for agent payments, TrueLayer says.

The Guardian reports the order was **nine mini margherita pizzas** for a real customer. TrueLayer's chief executive, Francesco Simoneschi, told BBC Radio 4 that 'This is possibly the last Black Friday as we know it', and said existing buyers' rights would still apply if an agent ordered the wrong product.

**Analysis — why it matters:** *Analysis: most agent shopping so far runs on cards; a bank-held mandate with hard limits is a different safety model, in which the bank rather than the agent enforces the spending cap.*

**Caveat:** A single supervised **sandbox pilot, not a consumer launch**. The 'first' claims are TrueLayer's; no price, launch date or customer numbers were given.

**Community reaction (opinion, not verified fact):**

> “Wait, so how was the purchase made without any credentials?” — [Tajnymag on Hacker News](<https://news.ycombinator.com/item?id=50666605>)

> “Unattended payment is too scary for me.” — [LelouBil on Hacker News](<https://news.ycombinator.com/item?id=50667360>)

**Sources:**

1. [Open Banking Expo (TrueLayer press release): Papa John's and TrueLayer partner with Lloyds to complete UK's first agentic Pay by Bank payment](<https://www.openbankingexpo.com/news/papa-johns-and-truelayer-partner-with-lloyds-to-complete-uks-first-agentic-pay-by-bank-payment>) — primary source. Checked: 27 Nov 2026, 16:06 CET
2. [The Guardian: Pizza history: AI agent's cardless purchase is a first for UK](<https://www.theguardian.com/business/2026/nov/27/ai-agent-cardless-transaction-pizza-papa-john-uk-fca-truelayer>) — reporting. Checked: 27 Nov 2026, 16:06 CET
3. [Hacker News: Tajnymag](<https://news.ycombinator.com/item?id=50666605>) — community. Checked: 27 Nov 2026, 16:06 CET
4. [Hacker News: LelouBil](<https://news.ycombinator.com/item?id=50667360>) — community. Checked: 27 Nov 2026, 16:06 CET

### Cryptography preprint claims a deterministic subexponential discrete-logarithm algorithm, building on OpenAI's October construction

*Research · New*

**Published:** 27 Nov 2026

A paper by Shuchang Liu, Bingsheng Zhang and Kui Ren, approved on the IACR Cryptology ePrint Archive on Friday, claims **a deterministic algorithm that solves the discrete logarithm problem in subexponential time**, both in prime fields and on prime-order elliptic curves, using no random bits and without the Generalized Riemann Hypothesis.

The result is conditional: the abstract says it holds **assuming the Cauchy–Hermite Boolean tensor contraction construction of OpenAI (October 2026)**, and it builds on the October refutations of the Exponential Time Hypothesis, which this journal covered on 27 October, and on later randomised subexponential algorithms for elliptic curves. The claimed running time is 2 to the power O(b divided by the square root of log log b) for b-bit primes.

Commenters on Hacker News argued the result is unlikely to matter in practice: randomised subexponential algorithms for the discrete logarithm have existed for decades, and the bound beats the standard baby-step giant-step attack only for very large keys.

**Analysis — why it matters:** *Analysis: the paper is a sign that the AI-produced complexity results of October are now being used as building blocks by human cryptographers, which is the kind of downstream effect the Bank of England governor and others have been warning about.*

**Caveat:** A **preprint, not peer reviewed**, read only through its abstract (the PDF sat behind a bot check), and conditional on a construction this journal has not verified. Community comments are opinions, not proof of the practical impact.

**Community reaction (opinion, not verified fact):**

> “The present deterministic algorithm is highly unlikely to have practical consequences for cryptographic protocols in use.” — [layer8 on Hacker News](<https://news.ycombinator.com/item?id=50666238>)

> “This result does not matter practically for cybersecurity.” — [pcstl on Hacker News](<https://news.ycombinator.com/item?id=50666560>)

**Sources:**

1. [IACR Cryptology ePrint Archive: Paper 2026/3020](<https://eprint.iacr.org/2026/3020>) — primary source. Checked: 27 Nov 2026, 16:06 CET
2. [Hacker News discussion](<https://news.ycombinator.com/item?id=50665968>) — community. Checked: 27 Nov 2026, 16:06 CET
3. [Hacker News: layer8](<https://news.ycombinator.com/item?id=50666238>) — community. Checked: 27 Nov 2026, 16:06 CET
4. [Hacker News: pcstl](<https://news.ycombinator.com/item?id=50666560>) — community. Checked: 27 Nov 2026, 16:06 CET

### UPDATE: Filings place Nvidia Blackwell racks at a Shanghai data centre tied to Alice Huang, Bloomberg reports

*Industry & policy · Updated*

**Published:** 27 Nov 2026

Update to the 13 November afternoon edition, which reported Bloomberg tracing banned Nvidia Hopper servers to a Shanghai data centre linked to Alice Huang, and to the 26 November morning edition's report on S&P's credit watch. The new development: Bloomberg reported on Friday that documents filed with Chinese regulators show **Blackwell-based hardware installed at the Yangtze River Delta Project** in Shanghai, according to Investing.com's account of the report.

According to that account, a company called Shanghai Shuoyao pledged a **GB300 NVL72 rack** as collateral for a 96 million yuan ($14 million) loan from Shanghai Innovation Bank, and a second company, Shanghai Kezhan, listed a GB200 server at the same site in documents for a 90 million yuan loan from a finance-leasing company owned by a Shanghai government agency. Bloomberg matched the rack's serial number, through a public warranty database, to a rack built by Taiwan's Gigabyte.

Blackwell chips have always needed a US export licence to ship to China. Shanghai Shuoyao has said it is a service provider to Megaspeed, the Singapore company Alice Huang founded in 2023, and called the relationship 'limited to ordinary commercial cooperation'. Megaspeed, which the US added to its Entity List this month, has denied wrongdoing. Seeking Alpha's summary says Bloomberg described Shanghai Kezhan's loan as dating from late 2025.

**Analysis — why it matters:** *Analysis: earlier reporting in this affair concerned older Hopper-generation servers; filings that place Nvidia's newest rack-scale systems inside a Chinese facility would bear directly on how well the export rules and Nvidia's partner checks work, ahead of Jensen Huang's Senate testimony on 3 December.*

**Caveat:** Bloomberg's report is paywalled and was **not read directly**; this story rests on Investing.com's and Seeking Alpha's summaries of it. How the hardware reached the site, and whether Megaspeed had any role in shipping it, is not established in those summaries.

**Sources:**

1. [Yahoo Finance (Investing.com): Nvidia Blackwell chips found in Shanghai data center tied to Alice Huang](<https://finance.yahoo.com/technology/ai/articles/nvidia-blackwell-chips-found-shanghai-124008621.html>) — reporting. Checked: 27 Nov 2026, 16:06 CET
2. [TradingView (Seeking Alpha): Nvidia Blackwell chips found at China data center linked to Alice Huang](<https://www.tradingview.com/news/seekingalpha:b53a51d8e094b:0-nvidia-blackwell-chips-found-at-china-data-center-linked-to-alice-huang-report>) — reporting. Checked: 27 Nov 2026, 16:06 CET

### Poland signs a five-year deal worth about $300 million for Palantir's AI battlefield decision software

*Industry & policy · New*

**Published:** 27 Nov 2026

Poland's defence ministry signed an agreement with Palantir on Friday worth **around $300 million over five years** for software that uses artificial intelligence to support army commanders' decisions, Defence Minister Wladyslaw Kosiniak-Kamysz said, Reuters reported.

Polska Zbrojna, the defence ministry's magazine, said ahead of the signing that the product is Palantir's **Maven Smart System**, to run in Poland under the codename Saturn. It combines data from drones, satellites, radars and reconnaissance systems into a shared picture of the battlefield, and uses AI to analyse it, detect and classify objects and help with target designation. The magazine says US forces use Maven and NATO is deploying its own version.

Kosiniak-Kamysz called the deal 'a watershed moment' for the armed forces and said: 'All keys, servers, and information are — and will remain — the exclusive property of the Polish Armed Forces.' Poland signed a memorandum with Palantir in 2025, according to Reuters; Polska Zbrojna dates a cooperation agreement on cybersecurity and IT to December 2024 and a letter of intent to October 2025.

**Analysis — why it matters:** *Analysis: the deal is one of the larger European purchases of US military AI software at a time when some European governments want to rely less on US technology for critical defence functions, which is why the minister stressed data and key ownership.*

**Caveat:** The **$300 million value and five-year term** come from the minister; the contract text has not been published. The two sources date the start of the cooperation differently; both are given.

**Sources:**

1. [Reuters, via Global Banking and Finance Review: Poland signs $300M Palantir AI defence contract over five years](<https://www.globalbankingandfinance.com/poland-signs-contract-palantir-worth-300-million-over-5>) — reporting. Checked: 27 Nov 2026, 16:06 CET
2. [Polska Zbrojna (Polish defence ministry magazine): Saturn dla wojska. MON podpisze umowę z Palantirem](<https://polska-zbrojna.pl/Mobile/articleshow/47674>) — primary source. Checked: 27 Nov 2026, 16:09 CET

### UPDATE: Japan's government presents its outline for giving the AI law penalties, and an expert panel broadly approves it

*Industry & policy · Updated*

**Published:** 27 Nov 2026

Update to this morning's story, which carried Nikkei's and Yomiuri's reports that Japan was drafting the amendment. The new development: on Friday a government AI strategy panel **formally outlined the draft bill**, Jiji Press reported, and according to BigGo Finance's report the plan **received broad approval** at the expert meeting the same day.

The outline obliges providers of advanced AI services to take measures against cyberattacks, Jiji says, with OpenAI and Anthropic apparently in mind. BigGo Finance's account adds that providers would have to report incidents and defects that could be exploited in cyberattacks, that the government could carry out on-site inspections and issue orders after recommendations are ignored, and that violating orders would carry penalties whose details are still to be worked out.

The government aims to finalise the bill early and submit it to the Diet, Jiji says; BigGo Finance names next year's ordinary Diet session. The current law, enacted in May 2025, lets the government investigate AI providers and give guidance, but answering is voluntary.

**Analysis — why it matters:** *Analysis: the plan moved from leaked press accounts to an outline presented by the government itself, which makes mandatory incident reporting for the largest foreign AI providers in Japan considerably more likely.*

**Caveat:** This is an outline, **not bill text**, and the size of any fine has not been set officially; this morning's 100 million yen figure came from press reports. BigGo Finance does not name its own source.

**Sources:**

1. [Nippon.com (Jiji Press): Japan to Revise AI Law to Introduce Penalties](<https://www.nippon.com/en/articles/-/58131>) — reporting. Checked: 27 Nov 2026, 16:06 CET
2. [BigGo Finance: Japan to Mandate Safety Measures and Incident Reporting for Advanced AI Providers](<https://finance.biggo.com/news/dfd711c3-71b5-4997-8c73-abb9a4baaba7>) — reporting. Checked: 27 Nov 2026, 16:06 CET

## Key patterns (editorial analysis)

- The Nvidia affair has moved from people to hardware: filings now place **Blackwell rack-scale systems** inside a Chinese facility tied to Alice Huang.
- Governments are buying and regulating AI at the same time: Poland bought Palantir's battlefield software while Japan moved to make frontier providers **report incidents under penalty**.
- Agent commerce is being built around limits set outside the agent, with the bank enforcing the spending cap in the TrueLayer pilot.

## Source coverage

- Engine version: 4.6.0
- Engine ran this edition: yes
- Engine look-back: 2 days

### Source status

- reddit: ok, partial (22 threads; Reddit blocked direct requests with HTTP 403; the Arctic Shift archive supplied posts)
- hackernews: ok (23 stories)
- github: ok (4 items)
- devto: ok (12 articles; tags ai and llm)
- youtube: not searched (yt-dlp not available on this machine)
- polymarket: not used: blocked in France (ANJ)
- x: not searched (no consent-free source configured)

### Notes

- The installed last30days engine (4.6.0) finished (exit 0) with evidence from Reddit, Hacker News, dev.to and GitHub. Its top clusters were mostly commentary, older items or community posts (an AI group-chat parody, Google's Workspace agent rules, a DeepMind podcast); of this edition's stories only the Papa John's payment appeared among them. The others were found through a Hacker News scan of the window, Google News RSS queries, publisher feeds, post-engine web supplements and the source pages. Item counts are not counts of verified developments.
- Polymarket not used: blocked in France (ANJ). X not searched. YouTube not searched (not available on this machine). Reddit returned results only through the Arctic Shift archive, because Reddit blocked direct requests (HTTP 403), so Reddit coverage was partial. VentureBeat's feed answered HTTP 429 and DeepMind's feed did not parse. Missing coverage does not mean nobody discussed these stories.
- Window: the normal window opens at the previous edition's issue time, 06:10 on 27 November. It was widened to 10:55 on 26 November (within 48 hours) to carry Sber's GigaChat 4 release, published at 11:00 that day, which no earlier edition carried. Everything else in the widened window followed the editorial gate, and stories earlier editions carried were not repeated.
- Not read: Bloomberg reports on the Shanghai Blackwell hardware and Poland's Palantir deal are paywalled; the Nvidia story rests on Investing.com's and Seeking Alpha's summaries, the Poland story on a Reuters copy and the defence ministry's magazine. Nikkei's report on Japan's outline is for members and was not used.
- Routes: The Guardian refused plain requests (HTTP 403) and was read through scripts/fetch\_source.py's direct route; BigGo Finance refused plain requests (HTTP 403) and was read through web extraction. The ePrint PDF sat behind a Cloudflare bot check, so only the abstract page was read. The host's web extraction tool hit its daily limit late in the run.
- Newsletter leads from the Iris mail bot: today's file holds five leads. OpenAI's GPT-6.2 billing fix ran this morning. FinCEN's cyber incident (24 November), Anthropic's study of 58 companies (23 November), the reported SpaceX and Tesla merger talks (first reported 25 November and not an AI development) and Amazon's Black Friday ads in ChatGPT while blocking OpenAI's crawlers (Digiday, 24 November) all fall more than 48 hours before this edition, so none was carried.
- Considered and not carried: Moonshot's Kimi for Science credit programme (26 November, minor); Singapore's remarks on chip talks with the US (the same remarks this morning's edition reported); New York's ban on AI chatbot toys (signed 24 November); the FCC's approval of SpaceX's orbital data centres (25 November).
- Also not carried: a reported SpaceX cut to Blackwell rental prices (SemiAnalysis via secondary summaries, 26 November); DeepSeek's test of a per-conversation cost display (user reports only, no DeepSeek statement); and viral X claims that Claude sabotages machine-learning research (24 to 25 November; X not cited).
- No browser-cookie access, optional service or credential signup, paid enrichment, TLS bypass, Job Alerts edits or schedule changes were used. Research logs and full provenance remain private.

### Engine footer (verbatim)

```text
---
✅ All agents reported back!
├─ 🟠 Reddit: 22 threads │ 3,922 upvotes │ 6,050 comments
├─ 🟡 HN: 23 stories │ 2,373 points │ 1,376 comments
├─ 👩‍💻 dev.to: 12 articles │ 330 reactions │ 340 comments
├─ 🐙 GitHub: 4 items │ 12 reactions │ 44 comments
├─ 🗣️ Top voices: r/singularity, r/artificial, r/technology
---
```
