# The AI Gazette — Afternoon edition, Sunday 15 November 2026

*Models, machines, and matters of consequence*

- Issue: 2026-11-15-afternoon
- Issued: 15 Nov 2026, 16:09 CET (Paris)
- Reporting window: 13 Nov 2026, 17:00 CET to 15 Nov 2026, 16:09 CET
- Timezone: Europe/Paris
- Previous issue: 2026-11-15-morning
- Price: Complimentary

## Editor's note

Ten hours since the morning edition, through a Sunday with no new frontier model release. Inside the normal window: Megaspeed's statement that **Alice Huang left in August 2025**, a South Korean exam cheating confession, a coolant spill at an xAI facility in Mississippi and Japan's plan for military AI guidelines. The window is widened to 17:00 on Friday 13 November, just under 48 hours, to carry three verified items no earlier edition ran: Cursor's account of how **a key issued to Fireworks** led to the tampered Claude Code extension, Bland's Tofu-1 speech model, and South Africa's AI visit to Silicon Valley. Vendor claims are labelled as such.

## The News

### Bland opens a research preview of Tofu-1, a full-duplex speech-to-speech model for phone calls

*Models · New*

**Published:** 13 Nov 2026

San Francisco voice-AI company Bland has introduced **Tofu-1**, which it describes as a **full duplex speech-to-speech model** built for calls in poor conditions: from moving cars and hospital rooms, over weak signal, or with several people talking at once. Bland announced it on 13 November, and MarkTechPost reported it on Sunday.

Bland says Tofu-1 listens while it speaks, so callers can interrupt or correct it mid-sentence, keeps the call moving while it works on a task, tells speakers apart and can generate several speakers and the sound of the room. Unlike cascaded voice systems that turn speech into text and back, it works on the audio itself, the company says.

Access is a **research preview for a limited number of enterprises**. Bland has not published the model's internal architecture, and its parameter count and turn-taking latency are not disclosed, MarkTechPost notes.

**Analysis — why it matters:** *Analysis: phone agents are moving from transcribe-then-reply pipelines to models that handle audio end to end, which matters most in the noisy, interrupted calls that cascades handle badly.*

**Caveat:** All capability claims are Bland's own; no independent evaluation or benchmark result was available, and the model is not generally available.

**Sources:**

