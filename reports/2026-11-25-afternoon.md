# The AI Gazette — Afternoon edition, Wednesday 25 November 2026

*Models, machines, and matters of consequence*

- Issue: 2026-11-25-afternoon
- Issued: 25 Nov 2026, 16:08 CET (Paris)
- Reporting window: 24 Nov 2026, 19:00 CET to 25 Nov 2026, 16:08 CET
- Timezone: Europe/Paris
- Previous issue: 2026-11-25-morning
- Price: Complimentary

## Editor's note

Google Research posted six papers its Cogentic agent system wrote on Gemini 4, led by a claimed **unconditional factoring algorithm in L\[1/3\] time**; no outside reviewer has checked them and Google says it has nothing to do with breaking encryption in practice. Amazon and Meta are reported to be **talking about ending Amazon's Muse block**, AI shares fell for a second day before the New York open, Fujitsu joined OpenAI's cyber-defence partner programme, KRAFTON released its own open-weight model and Japan set out an AI-power goal. There is **no new frontier model**. The window starts at 19:00 on Tuesday, before the previous issue time, to include KRAFTON's model, which no edition carried.

## The News

### KRAFTON releases Raon-1 mini, a 28.8-billion-parameter open-weight model it trained from scratch, under Apache 2.0

*Models · New*

**Published:** 24 Nov 2026

KRAFTON, the South Korean games company behind PUBG, took its in-house language model **Raon-1 mini** out of preview on Tuesday 24 November and published the weights on Hugging Face under the **Apache 2.0 licence**. No earlier edition carried it.

The model card describes a mixture-of-experts model with **28.8 billion parameters, 4.3 billion active** per token, designed and trained from scratch by KRAFTON AI, with a 262,144-token context and its own linear-attention variant. Users can pick one of six reasoning-effort levels, from none to max.

On KRAFTON's own benchmark table, Raon-1 mini scores 64.9 on MultiChallenge (59.0 for the preview), 55.9 on BrowseComp Plus and 72.3 on GDPVal, the best among the similar-sized mixture-of-experts models it compares. Seoul Economic Daily reports that KRAFTON plans a larger Raon-1 and a full-duplex voice model.

**Analysis — why it matters:** *Analysis: a games publisher training a competitive model from scratch adds to the small set of **non-US, non-Chinese open-weight models** that companies can run themselves.*

**Caveat:** All scores are **KRAFTON's own** and unverified; on the same table the dense Qwen3.8 27B, shown for reference, scores higher on GDPVal (74.3). The window was widened to include this release.

**Sources:**

