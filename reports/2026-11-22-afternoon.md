# The AI Gazette — Afternoon edition, Sunday 22 November 2026

*Models, machines, and matters of consequence*

- Issue: 2026-11-22-afternoon
- Issued: 22 Nov 2026, 16:08 CET (Paris)
- Reporting window: 20 Nov 2026, 20:40 CET to 22 Nov 2026, 16:08 CET
- Timezone: Europe/Paris
- Previous issue: 2026-11-22-morning
- Price: Complimentary

## Editor's note

About ten hours since the morning edition, a quiet Sunday, and **no new model release**. The window was widened back to 20:40 on Friday to carry METR's capability update and Saturday's newspaper reports on the Nvidia chip affair, which earlier editions missed. OpenRouter **dropped three inference providers** after the Dragos canary study. The governors of both parties set out **principles for a federal AI framework**, and South Korea's education minister resigned over his anti-AI-cheating rules.

## The News

### UPDATE: OpenRouter drops three inference providers and strips 125 endpoints of zero-data-retention status after the Dragos canary study

*Coding & agents · Updated*

**Published:** 22 Nov 2026

Update to this morning's edition, which reported Together AI's disclosure that a credential committed by a coding agent let an outsider download stored customer prompts, and Dragos's study of about two million seeded prompts. The new development: OpenRouter, which routes customers' requests to many third-party model hosts, says it has **off-boarded three providers** based on its own investigations.

OpenRouter also says it **removed 125 endpoints from Zero Data Retention eligibility**, covering providers the researchers flagged plus others removed as a precaution, and has notified all potentially affected customers. It says the findings showed no breach of OpenRouter itself, that it will run similar canary checks on an ongoing basis, and that removed endpoints need assurances and validation before regaining that status. It does not name the three providers.

Its post lists public notices from Novita, Phala and Together. Novita says a routing configuration issue sent some MiniMax requests to **MiniMax's official API** instead of its own servers: requests to MiniMax models through Novita between **28 May and 11 November 2026** may have been accessed or retained by a third party, including requests routed through OpenRouter. Novita says it has suspended the affected models and is following up with MiniMax.

**Analysis — why it matters:** *Editorial analysis: a marketplace that resells other companies' inference is now **testing providers' privacy promises** instead of taking them on trust; customers still cannot see which hosts were dropped.*

**Caveat:** The actions and the no-breach finding are OpenRouter's and Novita's own statements. Neither post gives a time of publication, and OpenRouter has not said whether Novita, Phala or Together is among the three providers it removed.

**Community reaction (opinion, not verified fact):**

