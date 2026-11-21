# The AI Gazette — Afternoon edition, Saturday 21 November 2026

*Models, machines, and matters of consequence*

- Issue: 2026-11-21-afternoon
- Issued: 21 Nov 2026, 16:08 CET (Paris)
- Reporting window: 20 Nov 2026, 21:00 CET to 21 Nov 2026, 16:08 CET
- Timezone: Europe/Paris
- Previous issue: 2026-11-21-morning
- Price: Complimentary

## Editor's note

Ten hours since the morning edition, a quiet Saturday, and **no new frontier model**. The window was widened back to 21:00 on Friday to pick up two stories the morning edition missed: Thinking Machines' laptop-sized open model **Inkling 2 Mini**, and Etsy's promise to revise its AI-training terms after sellers closed their shops. Overnight in Geneva, UN weapons talks ended with a **two-year mandate** to draft rules on autonomous weapons, without agreeing that those rules will be binding.

## The News

### Thinking Machines releases Inkling 2 Mini, a 26-billion-parameter open-weights model small enough to run on a 32GB Mac

*Models · New*

**Published:** 20 Nov 2026

Thinking Machines Lab released **Inkling 2 Mini** on Friday, an open-weights model under the **Apache 2.0 licence** that it says is small enough to run on a laptop. The weights are on Hugging Face, the model is on the company's Tinker platform, and Ollama lists it for Macs with **32GB or more of memory**. It was first posted to Hacker News at 21:12 Paris time on Friday, after the previous afternoon edition had closed, and the morning edition did not carry it.

Inkling 2 Mini is a mixture-of-experts model with **26.4 billion total parameters** and 3.4 billion active per token. It is a looped transformer: the middle 12 of its 24 layers run three times for every token, which the company says lets it reason more without writing more tokens. Most of its weights were trained and ship in 4-bit NVFP4, for a memory footprint of about 20GB.

Thinking Machines says the model leads every open-weights model under 100 billion parameters on DeepSWE v1.1 (48.2%) and Vals Index v2.2 (46.5%). It also says the model is weaker on multi-turn chat and on instructions with many constraints, where it trails Qwen3.8-27B. Artificial Analysis, which tests models independently, placed it at **20 on its Intelligence Index**, level with Qwen3.8 27B, at $0.59 per task against $3.53.

The lab also released a research variant with a variable number of loops, used to test whether looping hides reasoning from people reading a model's chain of thought. It reports that the chain of thought got shorter with more loops but stayed legible, and that the model did not score higher on tests of agentic sabotage as loops were added.

**Analysis — why it matters:** *Editorial analysis: a **looped transformer good enough for agentic coding** at laptop size is a new design point for open weights; tests beyond one index will show whether the benchmark lead holds.*

**Caveat:** The benchmark results are Thinking Machines' own, except the Artificial Analysis index. The release page gives only the date; the time comes from the first Hacker News post.

**Community reaction (opinion, not verified fact):**

