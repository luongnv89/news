# The AI Gazette — Afternoon edition, Sunday 1 November 2026

*Models, machines, and matters of consequence*

- Issue: 2026-11-01-afternoon
- Issued: 1 Nov 2026, 16:08 CET (Paris)
- Reporting window: 31 Oct 2026, 16:07 CET to 1 Nov 2026, 16:07 CET
- Timezone: Europe/Paris
- Previous issue: 2026-11-01-morning
- Price: Complimentary

## Editor's note

This Sunday afternoon edition has **six new stories and no updates**. The window opens at Saturday's 16:07 issue so it can carry two items this morning's edition missed: OpenAI's plan to **merge ChatGPT and Codex usage**, first discussed late on Saturday, and xAI's watermark notice dated 31 October. The other four appeared on Sunday. No new model release met the bar, and two items are plans rather than decisions: OpenAI's Washington push and a Korea-Japan data-centre fund.

## The News

### xAI will watermark text from seven Grok API models by default from 7 November, citing the EU AI Act

*Models · New*

**Published:** 31 Oct 2026

A developer documentation page from xAI, whose docs now carry the SpaceXSI name, says that **starting 7 November 2026** text responses from grok-4.7, grok-4.6, grok-4.5, grok-4.3 and three grok-4.20 variants will include **an invisible watermark**. The page says the watermark is applied "to comply with the EU AI Act". It was last updated on 31 October.

The watermark is on by default on every API endpoint. It covers ordinary text, structured outputs and tool-call arguments, and a response header, x-watermark, shows whether it was applied. **Team admins can opt out per model**, but must confirm that a legal exception applies and that they are responsible for any marking or disclosure duties.

The mark works by slightly shaping which tokens the model picks, so no characters are added. Detection is statistical and returns watermarked, not watermarked or uncertain, with longer text giving a stronger signal. **Access to the detection API is granted by application**.

**Analysis — why it matters:** *Analysis: with Anthropic extending its own text watermark to older Claude models, as this morning's edition reported, watermarking is becoming normal for API text. Only xAI and the organisations it admits can check for this mark.*

**Caveat:** xAI states that watermarking does not change quality or speed; that is **a vendor claim**. The page publishes **no accuracy or false-positive figures** and does not say how the mark holds up after paraphrasing or translation.

**Sources:**