> “the best ZDR agreement is the one that your company has directly with the inference provider(s).” — [redrix (Hacker News)](<https://news.ycombinator.com/item?id=50595608>)

> “Zero data retention, give or take 125 endpoints.” — [cobychapple (Hacker News)](<https://news.ycombinator.com/item?id=50596126>)

**Sources:**

1. [OpenRouter: Data Processing Incidents on Inference Providers](<https://openrouter.ai/blog/announcements/data-processing-incidents-on-inference-providers/>) — primary source. Checked: 22 Nov 2026, 16:06 CET
2. [Novita: Privacy notice regarding MiniMax requests on Novita](<https://novita.ai/blog/minimax-requests-privacy-notice/>) — primary source. Checked: 22 Nov 2026, 16:06 CET
3. [Dragos: AI supply chain security, what canary tokens found](<https://www.dragos.com/blog/ai-supply-chain-security-canary-tokens>) — primary source. Checked: 22 Nov 2026, 16:06 CET
4. [Hacker News: Data Processing Incidents on Inference Providers](<https://news.ycombinator.com/item?id=50595554>) — community. Checked: 22 Nov 2026, 16:06 CET

### METR says AI capabilities relevant to speeding up AI research are improving fast and getting harder to measure

*Research · New*

**Published:** 20 Nov 2026

METR, the independent evaluation group, published a research update on Friday 20 November covering public models up to **Claude Opus 5.5 and GPT-6 Astra**. It says current public evidence is **insufficient to rule out drastic acceleration of AI research** in the next couple of years, meaning progress so fast that humans could no longer meaningfully assess and react to catastrophic risks. Earlier editions did not carry it.

On its coding and optimisation tasks, METR says models usually match or beat skilled humans: when it recruited its own baseliners it **typically failed to find humans who outperform** the frontier models. Where many specialists had attempted a task, such as programming contests, models placed at a very high percentile but not at the very top.

On tasks that require choices without clear, fast feedback, METR says agents appear to have **worse judgment than human experts**. Across its two task suites it estimates that time horizons double roughly every **3.6 months**; naive extrapolation would reach its longest tasks, 200 hours, in July 2027, a projection it labels naive.

**Analysis — why it matters:** *Editorial analysis: the group whose 'time horizon' measure became a standard yardstick now says that measure no longer lets it argue that risk is low, which matters for labs and regulators that lean on its evaluations.*

**Caveat:** METR stresses **significant uncertainty**, including about which capabilities would actually be needed for drastic acceleration; its trend findings are sensitive to methodological choices, and its human comparisons rely on small baseliner pools.

**Sources:**

1. [METR: AI R&D-relevant model capabilities are improving rapidly and are getting harder to measure](<https://metr.org/blog/2026-11-20-q4-2026-capability-update>) — primary source. Checked: 22 Nov 2026, 16:06 CET

### UPDATE: The WSJ names a Singapore businessman as a key operator behind Megaspeed, and the NYT says China's spy agency ran a two-year chip campaign

*Industry & policy · Updated*

**Published:** 21 Nov 2026

Update to the 18 November morning edition, which reported Nvidia's results and its board ruling out Jensen Huang's return. The new development: The Wall Street Journal reported on Saturday that **Li Ming, a 52-year-old Chinese national** living in Singapore, took part in major decisions at Megaspeed, the company where Alice Huang was an executive, and played a key role at other firms trading Nvidia chips, citing people familiar with the businesses, according to The Asia Business Daily and Livemint.

Li was **charged with fraud in Singapore in February 2025** and is on bail. Prosecutors say he bought Nvidia-equipped servers from Supermicro by naming a local company he controlled as the end user, before the servers went to Malaysia and then a third location. The Journal also reports that a newer cloud company linked to people from Megaspeed, **Novagate Cloud**, imported at least $300 million of hardware containing Nvidia chips into Malaysia from January to May 2026, according to shipping records.

Separately, The New York Times reported on Saturday that China's Ministry of State Security has run a campaign for **at least two years** to help Chinese companies obtain and smuggle advanced AI chips and to gather intelligence on the industry, through a team reporting to its chief, Chen Yixin, citing serving and former officials in Asia, the United States and Europe, according to Chosunbiz. The Times says Alice Huang's specific role in that effort has not been established.

**Analysis — why it matters:** *Editorial analysis: both reports widen the affair from one executive's relationship to **networks that may still be buying chips**, just as Washington tightens rules on remote access to US chips.*

**Caveat:** Both reports rest on unnamed sources and were read only through other outlets' summaries, as the WSJ and NYT articles are paywalled. Li's lawyers did not respond to the Journal; Megaspeed denies diverting chips, and China calls the espionage claims fabrication.

**Sources:**

1. [The Asia Business Daily: WSJ says Li Ming was involved in key Megaspeed decisions](<https://view.asiae.co.kr/en/article/2026112214284920436>) — reporting. Checked: 22 Nov 2026, 16:06 CET
2. [Livemint: Who is Li Ming? The man linked to Nvidia's China chip trail](<https://www.livemint.com/companies/news/who-is-li-ming-how-did-alice-huangs-associate-funnel-nvidia-ai-chips-to-china-read-about-the-accusation-11795345041140.html>) — reporting. Checked: 22 Nov 2026, 16:06 CET
3. [Chosunbiz: China reportedly runs covert operation to obtain advanced AI chips](<https://biz.chosun.com/en/en-it/2026/11/22/IM6LALMIMZA4DCAQVBI3A37L3Q>) — reporting. Checked: 22 Nov 2026, 16:06 CET

### US governors of both parties ask Congress for a federal AI framework that leaves states room to regulate

*Industry & policy · New*

**Published:** 22 Nov 2026

The National Governors Association published **bipartisan principles for AI governance** on Sunday, drawn up by a council led by Maryland Governor Wes Moore, Indiana Governor Mike Braun, North Carolina Governor Josh Stein and Utah Governor Spencer Cox. The association says they are meant to inform the incoming Congress as it develops an AI framework.

The principles split the roles: the federal government should handle national and international AI risks, including a **risk-based framework for frontier models** with independent evaluation or audits and reporting of security breaches and significant safety incidents to federal authorities and affected states. States would remain the main check on harms to people as AI is used, including to children, older adults and workers.

On the central fight with Washington, the document says any attempt to **preempt state laws should be approached cautiously** and include meaningful input from a cross-section of states.

**Analysis — why it matters:** *Editorial analysis: the governors take a middle position in the preemption debate, accepting national rules for frontier models while resisting a federal override of state laws.*

**Caveat:** These are **recommendations, not law**; the association names no bill or congressional sponsor.

**Sources:**

1. [National Governors Association: Governors Call for AI Action](<https://www.nga.org/news/press-releases/governors-call-for-ai-action/>) — primary source. Checked: 22 Nov 2026, 16:06 CET
2. [NGA: Federal and State Roles in AI Regulation, statement of principles (PDF)](<https://www.nga.org/wp-content/uploads/2026/11/NGA_AI_Princples_Nov2026.pdf>) — primary source. Checked: 22 Nov 2026, 16:07 CET

### UPDATE: South Korea's education minister resigns over last-minute rules against AI cheating at the national college exam

*Industry & policy · Updated*

**Published:** 22 Nov 2026

Update to the 15 November afternoon edition, which reported that the top scorer in South Korea's tax accountant exam admitted cheating with a hidden camera and generative AI. The new development: **Education Minister Choi Kyo-jin resigned on Sunday**, and President Lee Jae Myung accepted his resignation the same day, Yonhap and the Korea JoongAng Daily report.

Choi took responsibility for confusion caused by anti-cheating rules changed until the eve of Thursday's college entrance exam, the Suneung, which about 500,000 students sat. The measures included **covering clothing buttons with stickers** to block miniature cameras and three emergency alerts sent to mobile phones nationwide during the exam. The ministry said **111 suspected cheating cases** involving electronic devices were detected.

Lee wrote on X that concerns over AI-assisted cheating are spreading to essay-based admissions and school tests, and said the government would inspect how exams are managed, the JoongAng Daily reports.

**Caveat:** The 111 cases are suspected cases reported by the ministry; how many involved AI tools has not been published.

**Sources:**

1. [Yonhap: Education minister resigns over college exam chaos amid AI cheating fears](<https://en.yna.co.kr/view/AEN20261122001052315>) — reporting. Checked: 22 Nov 2026, 16:07 CET
2. [Korea JoongAng Daily: Lee accepts education minister's resignation](<https://koreajoongangdaily.com/korea/lee-accepts-education-ministers-resignation-after-csat-anticheating-measures-trigger-nationwide-confusion/12984387>) — reporting. Checked: 22 Nov 2026, 16:07 CET
3. [BBC: South Korea education minister resigns over exam cheating scandal](<https://www.bbc.com/news/articles/cw3dgk29d37no>) — reporting. Checked: 22 Nov 2026, 16:07 CET

### Anthropic capped IPO deal teams and sought six-month bars on bankers working for rivals, Reuters reports

*Industry & policy · New*

**Published:** 22 Nov 2026

Anthropic told some of its 22 IPO underwriters to **limit their deal teams to four bankers**, all senior, Reuters reported on Sunday, citing several people familiar with the matter. One of them said the rule likely came from fear of leaks.

According to the report, Anthropic also asked some senior bank officers to sign documents **barring core deal-team members from working with rivals** including OpenAI, Cursor, DeepSeek and Hugging Face for six months after the listing. Bankers and lawyers told Reuters that exclusivity this broad is rare. University of Florida professor Jay Ritter said Anthropic, like SpaceX, negotiated to pay underwriters **nothing on the extra greenshoe shares**.

Anthropic, Goldman Sachs and Morgan Stanley declined to comment to Reuters. Anthropic's shares closed down 8.5% on Friday after their 17% first-day rise.

**Analysis — why it matters:** *Editorial analysis: the account shows how much leverage the largest AI companies now hold over Wall Street banks, and what other AI listings may try to impose.*

**Caveat:** The account rests on unnamed people close to the process. The Reuters page could not be fetched here; it was read in a syndicated copy.

**Sources:**

1. [Global Banking & Finance Review (Reuters): Like SpaceX, Anthropic ran an unusual IPO process, chafing some bankers](<https://www.globalbankingandfinance.com/exclusive-like-spacex-anthropic-ran-unusual-ipo-process/>) — reporting. Checked: 22 Nov 2026, 16:07 CET

## Key patterns (editorial analysis)

- Agent supply chains are being policed after the fact: OpenRouter **dropped three providers** once a canary study showed prompts leaking.
- Rules for AI are being written at every level at once, from governors' **federal-state split** to South Korea's exam halls.
- The Nvidia affair keeps widening into a question of **chip networks and state intelligence**, not one executive.

## Source coverage

- Engine version: 4.6.0
- Engine ran this edition: yes
- Engine look-back: 2 days

### Source status

- reddit: ok, partial (17 threads; Reddit blocked direct requests with HTTP 403; the Arctic Shift archive supplied posts)
- hackernews: ok (27 stories)
- github: ok (3 items)
- devto: ok (12 articles; tags ai and llm)
- youtube: not searched (yt-dlp not available on this machine)
- polymarket: not used: blocked in France (ANJ)
- x: not searched (no consent-free source configured)

### Notes

- The installed last30days engine (4.6.0) finished (exit 0) in 85 seconds with 59 evidence items from Reddit, Hacker News, dev.to and GitHub. Its top clusters were an essay on conscious AI, a coding agent for DOS, a Reddit thread on the AI trade and a European-law MCP server. Stories were found with 16 Google News RSS queries, publisher feeds, a Hacker News scan of the window, post-engine web supplements and the source pages. Item counts are not counts of verified developments.
- Window widened: it starts at 20:40 on Friday 20 November, just before METR announced its capability update, instead of at 06:09 this morning, to carry that report and Saturday's WSJ and NYT reports on the Nvidia chip affair, which earlier editions missed. Nothing an earlier edition carried is repeated.
- Polymarket not used: blocked in France (ANJ). X not searched. YouTube not searched (not available on this machine). Reddit returned results only through the Arctic Shift archive, because Reddit blocked direct requests (HTTP 403), so Reddit coverage was partial. VentureBeat's feed answered HTTP 429. Missing coverage does not mean nobody discussed these stories.
- Paywalled or not read: The Wall Street Journal's report on Li Ming and The New York Times' report on China's Ministry of State Security (both paywalled; read through The Asia Business Daily, Livemint and Chosunbiz), Bloomberg's report on the governors' principles (paywalled; the governors' own release was used), and Reuters' report on Anthropic's IPO process (the Reuters page could not be fetched; read in a syndicated copy).
- Newsletter leads from the Iris mail bot: today's file has four leads, all already covered or not carried this morning: Gemini 4 Neon ran on 19 November, and the rest are listed in the morning edition's notes.
- Not carried, as older or already covered: Tencent's Hy4 safety assessment (system card released 20 November; Hy4 covered earlier), the White House AI accord Trump called a 'constitution' (29 September), Wells Fargo's AI-agent terms (reported 3 November), coverage of the April attacks on Sam Altman's home, and the Frostbite CPU claim (carried 20 and 21 November).
- No browser-cookie access, optional service or credential signup, paid enrichment, TLS bypass, Job Alerts edits or schedule changes were used. Research logs and full provenance remain private.

### Engine footer (verbatim)

```text
---
✅ All agents reported back!
├─ 🟠 Reddit: 17 threads │ 19,161 upvotes │ 4,339 comments
├─ 🟡 HN: 27 stories │ 2,933 points │ 2,329 comments
├─ 👩‍💻 dev.to: 12 articles │ 179 reactions │ 88 comments
├─ 🐙 GitHub: 3 items │ 14 reactions │ 14 comments
├─ 🗣️ Top voices: r/technology, r/singularity, r/OpenAI
---
```