> “I think this may be the first public example of a looped transformer model good enough for real world use cases?” — [gchadwick (Hacker News)](<https://news.ycombinator.com/item?id=50581821>)

> “This is bonkers good if these benchmarks hold up in real-world scenarios.” — [montroser (Hacker News)](<https://news.ycombinator.com/item?id=50581726>)

**Sources:**

1. [Thinking Machines: Introducing Inkling 2 Mini](<https://thinkingmachines.ai/news/inkling-2-mini/>) — primary source. Checked: 21 Nov 2026, 16:06 CET
2. [Thinking Machines: Inkling 2 Mini model card](<https://thinkingmachines.ai/model-card/inkling-2-mini/>) — primary source. Checked: 21 Nov 2026, 16:06 CET
3. [Hugging Face: thinkingmachines/Inkling-2-Mini](<https://huggingface.co/thinkingmachines/Inkling-2-Mini>) — primary source. Checked: 21 Nov 2026, 16:06 CET
4. [Ollama: inkling-2-mini](<https://ollama.com/library/inkling-2-mini>) — primary source. Checked: 21 Nov 2026, 16:06 CET
5. [Artificial Analysis: Thinking Machines has released Inkling 2 Mini](<https://artificialanalysis.ai/articles/inkling-2-mini>) — reporting. Checked: 21 Nov 2026, 16:06 CET
6. [Hacker News: discussion of Inkling 2 Mini](<https://news.ycombinator.com/item?id=50581260>) — community. Checked: 21 Nov 2026, 16:08 CET

### UN weapons talks end with a two-year mandate to draft rules on autonomous weapons, but no commitment that they will be binding

*Industry & policy · New*

**Published:** 21 Nov 2026

The 128 states party to the UN **Convention on Certain Conventional Weapons** agreed in Geneva at about 04:45 Paris time on Saturday to 'elaborate' an international instrument on lethal autonomous weapons systems **over the next two years**. The review conference had met since Monday; talks on the final wording ran through the night after Russian objections over procedure led to some formal sessions being called off, diplomats told Al Jazeera.

Close to 100 states had backed legally binding rules on weapons that can kill without a human making the final decision. A group of seven, Austria, Belgium, Brazil, Ireland, Mexico, New Zealand and Panama, wanted a treaty negotiated within a year. Decisions require consensus, and the United States, Russia and Israel opposed binding rules, Al Jazeera and CNA reported. Some states rejected the word 'negotiate', so the text says 'elaborate', and **whether the result will bind anyone is left open**.

UN disarmament chief Izumi Nakamitsu called the outcome a 'significant achievement' and said 'the path to or possibility to have a legally binding instrument is still open'. A group of governmental experts will recommend the instrument's legal form, including whether it should be a binding protocol. The International Committee of the Red Cross said it regretted the lack of a clear negotiating mandate, and the Stop Killer Robots coalition called the mandate 'watered down'.

Separately, US Treasury Secretary Scott Bessent told CNBC on Friday that Presidents Trump and Xi had agreed at their Shenzhen meeting that humans should always be involved in military decisions made with AI, Reuters reported. No written text of that agreement was found.

**Analysis — why it matters:** *Editorial analysis: the forum that has discussed autonomous weapons for more than a decade now has a **2028 horizon but no guarantee of binding rules**, while campaigners say such weapons are already in use.*

**Caveat:** The agreed mandate text was not found online; its terms here come from the conference chair and UN officials as reported by news agencies. Reports put the close between 04:30 and 05:00 Geneva time.

**Sources:**

1. [Al Jazeera: Nations agree to 'elaborate' on rules for AI-run 'killer robots' by 2028](<https://www.aljazeera.com/news/2026/11/21/nations-agree-to-draft-rules-for-killer-robots-at-arms-control-summit>) — reporting. Checked: 21 Nov 2026, 16:06 CET
2. [The Guardian: International talks on controlling use of autonomous weapons collapse](<https://www.theguardian.com/technology/2026/nov/21/international-talks-control-ai-autonomous-weapons-collapse>) — reporting. Checked: 21 Nov 2026, 16:06 CET
3. [Anadolu: UN sees progress on autonomous weapons regulation despite lack of binding treaty mandate](<https://www.aa.com.tr/en/world/un-sees-progress-on-autonomous-weapons-regulation-despite-lack-of-binding-treaty-mandate/4133032>) — reporting. Checked: 21 Nov 2026, 16:06 CET
4. [CNA: States agree to UN talks aiming to regulate 'killer robots' by 2028](<https://www.channelnewsasia.com/world/united-nations-regulate-killer-robots-weapons-6571256>) — reporting. Checked: 21 Nov 2026, 16:06 CET
5. [NPR: Killer robots, the race to control weapons that can decide who lives or dies](<https://www.npr.org/2026/11/21/nx-s1-6047916/killer-robots-un-drones>) — reporting. Checked: 21 Nov 2026, 16:06 CET
6. [Defense News (Reuters): Trump, Xi agreed that military AI decisions should involve humans, Bessent says](<https://www.defensenews.com/global/asia-pacific/2026/11/20/trump-xi-agreed-that-military-ai-decisions-should-involve-humans-bessent-says/>) — reporting. Checked: 21 Nov 2026, 16:06 CET

### Etsy says it will revise new terms that let it and its partners train AI on sellers' work, after shops close in protest

*Industry & policy · New*

**Published:** 20 Nov 2026, 23:50 CET

Etsy told The New York Times on Friday that it would revise its new Terms of Use, which take effect on **16 December** and add a right for Etsy and its 'third party partners and vendors' to use sellers' content to 'develop, train, test and improve artificial intelligence and machine learning technologies'. The Verge reported the planned revision at 23:50 Paris time on Friday, after the previous afternoon edition had closed.

Several long-time sellers had closed their shops over the clause, the Times reported, among them an illustrator who had sold on the site for nearly a decade and a home goods and stationery brand with 13 years there. Etsy's vice-president for customer operations, James Ossman, said the company would **share the revised terms directly with sellers soon** and that their creative work belongs to them.

Earlier in the week, in a post on Etsy's community site, Ossman wrote that Etsy does not use seller content 'to train AI models designed to copy your original work or replace your creativity'. He listed its current uses as fraud detection, search and recommendations, and seller tools, and said vendors with access include fraud-detection services and advertising partners. The revised wording has **not yet been published**.

**Analysis — why it matters:** *Editorial analysis: Etsy is the latest platform to find that **broad AI-training clauses can cost it the creators** whose work it sells.*

**Caveat:** Etsy's promise to revise the terms was made in a statement emailed to The New York Times, read here in the Philadelphia Inquirer's syndicated copy because the Times site is paywalled. Etsy's Terms of Use page answered HTTP 403 and was not read; the clause wording comes from the Times report.

**Sources:**

1. [Etsy Community: Our recent Terms of Use update](<https://community.etsy.com/forum/announcements-290/topic/our-recent-terms-of-use-update-192097>) — primary source. Checked: 21 Nov 2026, 16:06 CET
2. [The Verge: Etsy says it will revise its new AI policy after backlash from sellers](<https://www.theverge.com/ai-artificial-intelligence/1039304/etsy-says-it-will-revise-its-new-ai-policy-after-backlash-from-sellers>) — reporting. Checked: 21 Nov 2026, 16:06 CET
3. [The Philadelphia Inquirer (New York Times): Many Etsy sellers close up shop over site's new AI policy](<https://www.inquirer.com/business/etsy-artists-vendors-sellers-ai-policy-train-protest-20261121.html>) — reporting. Checked: 21 Nov 2026, 16:06 CET
4. [Engadget: Etsy says it will not use sellers' content to train AI after they revolt over policy changes](<https://www.engadget.com/2324090/etsy-not-use-seller-content-train-ai>) — reporting. Checked: 21 Nov 2026, 16:06 CET

## Key patterns (editorial analysis)

- Open models are shrinking to laptop size: **Inkling 2 Mini fits in about 20GB**.
- Rules on military AI move by consensus and slowly: a **two-year mandate**, binding or not.
- Creators are pushing back on **AI-training clauses**, and platforms are revising them.

## Source coverage

- Engine version: 3.31.0
- Engine ran this edition: yes
- Engine look-back: 2 days

### Source status

- reddit: ok, partial (21 threads; 22 requests blocked with HTTP 403; Arctic Shift archive supplied posts, some of its lookups failed with HTTP 422)
- hackernews: ok (28 stories)
- github: ok (11 items)
- devto: ok (12 articles; tags ai and llm)
- youtube: not searched (yt-dlp not available on this machine)
- polymarket: not used: blocked in France (ANJ)
- x: not searched (no consent-free source configured)

### Notes

- The installed last30days engine finished (exit 0) with 72 evidence items from Reddit, Hacker News, dev.to and GitHub. Its top clusters were a coding agent for DOS, Chinese labs, Friday's Wall Street AI sell-off and the AI-designed Frostbite CPU; the Inkling comments quoted here came from the Hacker News search API. Stories were found with 16 Google News RSS queries, publisher feeds, post-engine web supplements and the source pages. Item counts are not counts of verified developments.
- Window widened: it starts at 21:00 on Friday, about when Thinking Machines released Inkling 2 Mini, instead of at 06:07 this morning, to carry two stories the morning edition missed (Inkling 2 Mini and Etsy's planned revision). Nothing the morning edition carried is repeated.
- Polymarket not used: blocked in France (ANJ). X not searched. YouTube not searched (not available on this machine). Reddit returned results through the Arctic Shift archive, but 22 direct requests were blocked (HTTP 403) and some archive lookups failed (HTTP 422), so Reddit coverage was partial. VentureBeat's feed answered HTTP 429 and Google DeepMind's feed could not be parsed. Missing coverage does not mean nobody discussed these stories.
- Paywalled or not read: The New York Times (paywalled; its Etsy report was read as syndicated by The Philadelphia Inquirer), Reuters' own pages (Bessent's remarks were read in Defense News' copy of the Reuters report), the Associated Press site, which answered HTTP 403 and is not cited, and Etsy's Terms of Use page, which answered HTTP 403. No published text of the Geneva mandate was found.
- Newsletter leads from the Iris mail bot: today's file has five leads. Inkling 2 Mini running locally on Ollama is carried here. Anthropic's first two trading days and Gemini's free task agent ran in earlier editions; the Product Hunt and Google Cloud hackathon was not carried.
- Not carried: OpenAI's report that its agents finish 46% of two-to-four-hour research tasks (published 18 November, outside the 48-hour limit), OpenAI's GPT-Live-1.1 voice model in the API (19 November), Nvidia's halt of licensed Hopper shipments to China (said on its earnings call earlier this week), ByteDance's Axion 1.0 paper (an arXiv preprint first posted on 2 November), South Korean President Lee Jae Myung's visit to the SK and AWS data centre site in Ulsan, and Fortune's report on large school districts pushing back on Google's AI Overviews.
- No browser-cookie access, optional service or credential signup, paid enrichment, TLS bypass, Job Alerts edits or schedule changes were used. Research logs and full provenance remain private.

### Engine footer (verbatim)

```text
---
✅ All agents reported back!
├─ 🟠 Reddit: 21 threads │ 12,461 upvotes │ 1,255 comments
├─ 🟡 HN: 28 stories │ 2,393 points │ 1,788 comments
├─ 👩‍💻 dev.to: 12 articles │ 127 reactions │ 37 comments
├─ 🐙 GitHub: 11 items │ 49 reactions │ 106 comments
├─ 🗣️ Top voices: r/technology, r/singularity, r/OpenAI
---
```