1. [Hugging Face: KRAFTON/Raon-1-mini model card](<https://huggingface.co/KRAFTON/Raon-1-mini>) — primary source. Checked: 25 Nov 2026, 16:06 CET
2. [Seoul Economic Daily: Krafton unveils in-house LLM Raon-1 Mini](<https://en.sedaily.com/business/2026/11/25/krafton-unveils-in-house-llm-raon-1-mini-pushes-commercial>) — reporting. Checked: 25 Nov 2026, 16:06 CET

### Google Research posts six papers written by its Cogentic agents on Gemini 4, including a claimed proof that any integer can be factored in number-field-sieve time

*Research · New*

**Published:** 25 Nov 2026, 11:21 CET

Google Research added **six new papers** to the Cogentic folder of its public google-research repository on GitHub on Wednesday; the commit was pushed at 11:21 Paris time. Each paper says it was **entirely obtained by Cogentic**, an agent framework for mathematical discovery using Gemini 4 as its base model, with no human interaction other than the initial prompt to generate a full proof. Cogentic was described in a September arXiv preprint as a multi-agent harness for automated proof discovery; the folder now lists ten papers, the first dated 30 October.

The lead paper claims a zero-error randomised algorithm that computes the complete prime factorisation of any integer N in worst-case expected time **L\_N\[1/3, 105\]**, relying on no unproven hypotheses. Its abstract says this improves on the rigorous L\_N\[1/2, 1\] bound of Lenstra and Pomerance from 1992 and matches the exponent of the heuristic General Number Field Sieve, the fastest practical method, whose running time has never been proved.

The other five claim: a deterministic subexponential factoring algorithm; discrete logarithms in finite fields of fixed small characteristic in **sub-quasi-polynomial time**; a communication-complexity bound of O(r^(1/2 - epsilon)) with epsilon of 5 x 10^-6 toward the log-rank conjecture; a polynomial-time algorithm for 1/5-approximate Nash equilibria in two-player games; and an edge-reconstruction result for dense graphs. The factoring paper's page says a complete Lean 4 formalisation exists and **will be released in a companion submission**.

**Analysis — why it matters:** *Analysis: this is the third frontier lab this week to post machine-written claims on long-standing problems, after Anthropic's VP versus VNP paper and OpenAI's matrix-multiplication manuscript. Because the constant in the factoring bound is **105, not the sieve's roughly 1.92**, the result concerns what can be proved, not how fast RSA keys can be broken.*

**Caveat:** None of the six papers has been peer reviewed, and the Lean proofs are **promised but not yet public**, so no outside check exists. The authorship claim is Google's own. The folder carries the repository's standard line 'This is not an official Google product'. The paper count comes from the folder index; the factoring and discrete-logarithm summaries come from the papers' own abstracts.

**Community reaction (opinion, not verified fact):**

> “Math is going through its own version of the industrial revolution.” — [david-gpu on Hacker News](<https://news.ycombinator.com/item?id=50642161>)

> “Since several comments ask about the practical effect of this paper for things like factorization: None at all.” — [dgacmu on Hacker News](<https://news.ycombinator.com/item?id=50642784>)

**Sources:**

1. [Google Research (GitHub): Cogentic research papers index](<https://github.com/google-research/google-research/tree/master/cogentic_research_papers>) — primary source. Checked: 25 Nov 2026, 16:06 CET
2. [Google Research (GitHub): Unconditional Integer Factorization in Time L\_N\[1/3, O(1)\]](<https://github.com/google-research/google-research/tree/master/cogentic_research_papers/integer_factorization>) — primary source. Checked: 25 Nov 2026, 16:06 CET
3. [Google Research (GitHub): commit adding six Cogentic research papers](<https://github.com/google-research/google-research/commit/4a7bc8ab0bc770e71a259b7966c500496b99010a>) — primary source. Checked: 25 Nov 2026, 16:06 CET
4. [arXiv: Cogentic, multi-agent orchestration for automated proof discovery](<https://arxiv.org/abs/2609.40324>) — primary source. Checked: 25 Nov 2026, 16:06 CET
5. [Hacker News discussion](<https://news.ycombinator.com/item?id=50642086>) — community. Checked: 25 Nov 2026, 16:06 CET

### Amazon and Meta are in talks to end Amazon's block on Meta's Muse shopping agent, Fortune reports

*Industry & policy · New*

**Published:** 25 Nov 2026

Amazon and Meta have held **multiple rounds of talks** about a deal that would let Meta's Muse agent connect to Amazon's store and end the block Amazon imposed two months ago, Fortune reported on Wednesday, citing people familiar with the discussions. This paper noted on 13 November that Amazon blocks Muse, and on 24 November reported Muse's UK launch.

According to Fortune, as summarised by TechCrunch and The Verge, the two sticking points are **how search results and advertising** would be handled. Amazon is said to worry about losing ad revenue, about the quality of the products Muse would surface, and about agents weakening its direct relationship with shoppers. Any agreement would reportedly need **sign-off from both chief executives**.

Neither company had responded to TechCrunch's or The Verge's requests for comment. The Verge notes that Amazon also blocked Perplexity's shopping agent and is promoting its own Alexa for Shopping assistant.

**Analysis — why it matters:** *Analysis: Amazon is the largest store an agent can be shut out of. Whether it opens up, and on what ad and ranking terms, will shape how much **third-party shopping agents can actually buy**.*

**Caveat:** The talks are reported from anonymous sources; **no deal has been announced** and Fortune says it is unclear whether one will be reached. Fortune's article was not read directly; its account is cited through TechCrunch and The Verge.

**Sources:**

1. [TechCrunch: Amazon and Meta reportedly in talks to lift blockade on AI agent Muse](<https://techcrunch.com/2026/11/25/amazon-and-meta-reportedly-in-talks-to-lift-blockade-on-ai-agent-muse/>) — reporting. Checked: 25 Nov 2026, 16:06 CET
2. [The Verge: Amazon is reportedly in talks to end Muse AI shopping block](<https://www.theverge.com/tech/1042071/meta-amazon-muse-ai-shopping-discussions>) — reporting. Checked: 25 Nov 2026, 16:06 CET

### UPDATE: AI shares fall for a second day after Huang's return, with Nasdaq futures down 3.2% and Korea's Kospi closing 6.2% lower

*Industry & policy · Updated*

**Published:** 25 Nov 2026

Update to Tuesday afternoon's report that Anthropic's shares had fallen below their $83 IPO price. The sell-off in AI stocks continued on Wednesday: before the New York open, **Nasdaq futures were down 3.2%** and S&P 500 futures 2.1%, Nvidia had slid 6.2% and Anthropic 5%, and CoreWeave nearly 9%, CNN reported. Anthropic closed Tuesday at **$81.91**, just under its offer price.

In Asia, South Korea's Kospi, dominated by the memory makers SK Hynix and Samsung, **closed down 6.2%**, CNN reported. AP reported that Taiwan's Taiex closed 4.8% lower, with TSMC down 3.6% and MediaTek down 10%.

AP said questions about Nvidia's governance and President Trump's shareholding added to doubts about AI valuations, alongside expected US tariff increases and Wednesday's October inflation data. Nvidia had risen more than 30% on Monday after reinstating Jensen Huang as chief executive.

**Analysis — why it matters:** *Analysis: the one-day rally on Huang's return has fully reversed, which suggests investors' worries about **AI spending, debt and regulation** run deeper than one company's leadership.*

**Caveat:** All US figures are **pre-market moves** reported on Wednesday morning, New York time; the regular session closes after this edition, and the final numbers will differ.

**Community reaction (opinion, not verified fact):**

> “It's so bizarre to see these crazy breakthroughs daily, but the market (and especially the AI market) keeps sliding down.” — [howunfortunate on Hacker News](<https://news.ycombinator.com/item?id=50642883>)

**Sources:**

1. [CNN: Tech stock selloff deepens as AI fears outweigh Huang's Nvidia return](<https://edition.cnn.com/2026/11/25/business/ai-sell-off-despite-huang-nvidia-return>) — reporting. Checked: 25 Nov 2026, 16:06 CET
2. [AP (via San Diego Union-Tribune): AI rout continues as market exuberance fades](<https://sandiegouniontribune.com/2026/11/25/ai-nvidia-wall-street>) — reporting. Checked: 25 Nov 2026, 16:06 CET

### Fujitsu joins OpenAI's Daybreak Defense Network and launches a vulnerability-assessment service built on OpenAI's cyber-defence tools

*Industry & policy · New*

**Published:** 25 Nov 2026

Fujitsu said on Wednesday that it has joined the **Daybreak Defense Network**, OpenAI's partner programme for cyber defence, and launched a **vulnerability-assessment service** the same day. The service combines OpenAI Daybreak's cyber-defence capabilities with Fujitsu's own AI-powered assessment system, linking source-code analysis with tests against live environments.

Fujitsu says the service covers discovery, checks whether a flaw can actually be exploited, remediation advice and retesting after a fix. It says its red team penetrated **all of roughly 30 organisations** it tested in 2026, and that in internal trials the system found new vulnerabilities that conventional methods missed. OpenAI Japan's Dino Mizushima said the network's security specialists review the results of AI-assisted assessments.

**Analysis — why it matters:** *Analysis: OpenAI is selling its security tools through large integrators rather than only directly, which puts AI-driven attack testing into ordinary enterprise contracts.*

**Caveat:** The effectiveness claims are **Fujitsu's own** and come with no published figures on the vulnerabilities found. Fujitsu's page refused a plain request (HTTP 429) and was read through a web-extraction tool.

**Sources:**

1. [Fujitsu: Fujitsu expands collaboration with OpenAI to launch a vulnerability assessment service](<https://global.fujitsu/en-global/pr/news/2026/11/25-01>) — primary source. Checked: 25 Nov 2026, 16:06 CET

### Japan's government outlines a goal of becoming the leading AI nation after the US and China in its revised security documents

*Industry & policy · New*

**Published:** 25 Nov 2026

Japan's government presented the economic-security sections of its revised **three national security documents** to a meeting of the ruling Liberal Democratic Party on Wednesday and obtained broad approval, Jiji reported in The Japan Times. The outline sets a goal of becoming a **leading AI nation after the United States and China**.

According to the outline, the documents will call for **reducing Japan's AI reliance** on other countries, invest intensively in automated driving and physical AI, and seek technology that makes Japan indispensable to others. The revisions are due later this year.

**Analysis — why it matters:** *Analysis: writing AI into national-security doctrine ties Japan's chip, model and data spending to defence planning rather than industrial policy alone.*

**Caveat:** This is an **outline approved by the ruling party**, not the final documents; the cabinet still has to adopt the revisions. The Japan Times refused a plain request (HTTP 403) and was read through a web-extraction tool.

**Sources:**

1. [The Japan Times (Jiji): Japan to declare aim to become AI nation after U.S. and China](<https://www.japantimes.co.jp/news/2026/11/25/japan/ai-nation-aim/>) — reporting. Checked: 25 Nov 2026, 16:06 CET

## Key patterns (editorial analysis)

- Machine-written mathematics is arriving in batches: Google posted **six Cogentic papers in one commit**, a day after OpenAI's and Anthropic's own claims, with formal proofs still to come.
- Agents now meet commercial gatekeepers: Amazon is reportedly negotiating **ads and search terms for Muse**, and OpenAI is reaching companies through partners such as Fujitsu.
- Markets and governments are pulling in different directions: AI shares fell again while Japan wrote an **AI-power goal into security planning**.

## Source coverage

- Engine version: 4.6.0
- Engine ran this edition: yes
- Engine look-back: 2 days

### Source status

- reddit: ok, partial (17 threads; Reddit blocked direct requests with HTTP 403; the Arctic Shift archive supplied posts)
- hackernews: ok (26 stories)
- github: ok (4 items)
- devto: ok (12 articles; tags ai and llm)
- youtube: not searched (yt-dlp not available on this machine)
- polymarket: not used: blocked in France (ANJ)
- x: not searched (no consent-free source configured)

### Notes

- The installed last30days engine (4.6.0) finished (exit 0) with evidence from Reddit, Hacker News, dev.to and GitHub. Its top clusters were mostly older items (Tidal's AI-music ban, Anthropic's 'Working with AI' study, an agent-checked Riemann draft); the Cogentic papers were found through a Hacker News scan of the window. Stories were also found with Google News RSS queries, publisher feeds, post-engine web supplements and the source pages. Item counts are not counts of verified developments.
- Polymarket not used: blocked in France (ANJ). X not searched. YouTube not searched (not available on this machine). Reddit returned results only through the Arctic Shift archive, because Reddit blocked direct requests (HTTP 403), so Reddit coverage was partial. Three Google News queries and VentureBeat's feed answered HTTP 429. Missing coverage does not mean nobody discussed these stories.
- Window widened: it starts at 19:00 Paris time on Tuesday 24 November, before the previous issue time (06:07 today), to include KRAFTON's Raon-1 mini release, which no edition carried. Nothing that an earlier edition carried is repeated except as a labelled update.
- Read through other routes: Fujitsu's press release (HTTP 429) and The Japan Times (HTTP 403) refused plain requests and were read with a web-extraction tool; The Register's JetBrains report was read with scripts/fetch\_source.py's direct route. Fortune's exclusive on the Muse talks was not read directly and is cited through TechCrunch and The Verge.
- Newsletter leads from the Iris mail bot: today's file still holds the same five leads as this morning, all already carried, repeated or older than 48 hours; none was used.
- Not carried: JetBrains' Kotlin Benchmark 2.0, posted 23 November, outside the window; Google DeepMind's agent-found quantum algorithms (23 November) and Ant Group's Ling-3.2-air (23 November), both older than 48 hours; the US Army's request for proposals for power and data centres at nine bases (19 to 20 November); OpenAI's tests of email addresses for its Dots agents, reported 24 November and first mentioned 17 November; a US jury's conviction of Huawei, which fell in the previous edition's window; and a Wall Street Journal report on Anthropic's debt, which is paywalled.
- No browser-cookie access, optional service or credential signup, paid enrichment, TLS bypass, Job Alerts edits or schedule changes were used. Research logs and full provenance remain private.

### Engine footer (verbatim)

```text
---
✅ All agents reported back!
├─ 🟠 Reddit: 17 threads │ 1,858 upvotes │ 1,200 comments
├─ 🟡 HN: 26 stories │ 1,052 points │ 715 comments
├─ 👩‍💻 dev.to: 12 articles │ 143 reactions │ 62 comments
├─ 🐙 GitHub: 4 items │ 13 reactions │ 48 comments
├─ 🗣️ Top voices: r/artificial, r/technology, r/ClaudeAI
---
```
