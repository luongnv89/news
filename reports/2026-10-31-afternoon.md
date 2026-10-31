# The AI Gazette — Afternoon edition, Saturday 31 October 2026

*Models, machines, and matters of consequence*

- Issue: 2026-10-31-afternoon
- Issued: 31 Oct 2026, 16:07 CET (Paris)
- Reporting window: 30 Oct 2026, 16:08 CET to 31 Oct 2026, 16:06 CET
- Timezone: Europe/Paris
- Previous issue: 2026-10-31-morning
- Price: Complimentary

## Editor's note

This edition has **five new stories and two updates**. The window reaches back to yesterday's 16:08 afternoon issue so it can carry Chainalysis' Friday-evening breach notice, which this morning's edition did not carry; everything else appeared after this morning's 06:09 issue. The updates add the WSJ's figure of **about $11 billion raised** to OpenAI's funding story, and Singapore's denial of a WSJ report on Alice Huang. New: an AI agent that injected a gene therapy into a live mouse, malware that asks an AI model to rank its victims, Claude Code's reported refusals of game work, and Sam Altman's meetings in Korea. No new model release met the bar for this edition.

## The News

### Developers report Claude Code refusing to recreate existing games, and some say legitimate game and reverse-engineering work is blocked

*Coding & agents · New*

**Published:** 31 Oct 2026, 13:20 CET

Tom's Hardware reports multiple user claims that **Claude Code and the Opus 5.5 model now refuse** to help recreate specific existing games, and in some cases block ordinary reverse-engineering and troubleshooting tasks. Rule text shared on X reads: 'Don't build a recreation of a specific existing game, even if it is renamed or called original.'

Issues filed in Anthropic's Claude Code repository describe the refusals. One, opened on 30 October by the owner of a company that builds digital versions of board wargames for clients who own the games, says that **around 27 October** sessions began receiving a server-side instruction and now refuse work they had done for months. It asks Anthropic to narrow the rule to actual copying, offer an exemption path and document such changes in the changelog.

**Analysis — why it matters:** *Analysis: if the rule is delivered from the server rather than shipped in a release, paying users have no changelog to check when a working project suddenly stops. A category-wide rule also cannot tell piracy from commissioned or original work.*

**Caveat:** **Anthropic has not confirmed the rule text** or commented, and Tom's Hardware notes there is no official confirmation of it. Some reports may come from users with infringing aims.

**Community reaction (opinion, not verified fact):**

> “A blanket category rule against "games" cannot tell the difference between piracy and commissioned professional work for a game's owner” — [lerugray (GitHub issue \#106167)](<https://github.com/anthropics/claude-code/issues/106167>)

