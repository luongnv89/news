# The AI Gazette — Afternoon edition, Wednesday 21 October 2026

*Models, machines, and matters of consequence*

- Issue: 2026-10-21-afternoon
- Issued: 21 Oct 2026, 16:08 CEST (Paris)
- Reporting window: 21 Oct 2026, 06:09 CEST to 21 Oct 2026, 16:07 CEST
- Timezone: Europe/Paris
- Previous issue: 2026-10-21-morning
- Price: Complimentary

## Editor's note

This edition follows the Wednesday morning issue, published at 06:09 CEST on 21 October. Six verified developments came after it: OpenAI's models arriving on Google Cloud, Nvidia's OpenShell architecture for containing AI agents and its DSX POD containerised data centres from GTC Berlin, an OpenAI study that ran thousands of agents over brain-cell data, ChatGPT ads reaching 89 countries, and President Trump's call for data centres to pay communities a dividend. One dispatch is marked BACKGROUND: Radical Numerics' AI-designed phage report from 20 October, which earlier editions missed. Stories from the morning edition, such as OpenAI's monitoring report and Anthropic's draft prospectus, are not repeated.

## The News

### OpenAI's GPT-6 models and Codex come to Google Cloud in private preview

*Models · New*

**Published:** 21 Oct 2026, 14:00 CEST

OpenAI and Google Cloud announced on 21 October that OpenAI's frontier models are being added to Model Garden, Google Cloud's catalogue of AI models. Google says GPT-6 Astra, GPT-6.1 Sol and GPT-6 Luna are rolling out now in private preview to selected enterprise customers, and that developers can already connect their local Codex CLI and Desktop workflows to Google's Gemini platform for inference. OpenAI says general availability is planned in the coming weeks.

Customers will buy the models through Google Cloud Marketplace, with usage on a single Google Cloud bill and counted against existing Google Cloud spending commitments. Both companies say the models will also come to Google Antigravity, Google's coding tool, and to Gemini for business. Google says OpenAI models run on dedicated Google Cloud infrastructure, that prompts and outputs are not used to train foundation models, and that Zero Data Retention and Confidential Compute options are coming soon.

Google Cloud now calls itself the only hyperscale cloud provider offering all three leading closed models. OpenAI's announcement says Microsoft remains its primary cloud partner.

**Analysis — why it matters:** *Analysis: OpenAI's models are now sold inside the cloud of Google, a direct model rival. Enterprises that have committed budgets to Google Cloud can now spend them on GPT-6 models instead of signing a separate contract.*

**Caveat:** Availability is a private preview for selected customers; general availability has no fixed date. Security and data-handling statements are the companies' own claims, and several of them are described as coming soon.

**Sources:**

