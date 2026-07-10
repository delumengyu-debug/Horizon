---
layout: default
title: "Horizon Summary: 2026-07-10 (EN)"
date: 2026-07-10
lang: en
---

> From 38 items, 10 important content pieces were selected

---

1. [EU Parliament greenlights Chat Control 1.0](#item-1) ⭐️ 9.0/10
2. [OpenAI Releases GPT-5.6 with Sol, Terra, Luna Models](#item-2) ⭐️ 9.0/10
3. [Interview: Mitchell Hashimoto on Ghostty and Zig](#item-3) ⭐️ 8.0/10
4. [Why US ambulance rides are so expensive](#item-4) ⭐️ 8.0/10
5. [Meta Releases Muse Spark 1.1 with Open Weights](#item-5) ⭐️ 8.0/10
6. [Meta Superintelligence: 1 Year Progress Update](#item-6) ⭐️ 8.0/10
7. [IMGNet: Face Verification Using Sign Pattern Matching](#item-7) ⭐️ 8.0/10
8. [Meta to Mass-Produce Custom AI Chip 'Iris' in September](#item-8) ⭐️ 8.0/10
9. [China's Long March 10B Achieves World's First Net-Based Recovery at Sea](#item-9) ⭐️ 8.0/10
10. [Tencent in talks to buy AI startup Manus from Meta](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [EU Parliament greenlights Chat Control 1.0](https://www.patrick-breyer.de/en/eu-parliament-greenlights-chat-control-1-0-breyer-our-children-lose-out/) ⭐️ 9.0/10

The EU Parliament approved a regulation allowing mass scanning of private messages without suspicion until 2028, despite a majority of voting MEPs opposing it (314 against, 276 in favor). This decision undermines end-to-end encryption and sets a dangerous precedent for mass surveillance, affecting millions of users on platforms like Instagram, Discord, Gmail, and iCloud. The vote used a procedural rule requiring an absolute majority of all MEPs (361 votes) to reject the measure; the motion to reject received only 314 votes, so the regulation passed despite majority opposition among those present.

hackernews · rapnie · Jul 9, 11:03 · [Discussion](https://news.ycombinator.com/item?id=48843923)

**Background**: Chat Control 1.0 is a temporary EU regulation first introduced in 2021 to combat child sexual abuse material (CSAM) by requiring platforms to scan private messages using client-side scanning technology. Critics argue it effectively mandates mass surveillance and breaks end-to-end encryption, violating fundamental privacy rights. The regulation had previously been rejected twice but was revived and fast-tracked for a decisive vote.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control_1.0">Chat Control 1.0</a></li>
<li><a href="https://fightchatcontrol.eu/chat-control-overview">Chat Control 1 . 0 vs 2.0 - Fight Chat Control</a></li>
<li><a href="https://www.patrick-breyer.de/en/posts/chat-control/">Chat Control : The EU’s CSAM scanner proposal – Patrick Breyer</a></li>

</ul>
</details>

**Discussion**: Commenters express outrage at the procedural manipulation and democratic deficit, calling it a 'nice piece of democracy' where a law passed despite majority opposition. Many fear this breaks foundational privacy principles and undermines trust in EU institutions.

**Tags**: `#privacy`, `#surveillance`, `#encryption`, `#EU regulation`

---

<a id="item-2"></a>
## [OpenAI Releases GPT-5.6 with Sol, Terra, Luna Models](https://openai.com/index/gpt-5-6/) ⭐️ 9.0/10

OpenAI has released GPT-5.6, a new family of frontier models including Sol (flagship), Terra (balanced), and Luna (fast/cost-efficient), along with ChatGPT Work and Codex updates. The Sol model achieves a new state-of-the-art score of 7.8% on the ARC-AGI-3 benchmark, demonstrating improved reasoning and intent understanding. This release signifies a major leap in AI capabilities, particularly in complex reasoning and adaptability to novel tasks, as evidenced by the ARC-AGI-3 performance. The three-tier model family (Sol, Terra, Luna) offers scalable options for different use cases, potentially accelerating AI adoption in enterprise and research settings. GPT-5.6 Sol sets a new SOTA on ARC-AGI-3 with 7.8%, outperforming all prior verified frontier models. The models feature improved intent understanding and original image detail preservation, with Luna being the most cost-efficient option. Additionally, GPT-5.4 will be deprecated on July 23.

hackernews · logickkk1 · Jul 9, 17:04 · [Discussion](https://news.ycombinator.com/item?id=48849066)

**Background**: ARC-AGI-3 is a benchmark designed to measure progress toward artificial general intelligence (AGI) by testing an AI's ability to explore novel environments, acquire goals, and build adaptable world models. GPT-5.6 is a successor to GPT-5.4, and includes three variants: Sol (flagship), Terra (balanced), and Luna (fast/cost-efficient), each tailored to different performance and cost requirements.

<details><summary>References</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi/3">ARC - AGI - 3</a></li>
<li><a href="https://deploymentsafety.openai.com/gpt-5-6">GPT-5.6 System Card - OpenAI Deployment Safety Hub</a></li>

</ul>
</details>

**Discussion**: The community is broadly impressed, with users noting improved autonomy and coding capabilities, e.g., scanning entire codebases and optimizing. Some debate persists about GPT-5.6 vs. Claude Code, but early tests suggest strong performance. A notable observation is that GPT-5.6 Sol is the first frontier model to beat an ARC-AGI-3 game, marking a significant milestone.

**Tags**: `#AI`, `#GPT-5.6`, `#OpenAI`, `#Large Language Models`, `#ARC-AGI`

---

<a id="item-3"></a>
## [Interview: Mitchell Hashimoto on Ghostty and Zig](https://alexalejandre.com/programming/interview-with-mitchell-hashimoto/) ⭐️ 8.0/10

Mitchell Hashimoto explains his choice of the Zig programming language for building Ghostty, a fast, cross-platform terminal emulator, and discusses his pragmatic design decisions. This interview sparks substantive community debate about language culture, particularly between Rust and Zig, and influences how developers think about tool choice and design philosophy in system software. Ghostty uses platform-native UI and GPU acceleration to deliver a fast terminal experience, and Mitchell's decision to use Zig stems from his preference for a minimalist language that avoids certain aspects of Rust culture.

hackernews · veqq · Jul 9, 17:17 · [Discussion](https://news.ycombinator.com/item?id=48849292)

**Background**: Ghostty is a relatively new terminal emulator that emphasizes performance and platform-native rendering, while Zig is a systems programming language designed as an improvement over C with manual memory management and compile-time metaprogramming. Mitchell Hashimoto is a well-known engineer, co-founder of HashiCorp, and his opinions carry weight in the developer community.

<details><summary>References</summary>
<ul>
<li><a href="https://ghostty.org/">Ghostty</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://github.com/ghostty-org/ghostty">GitHub - ghostty-org/ghostty: 👻 Ghostty is a fast, feature-rich, and cross-platform terminal emulator that uses platform-native UI and GPU acceleration.</a></li>

</ul>
</details>

**Discussion**: The community comments show mixed opinions: some praise Mitchell's pragmatic approach, while others disagree with his view on CLI output defaults or criticize the Rust vs. Zig cultural debate. One commenter notes that Zig's missing features were a blocker for their project, and another references Andrew Kelley's thoughts on the Bun Rust rewrite.

**Tags**: `#Ghostty`, `#Zig`, `#terminal emulator`, `#software engineering`, `#programming languages`

---

<a id="item-4"></a>
## [Why US ambulance rides are so expensive](https://davidoks.blog/p/why-american-ambulance-rides-are) ⭐️ 8.0/10

An analysis challenges the common greed narrative for high ambulance costs, pointing instead to systemic issues like low Medicare and insurance reimbursements, and the role of private equity firms. This shifts public understanding from blaming ambulance operators to recognizing broader healthcare system failures, potentially informing policy debates on medical debt and insurance reform. The article uses an options analogy to explain pricing and notes that ambulance providers often operate on thin margins, while private equity involvement exacerbates cost shifting to patients.

hackernews · jyunwai · Jul 9, 22:15 · [Discussion](https://news.ycombinator.com/item?id=48853091)

**Background**: Ambulance services in the US are often private or fire-based, with reimbursements from Medicare and insurance capped below costs, leading to high out-of-network charges. Private equity firms have acquired many providers, increasing billing complexity and pressure on margins.

**Discussion**: Commenters shared experiences of ambulance costs in Switzerland ($1500 for a short ride) and Quebec ($500 CAD), criticizing the article's defense of private equity. Some noted patients can refuse transport, adding nuance to cost debates.

**Tags**: `#healthcare`, `#economics`, `#private equity`, `#policy`

---

<a id="item-5"></a>
## [Meta Releases Muse Spark 1.1 with Open Weights](https://ai.meta.com/blog/introducing-muse-spark-meta-model-api/) ⭐️ 8.0/10

Meta announced Muse Spark 1.1, an agentic AI model with open weights, on July 9, 2026. The model supports tool use, visual chain of thought, and multi-agent orchestration. Muse Spark 1.1 marks a significant step in Meta's agentic AI strategy, offering competitive performance at lower pricing compared to rivals. Its open weights release could commoditize coding models and intensify competition in the AI industry. The model is priced at $1.25 per million input tokens and $4.5 per million output tokens, with cached input at $0.15. The evaluation report has been criticized for using non-standard resource caps that may invalidate benchmark results.

hackernews · ot · Jul 9, 14:10 · [Discussion](https://news.ycombinator.com/item?id=48846184)

**Background**: Agentic AI refers to systems that can autonomously pursue goals and use tools, moving beyond simple text generation. Open weights models allow anyone to download and modify the model, democratizing access to advanced AI. Meta's Muse Spark series is their first line of agentic models.

<details><summary>References</summary>
<ul>
<li><a href="https://ai.meta.com/blog/introducing-muse-spark-msl/">Introducing Muse Spark: Scaling Towards Personal Superintelligence</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent - Wikipedia</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>

</ul>
</details>

**Discussion**: Community comments show mixed reactions: some users praised the model's capabilities and pricing, while others questioned the benchmark methodology. A commenter noted that the evaluation used higher resource caps than official tasks, potentially disqualifying results. There was also discussion about Meta's strategy to commoditize AI through open weights.

**Tags**: `#meta`, `#ai`, `#agentic`, `#open-source`, `#benchmark`

---

<a id="item-6"></a>
## [Meta Superintelligence: 1 Year Progress Update](https://newsletter.semianalysis.com/p/the-future-of-meta-superintelligence) ⭐️ 8.0/10

Meta has made significant progress in its superintelligence efforts, including the creation of a top-tier reinforcement learning environment startup, the most aggressive compute ramp ever seen, and a 2000km scale-across AI infrastructure. This update signals Meta's accelerated push toward superintelligence, which could reshape the AI landscape and intensify competition with other tech giants like Google DeepMind. The compute ramp is described as the most aggressive ever seen, and the scale-across architecture spans over 2000km, enabling unprecedented coordination across data centers. The RL environment startup likely leverages data from employee screen and keyboard tracking.

rss · Semianalysis · Jul 9, 19:16

**Background**: Scale-across is a paradigm shift in AI infrastructure that breaks physical data center boundaries through optical fiber, transceivers, and switches, enabling large-scale distributed training. Reinforcement learning environments are simulated worlds where AI agents learn through trial and error, and high-quality environments are critical for advancing AI capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/the-future-of-meta-superintelligence">The Future of Meta Superintelligence: A 1 Year Progress Update</a></li>
<li><a href="https://www.naddod.com/blog/a-complete-guide-to-scale-across-the-third-pillar-of-ai-computing">What Is Scale-Across? A Complete Guide to the “Third Pillar ...</a></li>
<li><a href="https://colab.research.google.com/github/metadriverse/metaurban/blob/main/documentation/source/rl_environments.ipynb">rl_environments.ipynb - Colab</a></li>

</ul>
</details>

**Tags**: `#Meta`, `#superintelligence`, `#AI infrastructure`, `#compute`, `#reinforcement learning`

---

<a id="item-7"></a>
## [IMGNet: Face Verification Using Sign Pattern Matching](https://www.reddit.com/r/MachineLearning/comments/1urxvxh/i_built_imgnet_a_face_verification_model_that/) ⭐️ 8.0/10

A face verification model called IMGNet replaces cosine similarity with sliding window sign pattern matching, achieving 96.27% on LFW with a 10.58 MB model trained on CASIA-WebFace. When applied to ArcFace embeddings without retraining, IMG Sign Score achieves 99.58% on LFW. This demonstrates that sign pattern matching is a viable alternative to cosine similarity for face verification, potentially enabling more efficient and robust models. It also suggests that well-trained face embeddings intrinsically encode sign pattern consistency, decoupling the similarity metric from the training objective. The model uses a novel SW Block that computes pixel-wise differences at prime window sizes {3,5,7}, and the IMG Sign MSE Loss focuses purely on sign pattern agreement. Three metrics (IMG Sign, AMP IMG, Chain) share a single threshold, and a voting system decides match, uncertain, or different.

reddit · r/MachineLearning · /u/img-_- · Jul 9, 18:00

**Background**: Traditional face verification compares embedding vectors using cosine similarity, which measures global angular direction. The sliding window pattern is a technique for keeping track of a subset of continuous data in an array. IMGNet applies a sliding window over embedding dimensions and compares sign patterns locally, capturing relational structure independent of absolute values.

<details><summary>References</summary>
<ul>
<li><a href="https://dev.to/bradbieselin/the-sliding-window-pattern-3nei">The sliding window pattern - DEV Community</a></li>

</ul>
</details>

**Tags**: `#face verification`, `#machine learning`, `#embeddings`, `#deep learning`, `#sign pattern matching`

---

<a id="item-8"></a>
## [Meta to Mass-Produce Custom AI Chip 'Iris' in September](https://www.reuters.com/world/asia-pacific/meta-put-ai-chip-into-production-september-it-looks-double-computing-capacity-2026-07-09/) ⭐️ 8.0/10

Meta plans to begin mass production of its custom AI chip, code-named Iris, in September 2026, as part of its MTIA program. The company also aims to double its computing capacity from 7 gigawatts in 2026 to 14 gigawatts by 2027. This move reduces Meta's reliance on external suppliers like Nvidia and AMD, potentially lowering costs and improving performance for its AI workloads. It signals a major shift in the AI hardware landscape, as major tech companies increasingly invest in custom silicon. The Iris chip is part of the fourth generation of Meta's Training and Inference Accelerator (MTIA) program, designed with help from Broadcom and manufactured by TSMC. Testing was completed in just six weeks with no major issues found.

telegram · zaihuapd · Jul 9, 12:37

**Background**: Meta has been developing custom AI chips under the MTIA (Meta Training and Inference Accelerator) family since at least 2023, aiming to optimize hardware for its specific AI workloads like recommendation models and generative AI. Previously, Meta relied heavily on GPUs from Nvidia. Custom chips allow Meta to tailor performance and power efficiency, and reduce dependency on third-party suppliers amid high demand and supply constraints.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reuters.com/world/asia-pacific/meta-put-ai-chip-into-production-september-it-looks-double-computing-capacity-2026-07-09/">EXCLUSIVE: Meta to put AI chip into production in September ...</a></li>
<li><a href="https://ai.meta.com/blog/meta-mtia-scale-ai-chips-for-billions/">Four MTIA Chips in Two Years: Scaling AI Experiences for Billions</a></li>
<li><a href="https://about.fb.com/news/2026/03/expanding-metas-custom-silicon-to-power-our-ai-workloads/">Expanding Meta’s Custom Silicon to Power Our AI Workloads</a></li>

</ul>
</details>

**Tags**: `#AI chips`, `#Meta`, `#hardware`, `#custom silicon`, `#AI infrastructure`

---

<a id="item-9"></a>
## [China's Long March 10B Achieves World's First Net-Based Recovery at Sea](https://weibo.com/7340734455/R814of1Ki) ⭐️ 8.0/10

On July 10, 2026, China's Long March 10B rocket launched from Hainan Commercial Space Launch Site and successfully recovered its first stage at sea using a net-based recovery system, marking the world's first net-based rocket recovery. This achievement represents a major breakthrough in reusable rocket technology, potentially reducing launch costs and increasing launch frequency, putting China at the forefront of innovative recovery methods. The net-based recovery system consists of a hook device on the rocket and a net on a maritime platform, which together captured the first stage about 6 minutes after stage separation. The platform has DP2 dynamic positioning with accuracy within 1 meter.

telegram · zaihuapd · Jul 10, 04:36

**Background**: Reusable rocket technology aims to recover and reuse the most expensive parts of a rocket, typically the first stage. Traditional methods involve landing on a drone ship or ground pad, as done by SpaceX. China's net-based recovery is a novel approach that uses a large net on a platform to catch the descending rocket stage, potentially simplifying landing gear requirements.

<details><summary>References</summary>
<ul>
<li><a href="https://www.news.cn/20260710/ba0ac14f31dd492aaf918e7a86ac844a/c.html">长 征 十 号 乙 首飞成功 我国 运 载 火 箭 首次实现可控回收-新华网</a></li>
<li><a href="https://www.guancha.cn/politics/2026_07_10_823266.shtml">长 征 十 号 乙 运 载 火 箭 成功实现一子级可控回收</a></li>

</ul>
</details>

**Tags**: `#aerospace`, `#reusable rockets`, `#China`, `#space technology`, `#rocket recovery`

---

<a id="item-10"></a>
## [Tencent in talks to buy AI startup Manus from Meta](https://www.reuters.com/technology/tencent-talks-become-ai-start-up-manus-largest-shareholder-ft-reports-2026-07-10/) ⭐️ 8.0/10

Tencent is negotiating to acquire the AI startup Manus from Meta, aiming to become its largest shareholder through a buyback deal valued at least $2 billion. This deal reflects shifting dynamics in the AI industry, with Chinese tech giants like Tencent strengthening their AI capabilities amid regulatory pressures on foreign ownership. The deal involves Tencent, early investors ZhenFund and HSG, and follows Meta's earlier $2 billion acquisition of Manus, which was ordered by Chinese authorities to be unwound.

telegram · zaihuapd · Jul 10, 06:45

**Background**: Manus is an autonomous AI agent startup founded by Butterfly Effect, based in Singapore and originally from China. Meta had acquired Manus in late 2025 for around $2 billion, but Chinese regulators required Meta to divest the company due to national security concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Manus_(AI_agent)">Manus ( AI agent) - Wikipedia</a></li>
<li><a href="https://www.linkedin.com/posts/mighty-glory-corporate-solutions_what-is-manus-the-singapore-based-ai-startup-activity-7411919062869401601-8YSS">Meta Acquires Manus , Singapore AI Startup , for Specialized... | LinkedIn</a></li>

</ul>
</details>

**Tags**: `#AI`, `#acquisition`, `#Tencent`, `#Meta`, `#Manus`

---