1. [SpaceXSI Docs: Output Watermarking](<https://docs.x.ai/developers/advanced-api-usage/watermarking>) — primary source. Checked: 1 Nov 2026, 16:04 CET

### OpenAI says ChatGPT and Codex will share one token-based usage allowance from December as Work moves into the main chat

*Coding & agents · New*

**Published:** 1 Nov 2026, 14:53 CET

An OpenAI Help Center page says that **starting in December**, the usage allowance on Plus, Pro and Business plans **will be shared across ChatGPT and Codex**, "as we bring the agentic capabilities of Work into the main ChatGPT experience". Usage will be measured in tokens, so more advanced models and complex tasks use more of the allowance; **Instant chat will not draw from it**.

OpenAI says it expects most users will not have to wait for a reset more often than they do now. Combined remaining usage and reset times will appear under Settings, and users who hit the limit can wait, upgrade or buy credits. The page gives no allowance figures.

BleepingComputer, which saw an OpenAI email to subscribers, reports that a **combined Chat and Work experience will be tested** with a small group of users in the coming weeks, and that Codex stays a separate experience in the ChatGPT desktop app. Hacker News users were discussing the help page by late Saturday evening, after this journal's Saturday afternoon edition.

A second help page sets **card and device limits**: too many Go, Plus or Pro subscriptions on one payment card or device can block a purchase, and a device can show "Device limit reached". Free, Business, Enterprise and Edu accounts do not count. The Decoder reads this as aimed at people who rotate several cheap paid accounts to get more usage.

**Analysis — why it matters:** *Analysis: a single metered budget ends the separation between everyday chat and agent work. Heavy Codex users will now trade coding runs against chat with advanced models, and one Hacker News commenter says Claude has worked this way for a while.*

**Caveat:** Both help pages are **undated**, so the exact date of the change is unclear. This journal did not read OpenAI's email itself; its contents are as reported by BleepingComputer. OpenAI publishes **no numerical allowances** for any plan. BACKGROUND: the Pro usage increase of 29 October was covered on 30 October.

**Community reaction (opinion, not verified fact):**

> “Not surprising: Claude has behaved like this for awhile and it was only a matter of time.” — [minimaxir (Hacker News)](<https://news.ycombinator.com/item?id=50320635>)

> “I got it, too. Not surprising but this was definitely one of the deciding factors keeping me with ChatGPT. Much more willing to change providers now.” — [sjs382 (Hacker News)](<https://news.ycombinator.com/item?id=50321692>)

**Sources:**

1. [OpenAI Help Center: ChatGPT and Codex usage limits](<https://help.openai.com/en/articles/20001625-understanding-chatgpt-and-codex-usage-limits>) — primary source. Checked: 1 Nov 2026, 16:03 CET
2. [OpenAI Help Center: card and device limits](<https://help.openai.com/en/articles/20001559-understanding-card-and-device-limits-in-chatgpt>) — primary source. Checked: 1 Nov 2026, 16:05 CET
3. [BleepingComputer](<https://www.bleepingcomputer.com/news/artificial-intelligence/openai-says-its-doubling-pro-usage-limits-and-bringing-work-features-to-chat/>) — reporting. Checked: 1 Nov 2026, 16:03 CET
4. [The Decoder: Chat and Work merger](<https://the-decoder.com/openais-upcoming-chat-and-work-merger-in-chatgpt-signals-the-end-of-all-you-can-prompt-pricing/>) — reporting. Checked: 1 Nov 2026, 16:03 CET
5. [The Decoder: paid usage](<https://the-decoder.com/openai-is-steering-chatgpt-users-toward-more-paid-usage/>) — reporting. Checked: 1 Nov 2026, 16:03 CET
6. [Hacker News discussion](<https://news.ycombinator.com/item?id=50320588>) — community. Checked: 1 Nov 2026, 16:03 CET

### Leading mathematicians warn that OpenAI and Anthropic could keep AI-made mathematics behind paywalls

*Research · New*

**Published:** 1 Nov 2026, 06:00 CET

The Observer reports that Britain's most senior mathematicians, including **three Fields medal winners**, met at the Royal Society in London last week. The meeting followed OpenAI's publication last month of solutions, generated by its frontier models, to 377 of the hardest mathematical problems.

Martin Bridson, president of the Clay Mathematics Institute, described a "longer-term fear that knowledge could be hoarded behind paywalls" and asked: "Why should they get to say who has access to these tools, and on what basis do they choose who gets access?" So far **OpenAI and Anthropic have each committed $5m** to a Simons Foundation fund that gives some researchers access to their models.

Fields medallist Martin Hairer said open models cannot compete with frontier ones, leaving "one of the main tools for mathematic research" **under the control of two US companies**. Ana Caraiani of Imperial College London said no institution in Romania, her native country, is eligible to apply for access.

**Analysis — why it matters:** *Analysis: the dispute has moved from who solved a problem first to who controls access to the tools, which is a question about research governance rather than model quality.*

**Caveat:** These are **concerns, not evidence that results have been withheld**; neither company is reported as saying it will keep mathematical work secret, and the article as read carries no response from either company.

**Sources:**

1. [The Observer](<https://observer.co.uk/news/national/article/mathematicians-warn-ai-firms-are-keeping-vital-research-in-the-field-secret>) — reporting. Checked: 1 Nov 2026, 16:04 CET

### Axios: OpenAI plans a post-midterm push in Washington for 'speed limits' on the most powerful AI and new data-centre deals

*Industry & policy · New*

**Published:** 1 Nov 2026

Axios reports that right after Tuesday's US midterm elections, OpenAI will launch **a policy and PR campaign** starting in Congress's lame-duck session, which opens on 9 November. Chris Lehane, OpenAI's chief global affairs officer, told Axios his team has been stockpiling proposals since August, "some new and some repackaged".

The first proposal is what OpenAI calls **"speed limits"**: new ideas for mandatory safeguards on the most powerful AI systems, with a more aggressive drive in Congress. "You're going to see us talk more and more about the concept of speed limits," Lehane said.

On data centres, OpenAI plans community compacts and **proposed state legislation** giving residents a say in how projects are built and what benefits they receive. It will also argue that its facilities should be called **"AI compute campuses"**, citing a project in Pike County, Ohio. Further proposals cover help for workers, education and training, and US-shaped international standards.

**Analysis — why it matters:** *Analysis: a frontier lab asking for mandatory limits on frontier systems is notable, but until OpenAI publishes the proposals it is not possible to judge how binding they would be or whom they would constrain.*

**Caveat:** These are plans described to Axios, not published proposals; OpenAI has not said what a "speed limit" would require in practice. Axios **discloses a content licensing and technology agreement with OpenAI**. Axios blocked this journal's automated reader, so the story was read through a search index copy of the Axios page and a syndicated copy.

**Sources:**

1. [Axios](<https://www.axios.com/2026/11/01/scoop-openai-post-midterm-policy>) — reporting. Checked: 1 Nov 2026, 16:05 CET
2. [Daily8 (syndicated copy of the Axios story)](<https://www.daily8.com/en/article/d8_4945f438c59d6b3a24743d55aa65370b82cbe8bc011dfe10972e111fcd89bdb4>) — reporting. Checked: 1 Nov 2026, 16:05 CET

### KB Kookmin Bank will lead a record 10.7 trillion won loan for GPUs that will supply Naver Cloud

*Industry & policy · New*

**Published:** 1 Nov 2026, 06:20 CET

KB Kookmin Bank said on Sunday that it holds the mandate to lead a **10.7 trillion won ($8 billion) syndicated loan** for a Brookfield-backed AI computing project, The Korea Herald reports. The bank calls it **South Korea's first GPU financing** and the country's largest-ever syndicated loan arrangement.

The loan is part of a project worth about 13 trillion won. Brookfield will set up a special-purpose company, tentatively named Asset Co., to buy GPUs and other computing assets and supply capacity to Naver Cloud under a long-term agreement. The bank named no other lenders and gave no loan terms.

Naver's filing sets tentative targets of 55 megawatts in the first half of 2027, 100 megawatts by year-end and **200 megawatts in 2028**, centred on its GAK Sejong data centre. Naver signed its $9 billion infrastructure agreement with Brookfield on Tuesday, a condition of Nvidia's planned $1 billion investment in Naver.

**Analysis — why it matters:** *Analysis: the structure keeps the GPUs off Naver's own books, in a Brookfield-owned company financed by banks, so the cost of Naver's AI capacity now also depends on how lenders value chips.*

**Caveat:** The lender group and the final commitments of other banks have **not been disclosed**; the capacity targets are tentative.

**Sources:**

1. [The Korea Herald](<https://www.koreaherald.com/article/10921731>) — reporting. Checked: 1 Nov 2026, 16:03 CET

### Korea Investment and Japan's SBI discuss a fund of about 1.15 trillion yen to build AI data centres in Japan

*Industry & policy · New*

**Published:** 1 Nov 2026, 09:20 CET

Korea's Financial News reports that Korea Investment Holdings and Japan's SBI Group plan a joint fund to invest **about 1.15 trillion yen** (about 9.75 trillion won) in Japanese data centres with **200 megawatts of capacity**. The two groups are sounding out companies in both countries as investors and plan a blueprint by the end of the year.

Companies are looking at supplying chips, cooling and power equipment and at building and operating the sites. Kyushu is one candidate location, and the project's backers are understood to have held talks with Kyushu Electric Power.

Maeil Business reports a fund target of more than 1 trillion yen and quotes Korea Investment as saying the plan **"has not been confirmed"**. KED Global says the groups hope to expand the partnership over 30 years.

**Analysis — why it matters:** *Analysis: Korean finance and equipment makers are looking abroad for AI-infrastructure demand, in a structure Financial News compares with the Stargate project's pooling of money and suppliers.*

**Caveat:** This is an **early-stage plan reported by the press**; size, timing, site and participants are unconfirmed, and figures differ between reports.

**Sources:**

1. [Financial News (Korea)](<https://en.fnnews.com/news/202611010936588588>) — reporting. Checked: 1 Nov 2026, 16:05 CET
2. [Maeil Business (MK)](<https://www.mk.co.kr/en/stock/12192990>) — reporting. Checked: 1 Nov 2026, 16:05 CET
3. [KED Global](<https://www.kedglobal.com/artificial-intelligence/newsView/ked202611010002>) — reporting. Checked: 1 Nov 2026, 16:05 CET

## Key patterns (editorial analysis)

- Flat-rate AI is giving way to metered budgets: ChatGPT and Codex will **share one token allowance**, with new limits on extra paid accounts.
- Labs are shaping the rules around them: OpenAI will push **"speed limits" for powerful AI**, while xAI turns on **default text watermarks** for the EU AI Act.
- Access is the new fault line: mathematicians fear **AI-made results behind paywalls**, and Korean lenders are financing GPUs at record scale.

## Source coverage

- Engine version: 3.28.0
- Engine ran this edition: yes
- Engine look-back: 2 days

### Source status

- reddit: ok (16 threads)
- youtube: no-results (0 videos)
- hackernews: ok (10 stories)
- polymarket: unreachable (TLS certificate hostname mismatch; not bypassed)
- github: ok (13 items)
- devto: searched with tags ai and llm; 0 articles returned
- x: not searched (no consent-free source configured)

### Notes

- The window runs from Saturday's 16:07 CET afternoon issue to this edition, so it overlaps this morning's window to carry two items that edition missed. Dispatches with only a date carry that date; exact timestamps are given where a source supplied one.
- The installed last30days engine finished in 36 seconds with 39 evidence items from Reddit, Hacker News and GitHub. Its top item was the Hacker News thread on OpenAI's shared ChatGPT and Codex limits, which supplied the community quotes; other top items repeated stories already covered. Stories were chosen with Google News RSS, publisher feeds, web searches and checks of primary documents. Item counts are not counts of verified developments.
- Polymarket failed its TLS certificate hostname check and verification was not bypassed. YouTube completed with no matching videos, dev.to returned no articles and X was not searched. Failed or missing coverage does not mean nobody discussed these stories.
- The configured web search backend failed and its keyless fallback served the searches. Axios blocked automated reading (HTTP 403 and a bot check, not bypassed), so its story was read through a search index copy and a syndicated copy. VentureBeat's feed returned HTTP 429, Anthropic's news feed and one Tom's Hardware article HTTP 404. OpenAI's email to subscribers was not read directly.
- Not carried: the Vals AI study of Chinese models' political answers (published 12 October), Adobe's EditAgent paper (29 October), the UK CMA's Meta investigation (30 October), Google's Suncatcher satellite test (30 October) and the Justice Department's questions about Nvidia's Hugging Face deal (covered 29 October).
- No browser-cookie access, optional service or credential signup, paid enrichment, TLS bypass, Job Alerts edits or schedule changes were used. Research logs and full provenance remain private.

### Engine footer (verbatim)

```text
---
✅ All agents reported back!
├─ 🟠 Reddit: 16 threads │ 707 upvotes │ 341 comments
├─ 🟡 HN: 10 stories │ 412 points │ 340 comments
├─ 🐙 GitHub: 13 items │ 8 reactions │ 14 comments
├─ 🗣️ Top voices: r/singularity, r/artificial, r/ClaudeAI
---
```