1. [Bland: Tofu-1, speech-to-speech built for high-stakes calls](<https://www.bland.ai/speech-to-speech>) — primary source. Checked: 15 Nov 2026, 16:06 CET
2. [MarkTechPost: Bland launches Tofu-1, a full-duplex speech-to-speech model for calls](<https://www.marktechpost.com/2026/11/15/bland-tofu-1-full-duplex-speech-to-speech-model/>) — reporting. Checked: 15 Nov 2026, 16:06 CET

### UPDATE: Cursor says a key it had issued to Fireworks, exposed by Fireworks, opened the way to the tampered Claude Code extension

*Coding & agents · Updated*

**Published:** 13 Nov 2026

Update to the 30 and 31 October editions on the tampered Claude Code extension in Cursor's marketplace. The new development: in a post dated 13 November, Cursor says the attack **started at Fireworks**. An attacker obtained an access key Cursor had issued to the inference company, which Cursor says was exposed by Fireworks, and used it to copy data from a read-only storage bucket the two used to share data.

That bucket held limited coding agent traces, mostly from 2025, from sessions not in Privacy Mode that Cursor was permitted to use for training. Some traces contained credentials that had not been redacted, exposing API credentials of **less than 0.01% of customers**, Cursor says. From there the attacker reached select SaaS tools and accessed archived non-production source code repositories, limited support data and email conversations, usage metrics and contact details, and some credentials users had sent to Cursor's support team.

On 29 October a stolen credential let the attacker place malicious copies of Anthropic's Claude Code extension, versions 2.1.312 and 2.1.313, directly on the cache that serves Cursor's VS Code extension marketplace. Cursor says **at most 5,000 users** may have received the build, which was available for about 11 hours, and that the marketplace source, Open VSX, never had the malware.

Cursor says it has **moved all inference traffic off Fireworks**, rotated credentials and believes the incident is contained, with the last attacker activity seen on 1 November and blocked. Fireworks' security bulletins list an October 2026 incident involving unauthorized use of internal Fireworks credentials. The Hacker News reported Cursor's update on Sunday.

**Analysis — why it matters:** *Analysis: the chain ran through a model vendor holding training traces rather than through Cursor's release pipeline, so the data a coding tool shares with AI training and inference partners is part of its attack surface.*

**Caveat:** This account and its exposure figures come from Cursor's own investigation and were not independently verified; Fireworks' bulletins were checked only for the incident listing, not for what they say about Cursor's key. Cursor says users who installed the tampered versions should follow its October security notice, because uninstalling the extension alone may not be enough.

**Sources:**

1. [Cursor: An update on our recent security incident](<https://cursor.com/blog/security-incident-update>) — primary source. Checked: 15 Nov 2026, 16:06 CET
2. [Fireworks AI: Security bulletins](<https://fireworks.ai/security/bulletins>) — primary source. Checked: 15 Nov 2026, 16:06 CET
3. [The Hacker News: Stolen Fireworks AI key led to Cursor data breach and trojanized Claude Code extension](<https://thehackernews.com/2026/11/stolen-fireworks-ai-key-led-to-cursor.html>) — reporting. Checked: 15 Nov 2026, 16:06 CET

### UPDATE: Megaspeed says Alice Huang left the company in August 2025 and hires outside lawyers to investigate reports about its business

*Industry & policy · Updated*

**Published:** 15 Nov 2026, 09:20 CET

Update to this week's editions on Jensen Huang's resignation and the Megaspeed affair. The new development: Megaspeed, the Singapore-based cloud computing company at the centre of the case, said on Sunday that Alice Huang **officially left Megaspeed effective August 30, 2025** and has no current role there, in an emailed statement shared with CNBC and also reported by Reuters.

Megaspeed said recent media reports about its business, supply chain and global operations are not supported by verifiable evidence, and that it has **retained external legal counsel** to conduct a thorough internal investigation. It said it does not comment on Ms Huang's personal and private matters, and that its control frameworks are designed to comply with US export control requirements.

Reuters notes that Megaspeed has not been found to have violated the rules and that the US government and Nvidia did not respond immediately to requests for comment. Research group C4ADS has said, citing corporate records, that Alice Huang became Megaspeed's **controlling shareholder in March 2023**, the Reuters report carried by The Straits Times adds.

**Analysis — why it matters:** *Analysis: the statement dates Alice Huang's departure but does not address the reports about where Megaspeed's Nvidia chips went, which is what the export-control inquiries and Nvidia's board investigation turn on.*

**Caveat:** The departure date and the description of Megaspeed's compliance controls are the company's own claims and were not independently verified. US officials suspect Alice Huang of being a Chinese intelligence asset, according to reports cited by CNBC and Reuters; Beijing has denied the allegation, and no authority has publicly found Megaspeed in breach of US export rules.

**Community reaction (opinion, not verified fact):**

> “if true i'm GLAD he smuggled the chips to China so they could release such good open weights” — [u/Limp\_Classroom\_2645 on r/technology](<https://reddit.com/r/technology/comments/1xwh2q4/exportbanned_nvidia_chips_are_behind_chinas_most/19snx0maqv9oj/>)

> “It needs to be a lot more than Jensen.” — [u/Durtle\_Turtle on r/technology](<https://www.reddit.com/r/technology/comments/1xvsezb/nvidia_allegedly_engineered_scarcity_by_funding/>)

**Sources:**

1. [CNBC: Megaspeed says Alice Huang left in 2025 as it launches internal probe](<https://www.cnbc.com/2026/11/15/megaspeed-alice-huang-probe-nvidia-scandal.html>) — reporting. Checked: 15 Nov 2026, 16:06 CET
2. [The Straits Times (Reuters): Megaspeed says Alice Huang left company in August 2025](<https://www.straitstimes.com/business/megaspeed-says-alice-huang-left-company-in-august-2025>) — reporting. Checked: 15 Nov 2026, 16:06 CET

### Top scorer in South Korea's tax accountant exam admits he cheated with a hidden camera and generative AI

*Industry & policy · New*

**Published:** 15 Nov 2026

Han Won-seok, 34, who placed first in South Korea's 2026 certified tax accountant exam, admitted on Sunday that he **cheated using a miniature camera, a smartphone and generative AI**, in a video on his lawyer's YouTube channel, the BBC and The Korea Herald report. He said he photographed the questions, sent them to an AI and checked the answers on his phone, in both rounds of the exam.

He had scored 397.5 out of 400 in the first round, **159 of 160 questions correct**, which drew online suspicion; he had earlier denied cheating. The Korea Herald reports that he also admitted using the same methods in the first round of the certified public accountant exam in March. Seoul Metropolitan Police Agency told Yonhap it had received a written confession through his lawyer and assigned the case to investigators, the BBC reports.

The government said those found to have used AI to cheat in the exam will have their **qualification revoked and be banned from retaking it for five years**, according to the BBC, and the president's policy chief said new measures against cheating would be introduced.

**Analysis — why it matters:** *Analysis: the case shows a general-purpose AI assistant defeating a professional licensing exam built on speed and recall, and the response announced so far is enforcement and penalties rather than a change in how the test is set.*

**Caveat:** The account of how he cheated is his own confession, and the police investigation has only begun. The penalties were reported by the BBC from a government statement that was not read directly.

**Sources:**

1. [BBC: South Korea's top scorer in tax accountancy exam admits cheating](<https://www.bbc.com/news/articles/ckvg2ezvpe08o>) — reporting. Checked: 15 Nov 2026, 16:06 CET
2. [The Korea Herald: Tax accountant exam's top scorer admits to cheating with AI](<https://www.koreaherald.com/article/10937374>) — reporting. Checked: 15 Nov 2026, 16:06 CET
3. [The Korea Times: Top tax accountant exam scorer admits to using AI to cheat](<https://www.koreatimes.co.kr/southkorea/law-crime/20261115/top-tax-accountant-exam-scorer-admits-to-using-ai-to-cheat>) — reporting. Checked: 15 Nov 2026, 16:06 CET

### Thousands of gallons of propylene glycol spill from a tank at an xAI facility in Southaven, Mississippi, and reach a drainage ditch

*Industry & policy · New*

**Published:** 15 Nov 2026, 14:37 CET

A spill of **about 5,000 to 6,000 gallons of propylene glycol** from a tank at an xAI facility in Southaven, Mississippi, reached a nearby drainage ditch on Saturday, the Mississippi Department of Environmental Quality said, Action News 5 reports. Propylene glycol is used in antifreeze, deicers and heat-transfer fluids, also known as coolants.

Crews installed berms upstream and downstream to contain the release, and a contractor has been recovering the material with vacuum trucks since about 10 a.m. on Saturday, with MDEQ emergency staff assisting, according to MDEQ. **xAI had not commented** when the station published.

Background (6 November): Mississippi Today reported that MDEQ had released details of penalties against SpaceXAI for starting construction on its Southaven data centre facilities **without the required stormwater permits**, and that the company had told investors the fines could reach as much as 6.1 million dollars.

**Analysis — why it matters:** *Analysis: the Southaven sites already face state penalties over construction permits, so a coolant release into local drainage adds to scrutiny of how fast the company is building there.*

**Caveat:** The volume and the response details come from MDEQ via Action News 5; the cause of the tank failure and any environmental impact were not reported. Mississippi Today was read through an Internet Archive snapshot dated 10 November.

**Sources:**

1. [Action News 5: Chemical spill at xAI facility in Southaven reaches drainage ditch](<https://www.actionnews5.com/2026/11/15/chemical-spill-xai-facility-southaven-reaches-drainage-ditch/>) — reporting. Checked: 15 Nov 2026, 16:06 CET
2. [Mississippi Today: SpaceXAI started Southaven data center without water permits](<https://mississippitoday.org/2026/11/06/spacexai-southaven-data-center-fines-mdeq/>) — reporting. Checked: 15 Nov 2026, 16:06 CET

### Japan's Defense Ministry will publish guidelines for defence use of AI at the end of November, Koizumi says

*Industry & policy · New*

**Published:** 15 Nov 2026

Japanese Defense Minister Shinjiro Koizumi said on Sunday that the ministry will release **guidelines for the defense-related use of AI at the end of this month**, Jiji Press reports. They will update the ministry's AI basic policy compiled in July 2024 and apply to ministry staff and Self-Defense Forces personnel.

Koizumi named three pillars: ensuring **humans make decisions and bear responsibility** for the outcomes of AI use, turning data into power to defend the country, and balancing rapid adoption of AI with enhanced safety. "We will not hesitate to make a necessary revision since AI is an area where things change rapidly," he said, according to Jiji.

**Analysis — why it matters:** *Analysis: the announcement states intent; the substance will be in the text due at the end of November, including how far human responsibility is required for AI used in operations.*

**Caveat:** The guidelines have not been published; this is the minister's description of them as reported by Jiji Press.

**Sources:**

1. [Jiji Press: Japan Defense Ministry to release AI guidelines at end-Nov.](<https://jen.jiji.com/jc/eng?g=eco&k=2026111500349>) — reporting. Checked: 15 Nov 2026, 16:06 CET
2. [Nippon.com (Jiji Press): Japan Defense Ministry to release AI guidelines at end-Nov.](<https://www.nippon.com/en/articles/-/57469>) — reporting. Checked: 15 Nov 2026, 16:06 CET

### South Africa's Ramaphosa arrives in Silicon Valley with eight ministers for a week-long AI and investment visit

*Industry & policy · New*

**Published:** 14 Nov 2026

President Cyril Ramaphosa arrived in California on Saturday, 14 November, for a **working visit to Silicon Valley** on artificial intelligence, leading a delegation of officials, business leaders, researchers, technical experts and university students, the South African Presidency says. Ministers of finance, trade, energy, communications and four other portfolios travel with him.

The programme includes meetings with technology companies, investors and researchers and a South Africa AI Opportunity gathering on **AI infrastructure, data centres, computing capacity and energy**. The Presidency says South Africa wants to position itself as a competitive AI hub on the continent while safeguarding digital sovereignty, data protection and responsible AI governance.

Semafor reports that the itinerary includes meetings with Google, Cisco, Palo Alto Networks and Microsoft, and describes the trip as a **week-long push to court billions** in American AI infrastructure investment.

**Analysis — why it matters:** *Analysis: the visit pairs an investment pitch for data centres and compute with explicit conditions on sovereignty and data protection, the same balance other mid-sized economies are trying to strike with US AI companies.*

**Caveat:** No agreements or investment figures had been announced; the aims are the Presidency's own statements.

**Sources:**

1. [The Presidency of South Africa: President Ramaphosa arrives in California for high-level artificial intelligence learning visit to Silicon Valley](<https://www.thepresidency.gov.za/president-ramaphosa-arrives-california-high-level-artificial-intelligence-learning-visit-silicon>) — primary source. Checked: 15 Nov 2026, 16:06 CET
2. [SAnews: President Ramaphosa arrives in California](<https://www.sanews.gov.za/south-africa/working-visit-president-ramaphosa-arrives-california>) — primary source. Checked: 15 Nov 2026, 16:06 CET
3. [Semafor: South Africa's Ramaphosa takes AI pitch to Musk's turf](<https://www.semafor.com/article/11/13/2026/s-africas-ramaphosa-takes-ai-pitch-to-musk-turf>) — reporting. Checked: 15 Nov 2026, 16:06 CET

## Key patterns (editorial analysis)

- Security incidents now travel through AI supply chains: Cursor traces its breach to **a key shared with an inference vendor**.
- Generative AI is testing institutions built on trust, from Korea's licensing exams to **Japan's planned rules for military AI**.
- Governments are courting AI investment while tightening oversight, as South Africa's Silicon Valley delegation and the Megaspeed inquiries show.

## Source coverage

- Engine version: 3.31.0
- Engine ran this edition: yes
- Engine look-back: 2 days

### Source status

- reddit: ok, partial (20 threads; 25 requests blocked with HTTP 403, 11 archive queries failed with HTTP 422 and 3 got no response; Arctic Shift archive supplied posts)
- hackernews: ok (29 stories)
- github: ok (10 items)
- devto: ok (12 articles; tags ai and llm)
- youtube: not searched (yt-dlp not available on this machine)
- polymarket: not used: blocked in France (ANJ)
- x: not searched (no consent-free source configured)

### Notes

- The installed last30days engine finished (exit 0) with 71 evidence items from Reddit, Hacker News, dev.to and GitHub; its top clusters were stories earlier editions already ran (the FAA ground stop, the Nvidia financing report, the 13 November Claude outage). Most stories here were found with 16 Google News RSS queries, publisher feeds, the Hacker News search API, post-engine web supplements and the source pages. Item counts are not counts of verified developments.
- Window: widened to start at 17:00 on 13 November, just under 48 hours before this edition, to carry Cursor's 13 November incident update, Bland's 13 November Tofu-1 announcement and the South African Presidency's 14 November statement, which no earlier edition ran. The Megaspeed, South Korea, xAI and Japan stories fall inside the normal window since the morning edition.
- Polymarket not used: blocked in France (ANJ). X not searched. YouTube not searched (not available on this machine). Reddit returned results, but 25 of its requests were blocked (HTTP 403), so Reddit coverage was partial. Missing coverage does not mean nobody discussed these stories.
- Read through a non-direct route: Mississippi Today (HTTP 403) through an Internet Archive snapshot dated 10 November; The Hacker News (HTTP 403 to a plain request) through the host's page-extraction tool; MarkTechPost (HTTP 403 to a plain request) on a direct retry by the fetch script. Paywalled and not read or carried: the Financial Times report on Congress and AI chip export rules and The New York Times report on Howard Lutnick and chip rules.
- Newsletter leads from the Iris mail bot: not carried were Inkling 2 Small's open weights (released 12 November, outside the 48-hour limit), Anthropic's IPO price range (carried 10 and 13 November), Nvidia's customer financing (carried 14 November), Gemini Robotics 2.5 (carried 10 November), the Claude Fable 5.2 operating-system demonstration (announced 9 November), Claude for Manufacturing and Gemini 4 Hydrogen in Search (handled in the morning edition) and an e-signature tool that is not an AI story.
- Not carried: Meituan's LongCat-2.5 weights (repository created 4 November), Crissy Field's Lovable data-exposure research (published 2 November), L3Harris's statement on the 13 November ground stop (no AI finding), and market commentary on Anthropic's listing and data-centre stocks.
- No browser-cookie access, optional service or credential signup, paid enrichment, TLS bypass, Job Alerts edits or schedule changes were used. Research logs and full provenance remain private.

### Engine footer (verbatim)

```text
---
✅ All agents reported back!
├─ 🟠 Reddit: 20 threads │ 58,260 upvotes │ 4,262 comments
├─ 🟡 HN: 29 stories │ 2,502 points │ 2,047 comments
├─ 👩‍💻 dev.to: 12 articles │ 278 reactions │ 77 comments
├─ 🐙 GitHub: 10 items │ 43 reactions │ 95 comments
├─ 🗣️ Top voices: r/technology, r/LocalLLaMA, r/artificial
---
```