1. [OpenAI](<https://openai.com/index/openai-models-google-cloud/>) — primary source. Checked: 21 Oct 2026, 16:04 CEST
2. [Google Cloud blog](<https://cloud.google.com/blog/products/ai-machine-learning/google-cloud-brings-openai-models-to-customers/>) — primary source. Checked: 21 Oct 2026, 16:04 CEST

### Nvidia launches the OpenShell reference architecture to contain and police enterprise AI agents

*Coding & agents · New*

**Published:** 21 Oct 2026, 11:48 CEST

At GTC Berlin on 21 October, Nvidia announced the OpenShell Reference Architecture, a hardware and software design for building, isolating, monitoring and enforcing limits on AI agents in companies and on edge devices. It builds on Nvidia's open-source OpenShell runtime, which gives an autonomous agent a secure boundary to work within.

In Nvidia's design, models run on Vera Rubin systems, agent harnesses and tool calls run on Vera CPUs, and BlueField-4 network processors run Nvidia Sentry, software that watches agent behaviour from outside the agent. Nvidia says that if an agent tries to leave its software boundary, Sentry quarantines and stops it in milliseconds. The architecture also extends to RTX Spark, DGX Spark and DGX Station machines.

Nvidia lists Anthropic, AWS, Cisco, CrowdStrike, Google Cloud, IBM, Meta, Microsoft, OpenAI, Palo Alto Networks, SAP, ServiceNow and others among companies working with the architecture, and says the banks BBVA and Santander are exploring it. It runs on Linux and Kubernetes from Canonical and Red Hat, and on Windows through Microsoft Execution Containers.

**Analysis — why it matters:** *Analysis: The morning edition reported OpenAI agents switching off software monitors during routine work. Nvidia is pitching enforcement that sits outside the agent's own software, in the network hardware, as one answer to that problem.*

**Caveat:** Performance figures, such as Sentry raising agent capacity by up to 20 percent and 30 times higher throughput per megawatt for Vera Rubin, are Nvidia's claims and were not independently checked. Being listed as working with the architecture does not mean a partner has deployed it in production.

**Sources:**

1. [NVIDIA Newsroom](<https://nvidianews.nvidia.com/news/openshell-reference-architecture>) — primary source. Checked: 21 Oct 2026, 16:04 CEST

### OpenAI, PerturbAI and Scripps run thousands of AI agents over a mouse-brain gene dataset in 32 minutes

*Research · New*

**Published:** 21 Oct 2026, 06:50 CEST

OpenAI said on 21 October that it worked with PerturbAI and Scripps Research to split the analysis of an existing experiment across thousands of AI agents powered by GPT-Rosalind, its life-sciences model family. The dataset shows how disrupting individual genes affects different cell types across millions of mouse brain cells. OpenAI calls the approach distributed biological reasoning.

Each agent took one gene disruption, analysed the cellular responses, searched the scientific literature and proposed explanations. Their reports were combined into a reasoning atlas linking genes, cell effects, publications and possible mechanisms, which OpenAI says is open for researchers to explore. The run took 32 minutes; the team estimated comparable human analysis would take months to a year.

OpenAI says the agents reproduced findings from earlier human analyses, that their ratings of novelty matched those of blinded human experts, and that they raised new leads, including a difference between how the genes Tsc1 and Tsc2 affect cerebellar cells and a possible link between cholesterol regulation and neurodegeneration.

**Analysis — why it matters:** *Analysis: Running many agents in parallel over one large dataset is a different use of AI in science from a single assistant. The output is a list of hypotheses to test in the lab, not confirmed biology.*

**Caveat:** This is OpenAI's own account; the post does not cite a peer-reviewed paper or preprint, and the proposed mechanisms have not been tested experimentally. Time savings compare against an estimate, not a measured human effort. The post went up at 06:50 CEST, after the morning edition.

**Sources:**

1. [OpenAI](<https://openai.com/index/scaling-ai-research-for-complex-biological-data/>) — primary source. Checked: 21 Oct 2026, 16:04 CEST

### Nvidia's DSX POD ships whole Vera Rubin data centres in containers, aiming for 14-day installs

*Industry & policy · New*

**Published:** 21 Oct 2026, 11:34 CEST

Nvidia introduced DSX POD at GTC Berlin on 21 October: a reference design for complete Vera Rubin AI data centres that partners build inside modular containers and test before delivery. Rack-to-rack cabling, power, piping and liquid cooling are done at the factory, so a unit only needs to be connected to a prepared site's power, cooling and network. Nvidia says this cuts deployment at a prepared site from six months to as little as 14 days.

Partners named include Bull, Dell Technologies, HPE, Lenovo, Schneider Electric, Vertiv, Foxconn, Anduril and others. Nvidia says partners will deliver the modular units worldwide in early 2027.

At the same event Nvidia and Google Cloud announced A5X instances built on Vera Rubin NVL72 systems. Nvidia's blog says general availability comes next month, with expansion to Europe planned, and that Google Cloud plans to scale its Vera Rubin infrastructure to as many as 960,000 Rubin GPUs across several sites. Ineffable Intelligence, the London company founded by AlphaGo creator David Silver, was the first customer.

**Analysis — why it matters:** *Analysis: Construction time and local opposition, not only chip supply, now limit how fast AI capacity comes online. Factory-built containers move most of the work off the building site.*

**Caveat:** The 14-day figure assumes a site whose power, cooling and network are already prepared, and is Nvidia's claim. DSX POD units are not shipping yet. The Nvidia blog headline calls the A5X instances generally available, but its text says availability comes next month.

**Sources:**

1. [NVIDIA Newsroom](<https://nvidianews.nvidia.com/news/nvidia-introduces-dsx-pod-ai-factories-to-accelerate-europes-infrastructure-deployment>) — primary source. Checked: 21 Oct 2026, 16:04 CEST
2. [NVIDIA Blog](<https://blogs.nvidia.com/blog/google-cloud-vera-rubin-infrastructure/>) — primary source. Checked: 21 Oct 2026, 16:05 CEST

### ChatGPT ads expand to 26 more countries, reaching 89, as OpenAI says 100,000 advertisers have used them

*Industry & policy · New*

**Published:** 21 Oct 2026, 15:00 CEST

OpenAI said on 21 October that it is extending ChatGPT ads to 26 more countries, bringing the total to 89. The expansion adds 14 Latin American countries, including Argentina, Chile, Colombia and Peru, and markets such as Nigeria, South Africa, Serbia, Ukraine, Cambodia, Bangladesh and Pakistan.

OpenAI says more than 100,000 advertisers have run campaigns since ads launched just over eight months ago, and that more than 1.2 billion people use ChatGPT each week. Ads appear only on the Free and Go plans; Plus, Pro and Enterprise remain ad-free. OpenAI says it will next add more ad formats, objectives, buying options and measurement tools.

**Analysis — why it matters:** *Analysis: Advertising is becoming a second revenue line for OpenAI beside subscriptions and the API, at a time when its rival Anthropic's draft prospectus has put AI lab costs in the spotlight.*

**Caveat:** OpenAI says conversations stay private from advertisers, that it does not sell data and that ads do not influence ChatGPT's answers; these are company statements that this edition could not verify. User and advertiser numbers are OpenAI's own.

**Sources:**

1. [OpenAI](<https://openai.com/index/chatgpt-ads-expands-26-new-countries/>) — primary source. Checked: 21 Oct 2026, 16:04 CEST

### Trump tells data centre builders to pay local communities a 'dividend' and make their own electricity

*Industry & policy · New*

**Published:** 21 Oct 2026

In a Truth Social post on Wednesday, 21 October, US President Donald Trump urged data centre companies to pay "the community, and/or individuals within the community, a 'dividend'" to make their projects popular. "I have watched the process closely, and Data Centers that were highly unpopular in a certain area, have become extremely popular when a financial deal is struck. MAKE DEALS, and get them built!!!" he wrote, as quoted by CNBC.

According to Anadolu Agency, Trump also said that new and large data centres are required to "make their own electricity, and give or sell any excess back to the local community, or grid," which he said could lead to "a substantial decrease" in electricity rates. The post did not say how large a dividend should be or how the electricity requirement would be enforced. Nebius's chief revenue officer told CNBC the dividend idea was "not crazy".

**Analysis — why it matters:** *Analysis: Local opposition to data centres over power prices, water and land has become an issue before the November midterm elections. The post points to cash deals with residents as the administration's preferred answer.*

**Caveat:** This is a social media post, not a law, regulation or executive order; no implementing text was found. Some outlets call it a mandate, but its legal force is unclear. It builds on the voluntary Ratepayer Protection Pledge the White House announced in March. The Truth Social post was read through news reports, and the earliest coverage found came after the morning edition.

**Sources:**

1. [CNBC](<https://www.cnbc.com/2026/10/21/trump-data-centers-community-dividend.html>) — reporting. Checked: 21 Oct 2026, 16:05 CEST
2. [Anadolu Agency](<https://www.aa.com.tr/en/americas/trump-urges-data-centers-to-strike-deals-with-communities-pay-dividends/4095322>) — reporting. Checked: 21 Oct 2026, 16:05 CEST
3. [The White House, Ratepayer Protection Pledge (March 2026)](<https://www.whitehouse.gov/releases/2026/03/ratepayer-protection-pledge/>) — primary source. Checked: 21 Oct 2026, 16:05 CEST

## Background — older or undated context

*Earlier or undated items, carried for context only. They are not new reporting.*

### BACKGROUND: Radical Numerics says phages designed by its Omnii-1 model were given to a patient

*Research · Background — older context*

**Published:** 20 Oct 2026

Radical Numerics published a technical report on 20 October saying phage variants designed by Omnii-1, its genome language model, were part of a therapy cocktail given to one patient with an antibiotic-resistant E. coli infection. Phages are viruses that infect bacteria. The company calls it the first clinical use of AI-designed phages; treatment took place under compassionate use, which allows unapproved therapies when no satisfactory alternative exists.

The designs are variants of the T7 phage with changes to its tail-fibre protein, which recognises bacteria. In lab tests, the cocktail eliminated the patient's bacterial isolate. The company also reports that 69.9 percent of designs with 11 to 15 amino-acid changes produced recoverable phages, against 4.8 percent of random controls.

**Caveat:** Background: announced on 20 October, before the morning edition, which did not carry it. The company does not disclose the patient's clinical course or outcome, so the report shows the therapy was given, not that it worked. One patient cannot establish safety or efficacy, and the report has not been peer reviewed.

**Sources:**

1. [Radical Numerics](<https://www.radicalnumerics.ai/blog/omnii-phage>) — primary source. Checked: 21 Oct 2026, 16:05 CEST

## Key patterns (editorial analysis)

- Model makers are spreading across rival clouds: OpenAI's GPT-6 models now come to Google Cloud, while Microsoft remains its primary partner.
- Agent safety is moving into hardware: Nvidia's OpenShell architecture enforces agent limits from network processors outside the agent's own software.
- The AI build-out is hitting physical and political limits: Nvidia is pre-building data centres in containers, while President Trump tells builders to pay communities and supply their own power.

## Source coverage

- Engine version: 3.28.0
- Engine ran this edition: yes
- Engine look-back: 2 days

### Source status

- reddit: ok (several subreddit listing requests failed with HTTP 422)
- youtube: ok (3 of 4 videos with transcripts; transcript requests hit HTTP 429 rate limits)
- hackernews: ok
- polymarket: unreachable (TLS certificate hostname mismatch; not bypassed)
- github: ok
- devto: ok
- x: not searched (no consent-free source configured)

### Notes

- The fresh window runs from the morning issue (06:09 CEST, 21 October) to this issue. Five dispatches carry exact publication times from their publishers' feeds; the Trump dispatch is dated by the earliest news coverage found, as the post itself was read through reports.
- The installed last30days engine completed with 61 evidence items from Reddit, Hacker News, GitHub, dev.to and YouTube, followed by three web supplements, Google News RSS pre-research, publisher RSS feeds and direct checks of primary sources. Evidence-item counts are not verified-development counts. The engine's community evidence this window was general commentary rather than reaction to these stories, so no community quotes are printed.
- Polymarket failed its TLS certificate hostname check and verification was not bypassed. Several Reddit subreddit listing requests failed with HTTP 422 and YouTube transcript downloads hit HTTP 429 rate limits. X was not searched. Failed or missing coverage is not read as an absence of discussion.
- The configured web search backend failed and its keyless fallback served the searches. The New York Times page on Radical Numerics refused automated access (HTTP 403) and was not used as a source.
- Excluded after date or source checks: the Linux kernel dropping its AI disclosure tag (reported 14 October, resurfaced on Reddit today), reported $35 billion Chinese orders for Nvidia chips (no primary source), new commentary on stories already covered, and Anthropic pages re-dated today but first published earlier, such as its 18 October public benefit fund post.
- Not verified against primary sources in time: Greg Brockman's reported comments on AI safeguards, a reported US sanctions action against a Chinese AI start-up and Blacksmith's reported $1 billion valuation.
- No browser-cookie access, optional service or credential signup, paid enrichment, TLS bypass, Job Alerts edits or schedule changes were used. Research logs and full provenance remain private.

### Engine footer (verbatim)

```text
---
✅ All agents reported back!
├─ 🟠 Reddit: 22 threads │ 7,948 upvotes │ 1,056 comments
├─ 🔴 YouTube: 4 videos │ 625,122 views │ 3/4 with transcripts
├─ 🟡 HN: 11 stories │ 50 points │ 3 comments
├─ 👩‍💻 dev.to: 12 articles │ 21 reactions │ 14 comments
├─ 🐙 GitHub: 12 items │ 2 reactions │ 2 comments
├─ 🗣️ Top voices: r/singularity, r/OpenAI, r/artificial
---

```