> “all those RE guys ll just hop to chat gpt instead” — [vivzkestrel (Hacker News)](<https://news.ycombinator.com/item?id=50316581>)

**Sources:**

1. [Tom's Hardware](<https://www.tomshardware.com/tech-industry/artificial-intelligence/anthropics-ai-model-is-now-blocking-attempts-at-video-game-recreation-and-cloning-users-also-claim-non-malicious-generic-reverse-engineering-tasks-are-blocked>) — reporting. Checked: 31 Oct 2026, 16:03 CET
2. [anthropics/claude-code\#106167](<https://github.com/anthropics/claude-code/issues/106167>) — community. Checked: 31 Oct 2026, 16:03 CET
3. [anthropics/claude-code\#105589](<https://github.com/anthropics/claude-code/issues/105589>) — community. Checked: 31 Oct 2026, 16:04 CET

### WIRED: a start-up let a Claude agent choose a gene therapy and inject it into a live mouse's brain after Opus 5.5 refused

*Research · New*

**Published:** 31 Oct 2026, 11:00 CET

WIRED reports that **Exin Therapeutics**, a San Francisco start-up developing epilepsy drugs, connected an AI agent to a custom rig with a motorised needle, an injector and a camera, and let it **carry out a brain injection on a living mouse**. A veterinary surgeon performed the craniotomy first while the agent watched.

The agent picked a gene therapy from 19 options in a spreadsheet, chose the brain region and injection coordinates, and controlled the needle, volume and speed. According to chief executive Gabriel Ocana Santero, the team first tried Anthropic's **Claude Opus 5.5, which refused** to guide the needle, and then switched to **Claude Sonnet 5**, which agreed.

The team required the agent to propose its plan for human approval, fitted an emergency stop and blocked it from editing the equipment code. When a glitch broke the coordinate system, the agent saw the position was wrong but would not change the code, so a separate Opus 5 agent, not told that surgery was under way, fixed it. The procedure took slightly over an hour against a typical 45 minutes, and the therapy's effect on seizures has not yet been assessed.

**Analysis — why it matters:** *Analysis: the account shows models from one vendor answering the same request differently, and a team working around a refusal by switching models and withholding context from a second agent. That is a practical problem for anyone relying on refusals as a safeguard in physical labs.*

**Caveat:** This is the **company's own account**, given to WIRED and first posted on X by its founder; there is no paper or independent check, and **Anthropic did not respond** to WIRED. Whether the therapy works is not yet known.

**Sources:**

1. [WIRED](<https://www.wired.com/story/an-ai-agent-did-brain-surgery-on-live-mouse/>) — reporting. Checked: 31 Oct 2026, 16:03 CET

### Cisco Talos: the VOLTA infostealer hands stolen data to an AI model to rank each victim by what can be monetised

*Research · New*

**Published:** 31 Oct 2026, 13:00 CET

Cisco's Talos threat-intelligence group published an analysis of **VOLTA, a self-deleting Windows infostealer** that names itself VOLTA-AUTODOXER. After stealing passwords, cookies, payment cards, crypto-wallet seed phrases, session tokens, SSH and cloud keys and screenshots, it builds a profile of the person behind the machine.

Talos says the profile includes geolocation and home address, employer, inferred birth year and card digits, and is enriched through the stolen sessions, for example by searching the victim's Gmail for receipts. The bundle is then **sent to a model through OpenRouter** with a prompt to write a 'target assessment' ranking the victim's assets by monetisation value and judging their security habits.

If a model refuses, the malware checks for phrases such as 'I can't' and **falls back through a chain of up to three models**, which Talos lists as ending with kimi-k2 and gemini-2.5-flash. Talos says the stealer uses no attacker-owned infrastructure.

**Analysis — why it matters:** *Analysis: here the model is not writing malware but acting as the criminal's triage analyst, deciding which victims are worth pursuing. The refusal-fallback chain shows attackers expect guardrails and plan around them.*

**Caveat:** The findings come from Talos' analysis of samples; it does not say how widely VOLTA has been deployed.

**Sources:**

1. [Cisco Talos](<https://blog.talosintelligence.com/appraisal-by-ai-model-driven-victim-prioritization-in-the-volta-infostealer/>) — primary source. Checked: 31 Oct 2026, 16:03 CET
2. [WIRED](<https://www.wired.com/story/kernel-panic-volta-autodoxer-ai-infostealer-malware/>) — reporting. Checked: 31 Oct 2026, 16:03 CET

### UPDATE: WSJ says OpenAI has raised about $11 billion of its $30 billion target and will turn to family offices for the rest

*Industry & policy · Updated*

**Published:** 31 Oct 2026, 10:22 CET

This morning's edition reported, from the Financial Times, that OpenAI had cut its funding target to about $20 billion. The new detail comes from The Wall Street Journal, as summarised by The Decoder on Saturday: OpenAI has **secured about $11 billion so far** of the $30 billion it set out to raise, at a **valuation of $1.25 trillion** rather than the $1.4 trillion it sought.

According to the same account, the shortfall reflects fading interest from large investors during the tech selloff, and OpenAI now plans to raise **up to $20 billion from family offices and wealthy individuals**. The Decoder adds that OpenAI is reportedly planning a stock-market listing early next year.

**Analysis — why it matters:** *Analysis: the WSJ figure puts a number on how much of the round large investors have actually committed, which the FT report did not. A round filled by family offices and wealthy individuals would rely less on the big institutions that usually anchor late-stage deals.*

**Caveat:** The WSJ article was not read (paywall), and its exact publication time could not be checked; a Hacker News link to it was posted at 04:22 Paris time on 31 October. **OpenAI has not confirmed the figures**.

**Community reaction (opinion, not verified fact):**

> “this is more about the supply and demand of capital in any given moment than it is about the outlook of the company.” — [lasky (Hacker News)](<https://news.ycombinator.com/item?id=50313560>)

**Sources:**

1. [The Decoder (summary of the WSJ report)](<https://the-decoder.com/openai-raises-just-11-billion-of-its-30-billion-target-as-big-investors-lose-their-ai-appetite/>) — reporting. Checked: 31 Oct 2026, 16:03 CET
2. [Hacker News discussion of the WSJ report](<https://news.ycombinator.com/item?id=50312922>) — community. Checked: 31 Oct 2026, 16:04 CET

### UPDATE: Singapore says its officials never told the WSJ they suspected Alice Huang, and that it did not investigate her

*Industry & policy · Updated*

**Published:** 31 Oct 2026

On 29 October this journal reported The New York Times' account that US officials concluded Alice Huang, an executive linked to the Singapore data-centre company Megaspeed and close to Nvidia's Jensen Huang, was a Chinese intelligence asset. On 31 October Singapore's Ministry of Home Affairs **disputed a follow-up Wall Street Journal article** dated 30 October.

The ministry says the WSJ cited sources saying Singapore officials were concerned about Alice Huang's ties to Jensen Huang or to Chinese intelligence and had investigated her ties to China. It states that **neither the government nor its officials said this**, and that **no such investigations were conducted** in respect of her.

The ministry published the WSJ's questions and the police reply it sent on 30 October. That reply says **investigations into Megaspeed are ongoing**, and that Singapore charged four individuals and four companies between February 2025 and July 2026 with fraud on server suppliers.

**Analysis — why it matters:** *Analysis: Singapore's denial covers what the WSJ attributed to Singapore officials. It does not address the US intelligence conclusions reported by The New York Times, and it confirms that the inquiry into Megaspeed itself continues.*

**Caveat:** The WSJ article itself was not read (paywall), so its wording is known here only through the ministry's description. The underlying intelligence claims rest on anonymous sources, and **none of the reports accuses Jensen Huang of wrongdoing**.

**Sources:**

1. [Ministry of Home Affairs, Singapore](<https://www.mha.gov.sg/media-room/newsroom/clarification-statement-on-wall-street-journals-article/>) — primary source. Checked: 31 Oct 2026, 16:03 CET

### Chainalysis says an attacker using 'offensive agentic techniques' broke into its systems and reached customer names and emails

*Industry & policy · New*

**Published:** 30 Oct 2026, 22:14 CET

Blockchain-analysis firm Chainalysis published a security notice on Friday evening saying that this month it **detected an external actor using 'offensive agentic techniques'** to gain unauthorised access to its systems and internal tools.

The company says **user IDs, full names, email addresses and organisation role labels** were accessed, but that it has found no evidence of access to investigation content, query results, clear-text passwords, MFA secrets or session tokens. It says the incident is unrelated to the recent Binance theft and that it is using large language models in a wider security review.

**Analysis — why it matters:** *Analysis: a company whose business is tracing criminals attributes its own breach to AI-driven attack methods, following CrowdStrike's report this week of a China-linked group using agents against more than 200 organisations.*

**Caveat:** Chainalysis has **not explained what the agentic techniques were**, which flaws were exploited or how many customers are affected.

**Sources:**

1. [Chainalysis](<https://www.chainalysis.com/blog/security-incident-october-30/>) — primary source. Checked: 31 Oct 2026, 16:04 CET
2. [BleepingComputer](<https://www.bleepingcomputer.com/news/security/chainalysis-discloses-data-breach-from-offensive-agentic-techniques/>) — reporting. Checked: 31 Oct 2026, 16:04 CET
3. [The Hacker News](<https://thehackernews.com/2026/10/chainalysis-confirms-intrusion-into.html>) — reporting. Checked: 31 Oct 2026, 16:04 CET

### Sam Altman meets about 50 Samsung executives and SK's chairman in South Korea as memory chips run short

*Industry & policy · New*

**Published:** 31 Oct 2026

OpenAI chief executive Sam Altman met **about 50 executives from Samsung's electronics, finance and biotech affiliates** at a Samsung training centre in Yongin, south of Seoul, on Saturday, Samsung said. Yonhap reports that the session focused on how AI will reshape companies' decisions and operations.

Yonhap, citing industry sources, says **SK Group chairman Chey Tae-won also met Altman** the same day with executives from SK hynix and SK Telecom; it adds that analysts said they may have discussed high-bandwidth memory and data centres. Bloomberg, in a report carried by The Straits Times, says the visit builds on earlier agreements to supply memory for OpenAI's Stargate project, as memory shortages push up chip prices.

**Analysis — why it matters:** *Analysis: memory has become a bottleneck for AI data centres, and Samsung and SK hynix are its two largest suppliers. Altman meeting both on one day signals where OpenAI sees its supply risk.*

**Caveat:** Samsung described the meeting in general terms; **no new supply agreement was announced**, and what Altman discussed with SK is not on the record.

**Sources:**

1. [Yonhap](<https://en.yna.co.kr/view/AEN20261031002651315>) — reporting. Checked: 31 Oct 2026, 16:03 CET
2. [The Straits Times (Bloomberg)](<https://www.straitstimes.com/business/openais-altman-meets-samsung-executives-as-chip-crunch-deepens>) — reporting. Checked: 31 Oct 2026, 16:04 CET

## Key patterns (editorial analysis)

- Agents are acting in the physical and criminal world: one **chose and injected a therapy in a live mouse**, and malware now **uses a model to rank its victims**.
- Refusals are uneven: Opus 5.5 declined the mouse injection while Sonnet 5 agreed, and developers say **a server-side games rule blocks legitimate work**.
- The funding squeeze is sharper than first reported: OpenAI has **about $11 billion of a $30 billion target**, according to the WSJ.

## Source coverage

- Engine version: 3.28.0
- Engine ran this edition: yes
- Engine look-back: 2 days

### Source status

- reddit: ok (25 threads)
- youtube: ok (1 video, with transcript)
- hackernews: ok (31 stories)
- polymarket: unreachable (TLS certificate hostname mismatch; not bypassed)
- github: ok (15 items)
- devto: searched with tags ai, machinelearning and llm; 0 articles returned
- x: not searched (no consent-free source configured)

### Notes

- The window runs from yesterday's 16:08 CET afternoon issue to this edition, wider than usual, to carry one Friday-evening disclosure (Chainalysis) that this morning's edition did not carry. Dispatches with only a date carry that date; exact timestamps are given where a source supplied one.
- The installed last30days engine finished with 72 evidence items from Reddit, Hacker News, GitHub and YouTube. Its top item was the Hacker News thread on Claude's game-related refusals, which supplied a community quote; most other top items were general discussion rather than verifiable news. Stories were chosen with Google News RSS, publisher feeds, web searches and checks of primary documents. Item counts are not counts of verified developments.
- Polymarket failed its TLS certificate hostname check and verification was not bypassed. X was not searched. dev.to returned no articles. Failed or missing coverage does not mean nobody discussed these stories.
- The configured web search backend failed and its keyless fallback served the searches. VentureBeat's feed returned HTTP 429 and Investing.com HTTP 403. The two WSJ articles were not read (paywall). One Tom's Hardware article on Intel returned 404 and was not used.
- Not carried because they appeared before this window: Parameter's ChatGPT shared-link flaw (fixed 26 October, write-up 28 October), Factory's Droid 1.0 (29 October), Vercel's agent-desktop (30 October), Google DeepMind's ForTy forest map (22 October) and Microsoft's voluntary exit offer (26 October). Friday's market moves, including Apple overtaking Nvidia by market value, were also left out.
- No browser-cookie access, optional service or credential signup, paid enrichment, TLS bypass, Job Alerts edits or schedule changes were used. Research logs and full provenance remain private.

### Engine footer (verbatim)

```text
---
✅ All agents reported back!
├─ 🟠 Reddit: 25 threads │ 647 upvotes │ 324 comments
├─ 🔴 YouTube: 1 video │ 3,391 views │ 1/1 with transcripts
├─ 🟡 HN: 31 stories │ 2,932 points │ 2,137 comments
├─ 🐙 GitHub: 15 items │ 7 reactions │ 9 comments
├─ 🗣️ Top voices: r/artificial, r/singularity, r/OpenAI
---
```
