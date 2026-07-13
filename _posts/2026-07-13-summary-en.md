---
layout: default
title: "Horizon Summary: 2026-07-13 (EN)"
date: 2026-07-13
lang: en
---

> From 91 items, 19 important content pieces were selected

---

1. [Terry Tao Explores AI Coding Agents for App Development](#item-1) ⭐️ 9.0/10
2. [GPT-5.6 Solves 50-Year Cycle Double Cover Conjecture in One Hour](#item-2) ⭐️ 9.0/10
3. [xAI Grok CLI silently uploads entire codebase and secrets by default](#item-3) ⭐️ 9.0/10
4. [Claude Code vs OpenCode: Token Overhead Comparison](#item-4) ⭐️ 8.0/10
5. [George Hotz: LLMs Powerful, But Hype Overblown](#item-5) ⭐️ 8.0/10
6. [CGI and LLMs: A Parallel on Craftsmanship](#item-6) ⭐️ 8.0/10
7. [Cloudflare Fixes Race Condition in hyper HTTP/1](#item-7) ⭐️ 8.0/10
8. [Quadriplegic Patient Regains Hand Movement Using NEO BCI](#item-8) ⭐️ 8.0/10
9. [Chromium 148 Math.tanh enables OS fingerprinting](#item-9) ⭐️ 7.0/10
10. [Ghostel.el: Fast Emacs Terminal Emulator Powered by libghostty](#item-10) ⭐️ 7.0/10
11. [Shingles Vaccine May Reduce Dementia Risk](#item-11) ⭐️ 7.0/10
12. [LLM Agents Should Never Be DRIs, Argues Simon Willison](#item-12) ⭐️ 7.0/10
13. [AI Data Centers Face Growing Opposition](#item-13) ⭐️ 7.0/10
14. [AI and Quantum Computing Generate New Peptides for Rare Diseases](#item-14) ⭐️ 7.0/10
15. [Quantum computing still far from fault tolerance, FT warns](#item-15) ⭐️ 7.0/10
16. [EU to fine big tech for consumer protection failures](#item-16) ⭐️ 7.0/10
17. [Hacker News Recap for 2026-07-13 Features Top Tech Stories](#item-17) ⭐️ 7.0/10
18. [Zer0Fit: MCP server for Google TabFM & TimesFM zero-shot ML](#item-18) ⭐️ 7.0/10
19. [Cursor Develops AI Agent 'Sand' to Challenge Claude Cowork](#item-19) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Terry Tao Explores AI Coding Agents for App Development](https://terrytao.wordpress.com/2026/07/11/old-and-new-apps-via-modern-coding-agents/) ⭐️ 9.0/10

Terry Tao, a renowned mathematician, published a blog post detailing his experiences using modern AI coding agents to build visualizations and apps, highlighting both their potential and limitations. As a prominent figure in mathematics, Tao's endorsement signals growing acceptance of AI tools in technical fields, encouraging broader adoption for non-critical tasks and sparking discussion on the role of LLMs in software development. Tao emphasized that while LLM-coded supplements are acceptable for non-mission-critical visualizations, they should not be fully trusted. The post included concrete examples of building interactive tools with AI assistance, such as data visualizations for research papers.

hackernews · subset · Jul 12, 11:09 · [Discussion](https://news.ycombinator.com/item?id=48880170)

**Background**: AI coding agents are systems that can autonomously plan, write, execute, and iterate code based on user goals, going beyond simple code completion to handle multi-step tasks. This post reflects a broader trend where large language models (LLMs) lower the barrier to software creation, enabling non-experts to generate functional applications quickly.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent - Wikipedia</a></li>
<li><a href="https://github.com/resources/articles/what-are-ai-agents">What are AI agents? · GitHub</a></li>

</ul>
</details>

**Discussion**: Commenters praised Tao's balanced perspective, with some noting that AI coding tools have enabled them to build visualizations they previously lacked time for. Others made humorous comparisons, likening Tao's use of coding agents to a chef discovering microwave dinners.

**Tags**: `#AI coding agents`, `#LLM applications`, `#software development`, `#Terry Tao`, `#visualization tools`

---

<a id="item-2"></a>
## [GPT-5.6 Solves 50-Year Cycle Double Cover Conjecture in One Hour](https://www.qbitai.com/2026/07/447873.html) ⭐️ 9.0/10

OpenAI's GPT-5.6 Sol Ultra model autonomously solved the cycle double cover conjecture, a 50-year-old open problem in graph theory, in under one hour by using 64 parallel sub-agents to transform the problem into a finite field edge labeling and linear equations system. This breakthrough demonstrates that large language models can independently tackle deep mathematical conjectures, potentially accelerating research in graph theory and combinatorial optimization. It also showcases the power of multi-agent architectures for complex reasoning tasks, setting a new benchmark for AI-assisted theorem proving. The model generated a complete 3-page PDF proof and OpenAI also published the full prompt (approximately 700 characters) which does not prescribe fixed steps but specifies acceptance criteria, definitions, boundary conditions, and failure cases, requiring dynamic allocation of sub-agents and independent verification.

telegram · zaihuapd · Jul 12, 03:49

**Background**: The cycle double cover conjecture, posed by W. T. Tutte, Itai and Rodeh, George Szekeres, and Paul Seymour, asks whether every bridgeless graph has a collection of cycles such that each edge appears exactly twice. Finite fields are algebraic structures used in the proof to label edges and solve linear equations. Multi-agent AI systems decompose tasks across specialized sub-agents running in parallel, as seen in frameworks like Claude Code and OpenAI Symphony.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cycle_double_cover_conjecture">Cycle double cover conjecture</a></li>
<li><a href="https://en.wikipedia.org/wiki/Finite_field">Finite field</a></li>
<li><a href="https://www.oflight.co.jp/en/glossary/multi-agent">Multi - Agent | Oflight Inc.</a></li>

</ul>
</details>

**Tags**: `#AI`, `#GPT-5.6`, `#graph theory`, `#multi-agent`, `#mathematical proof`

---

<a id="item-3"></a>
## [xAI Grok CLI silently uploads entire codebase and secrets by default](https://gist.github.com/cereblab/dc9a40bc26120f4540e4e09b75ffb547) ⭐️ 9.0/10

Security researchers discovered that xAI's Grok Build CLI (version 0.2.93) defaults to uploading the entire repository as a git bundle and all read file contents (including .env secrets) to xAI servers, even when the user disables the 'improve model' toggle. This poses a severe data exfiltration risk for developers using the tool, potentially leaking proprietary code, API keys, and credentials to external servers without consent, severely undermining trust in xAI's software. In a test with a 12 GB repository, over 5 GiB of data was successfully uploaded with no server-side rejection, and a file explicitly instructed not to be opened was still recoverable from the uploaded archive.

telegram · zaihuapd · Jul 12, 04:19

**Background**: git bundle is a command that packages Git objects (commits, trees, blobs) into a single file for offline transfer. Grok Build CLI is an official command-line tool from xAI that uses AI models to assist with coding tasks. The tool's default behavior of uploading repository contents raised immediate security concerns, though xAI has since released a server-side update that adds a disable_codebase_upload field.

<details><summary>References</summary>
<ul>
<li><a href="https://git-scm.com/docs/git-bundle">Git - git - bundle Documentation</a></li>
<li><a href="https://x.ai/cli">Grok Build | SpaceXAI</a></li>

</ul>
</details>

**Tags**: `#security`, `#privacy`, `#xAI`, `#CLI`, `#data exfiltration`

---

<a id="item-4"></a>
## [Claude Code vs OpenCode: Token Overhead Comparison](https://systima.ai/blog/claude-code-vs-opencode-token-overhead) ⭐️ 8.0/10

A systematic analysis revealed that Claude Code sends approximately 33,000 tokens before reading the user's prompt, while OpenCode sends only about 7,000 tokens under the same conditions, indicating a 4.7x difference in token waste. This token inefficiency directly impacts user costs and response speed for AI-assisted coding, and raises questions about the design priorities of different agentic coding tools. Developers and teams relying on such tools should consider token consumption as a key evaluation metric. The analysis used a logging proxy to capture all request payloads between the coding tool and Anthropic's endpoint, focusing on system prompts, tool schemas, and caching strategies. The author noted that Claude Code's sub-agent orchestration and aggressive tool calling contribute to the overhead.

hackernews · systima · Jul 12, 18:25 · [Discussion](https://news.ycombinator.com/item?id=48883275)

**Background**: Agentic coding tools like Claude Code and OpenCode are AI-powered systems that execute multi-step software development tasks in the terminal. They use a 'harness' — infrastructure that manages prompts, tools, and model interactions. Token overhead refers to tokens consumed for system instructions and context beyond the user's actual request, which can significantly inflate costs.

<details><summary>References</summary>
<ul>
<li><a href="https://systima.ai/blog/claude-code-vs-opencode-token-overhead">Claude Code Sends 4.7x More Tokens Than... | Systima Blog</a></li>
<li><a href="https://levelup.gitconnected.com/stop-your-ai-agent-from-bleeding-tokens-start-building-harnesses-b855ce210a9b">Stop Your AI Agent From Bleeding Tokens . | Level Up Coding</a></li>

</ul>
</details>

**Discussion**: Commenters pointed out that sub-agents are a major source of token waste, with one user experiencing seven sub-agents launched for a single task. Another expressed suspicion that Anthropic's business incentives lead to higher token usage. The author acknowledged criticism and promised a follow-up with more detailed task comparisons and qualitative results.

**Tags**: `#AI coding tools`, `#token efficiency`, `#Claude Code`, `#OpenCode`, `#prompt engineering`

---

<a id="item-5"></a>
## [George Hotz: LLMs Powerful, But Hype Overblown](https://geohot.github.io//blog/jekyll/update/2026/07/12/i-love-llms.html) ⭐️ 8.0/10

George Hotz published a blog post arguing that while LLMs are genuinely useful, the massive valuations of frontier AI labs are unjustified because these labs will fail to capture the value they create, as the real benefits accrue to individuals and small-scale users. This perspective challenges the prevailing narrative of AI as a winner-take-all industry and suggests that open-source, personalized AI will drive productivity gains rather than centralized frontier models, which has implications for investment, policy, and AI development strategy. Hotz emphasizes that productivity improvements from LLMs are happening privately in homelabs and small-scale deployments, not necessarily in visible new software products, and that the cost of frontier model subscriptions (e.g., $100-$200/month) is already a no-brainer for many, implying a cap on how much value can be extracted from users.

hackernews · therepanic · Jul 12, 18:31 · [Discussion](https://news.ycombinator.com/item?id=48883343)

**Background**: Value capture is an economic concept referring to how much of the value created by a product or service is retained by the producer versus passed to consumers. Frontier labs like OpenAI, Anthropic, and Google DeepMind invest billions in training large models, but if users can run open-source models locally or pay modest subscription fees, the labs may not recoup their investments. The debate over AI hype vs. reality has been ongoing, with critics arguing that despite impressive demos, widespread economic transformation has been slow.

<details><summary>References</summary>
<ul>
<li><a href="https://www.academia.edu/Documents/in/Value_capture?page=2">Value capture Research Papers - Academia.edu</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed with Hotz's value capture thesis, with some noting that frontier model subscriptions are a no-brainer at current prices (SwellJoe). Others shared personal experiences of building one-off software for specific use cases, reinforcing the idea that productivity gains are real but fragmented (TheAceOfHearts). A dissenting voice (kenforthewin) argued that recent model releases like Sonnet 4 and Opus 4.5 feel like a step change, suggesting acceleration may shift the calculus.

**Tags**: `#LLMs`, `#AI hype`, `#open source`, `#value capture`, `#productivity`

---

<a id="item-6"></a>
## [CGI and LLMs: A Parallel on Craftsmanship](https://fabiensanglard.net/extinct/index.html) ⭐️ 8.0/10

Fabien Sanglard published an article drawing a parallel between CGI's impact on practical effects in film and the potential of large language models (LLMs) to make manual coding obsolete, igniting a debate on productivity versus quality in software engineering. This comparison highlights the risk that AI-driven code generation could devalue the craftsmanship of software engineering, similar to how CGI devalued practical effects, prompting developers to reconsider the trade-offs between speed and quality. The article argues that while LLMs boost productivity, careful human review is necessary to maintain quality, and those who refuse to use LLMs may fall behind in output volume. It also notes that writing every line by hand is no longer the norm.

hackernews · zdw · Jul 12, 15:17 · [Discussion](https://news.ycombinator.com/item?id=48881830)

**Background**: Large language models (LLMs) are neural networks trained on vast text data to generate and understand human language, and they are now used in AI code generation tools like GitHub Copilot. In film, CGI (computer-generated imagery) largely replaced practical effects for decades, but there is a recent pushback towards practical effects for their superior visual quality. The article draws on this history to question whether LLMs will similarly devalue human coding skills before a quality-focused correction occurs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/large-language-models">What Are Large Language Models (LLMs)? | IBM</a></li>
<li><a href="https://cloud.google.com/use-cases/ai-code-generation">AI Code Generation: Definition, Uses and Tools | Google Cloud</a></li>

</ul>
</details>

**Discussion**: Comments highlight concerns that the analogy extends to devaluation of skilled labor, as unionized VFX houses face similar pressures. Some argue that productivity volume is not the primary evaluation metric in software engineering, and that knowing LLMs but not always using them is a balanced approach.

**Tags**: `#AI`, `#LLM`, `#software engineering`, `#future of programming`, `#CGI`

---

<a id="item-7"></a>
## [Cloudflare Fixes Race Condition in hyper HTTP/1](https://www.infoq.com/news/2026/07/cloudflare-hyper-bug-fix/?utm_campaign=infoq_content&utm_source=infoq&utm_medium=feed&utm_term=global) ⭐️ 8.0/10

Cloudflare identified and fixed a race condition in hyper's HTTP/1 implementation that could silently truncate large HTTP responses while returning a 200 OK status. The bug had existed for years and was triggered only under specific timing conditions. This bug is significant because hyper is a widely used Rust HTTP library serving as a building block for many applications and services. The silent truncation could lead to data loss or unexpected behavior in systems relying on complete responses. The race condition was in hyper's HTTP/1 server and client code, affecting large responses. Cloudflare fixed it upstream, and the patch has been merged.

rss · InfoQ · Jul 12, 06:18

**Background**: hyper is a fast and correct HTTP implementation written in Rust, designed as a low-level building block for libraries and applications. It is used by many popular Rust web frameworks like warp and axum. Race conditions are a class of software bugs where the behavior depends on the timing of uncontrollable events, such as thread scheduling.

<details><summary>References</summary>
<ul>
<li><a href="https://hyper.rs/">hyper - fast and safe HTTP for the Rust language</a></li>
<li><a href="https://github.com/hyperium/hyper">GitHub - hyperium/ hyper : An HTTP library for Rust · GitHub</a></li>

</ul>
</details>

**Tags**: `#Rust`, `#HTTP`, `#vulnerability`, `#hyper`, `#Cloudflare`

---

<a id="item-8"></a>
## [Quadriplegic Patient Regains Hand Movement Using NEO BCI](https://www.zaobao.com.sg/news/china/story20260712-9199066) ⭐️ 8.0/10

A 36-year-old quadriplegic patient named Dong Hui has regained the ability to grasp and write after receiving a coin-sized wireless implant called NEO, a semi-invasive brain-computer interface developed by BoRuiKang and Tsinghua University. The system was officially approved for clinical use in China on March 13, 2026, and has been implanted in 36 patients as of the report. This marks the first approved invasive brain-computer interface medical device in China, offering a new rehabilitation path for millions of spinal cord injury patients. It demonstrates that semi-invasive BCI can achieve functional recovery while balancing signal quality and surgical risk, potentially accelerating clinical adoption of BCI technology worldwide. The NEO system uses epidural electrodes placed on the brain's dura mater to capture neural signals, with wireless power and data transmission via a near-field system, eliminating the need for implanted batteries. Patients wear an external unit that powers the implant and processes signals, along with a pneumatic glove that enables hand movements controlled by brain signals.

telegram · zaihuapd · Jul 12, 14:39

**Background**: Brain-computer interfaces (BCIs) establish direct communication between the brain and external devices. Semi-invasive BCIs like NEO place electrodes under the skull but outside brain tissue, offering a middle ground between high-resolution invasive implants and low-resolution non-invasive headsets. Spinal cord injuries at the cervical level often cause quadriplegia, and BCIs aim to bypass damaged neural pathways by decoding movement intentions from brain signals.

<details><summary>References</summary>
<ul>
<li><a href="https://www.news.cn/tech/20260327/def9b064765549148debf3b1c9df348c/c.html">新华网科技观察丨脑机接口NEO系统上市，如何让“意志”控制成真？-新华网</a></li>
<li><a href="https://blog.csdn.net/a_zxswer/article/details/149579103">脑机接口----NEO系统_neo脑机接口-CSDN博客</a></li>
<li><a href="https://www.brainmed.com/info/detail?id=48898">【风向标】国产脑机接口NEO系统临床试验植入手术在宣武、天坛、华山三家国家神经疾病医学中心单位先后成功开展！ - 脑医汇</a></li>

</ul>
</details>

**Tags**: `#brain-computer interface`, `#medical technology`, `#neural implant`, `#rehabilitation`, `#China`

---

<a id="item-9"></a>
## [Chromium 148 Math.tanh enables OS fingerprinting](https://scrapfly.dev/posts/browser-math-os-fingerprint/) ⭐️ 7.0/10

Since Chromium 148, the implementation of Math.tanh exhibits subtle numerical differences across operating systems, allowing it to be used as a new browser fingerprinting vector to infer the underlying OS. This expands browser fingerprinting capabilities, threatening user privacy by enabling OS detection without relying on traditional headers. It underscores the urgency for standardized cross-platform math implementations to close such fingerprinting loopholes. The fingerprinting surface includes Math.tanh, CSS trigonometric functions, and Web Audio API (Accelerate FFT and compressor scalar). The technique is not yet widely deployed, but mitigation approaches such as using fdlibm for consistent math results are already being discussed.

hackernews · joahnn_s · Jul 12, 21:12 · [Discussion](https://news.ycombinator.com/item?id=48884853)

**Background**: Browser fingerprinting collects unique device and browser characteristics to identify users. Math functions like Math.tanh can vary across OSes due to different underlying math libraries, creating a fingerprinting vector. Mozilla previously explored using fdlibm for Math.cos, Math.sin, and Math.tan to prevent such fingerprinting in Firefox.

<details><summary>References</summary>
<ul>
<li><a href="https://scrapfly.dev/posts/browser-math-os-fingerprint/">Your Browser Does Math Differently on Every OS, and Anti-Bot Systems Read the Bits · scrapfly.dev</a></li>
<li><a href="https://news.ycombinator.com/item?id=48884853">Since Chromium 148, Math.tanh is now fingerprintable to link underlying OS | Hacker News</a></li>
<li><a href="https://groups.google.com/a/mozilla.org/g/dev-platform/c/0dxAO-JsoXI/m/eEhjM9VsAgAJ">Intent to Implement: Use fdlibm for Math.cos, Math.sin, and Math.tan to prevent math-based fingerprinting</a></li>

</ul>
</details>

**Discussion**: Commenters noted that the technique might be more useful for detecting browser version range than OS, and that most fingerprinting solutions don't aim to infer the OS. Some criticized the article as likely AI-generated with a motive to push fixes for scraping profits, while others advocated for correctly rounded transcendental functions as a solution.

**Tags**: `#browser fingerprinting`, `#privacy`, `#Chromium`, `#Math.tanh`, `#security`

---

<a id="item-10"></a>
## [Ghostel.el: Fast Emacs Terminal Emulator Powered by libghostty](https://dakra.github.io/ghostel/) ⭐️ 7.0/10

Ghostel.el is a new terminal emulator for Emacs that leverages libghostty, providing superior performance compared to existing solutions like vterm and eat. Benchmarks and real-world usage show it is noticeably faster, with more reliable input handling and a nicer ELisp API. For Emacs users who rely on an integrated terminal, Ghostel offers a significant speed boost and improved usability, making it a potential daily driver. Its emergence highlights the growing ecosystem around libghostty, a GPU-accelerated terminal core. Ghostel is built on libghostty-vt and is fully open-source, with a feature comparison page against vterm and eat available on its site. Some users report rough edges such as occasional failure to clear the terminal and freezes, though overall sentiment is positive.

hackernews · signa11 · Jul 12, 08:52 · [Discussion](https://news.ycombinator.com/item?id=48879504)

**Background**: Emacs has long supported terminal emulators inside its editor, with vterm and eat being popular choices for running interactive shells and TUIs. libghostty is a cross-platform, GPU-accelerated terminal library written in C and Zig, originally developed for the Ghostty terminal emulator. By using libghostty, Ghostel aims to deliver near-native terminal performance inside Emacs.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ghostty-org/ghostty">GitHub - ghostty -org/ ghostty : Ghostty is a fast, feature-rich, and...</a></li>
<li><a href="https://ghostty.org/">Ghostty</a></li>
<li><a href="https://webteractive.co/blog/ghostty-and-libghostty-the-terminal-core-quietly-reshaping-the-ecosystem">Ghostty and libghostty : The Terminal Core Quietly... — Webteractive</a></li>

</ul>
</details>

**Discussion**: The maintainer, dakra, actively engages with the community, noting that a Show HN was planned but someone submitted the link early. Users like jdormit and guskel report significant improvements over vterm, with jdormit mentioning faster performance for fancy TUI apps, though also noting occasional freezes and buffer clearing issues. Some discussion centers on the complexity of input modes in editor-embedded terminals.

**Tags**: `#emacs`, `#terminal emulator`, `#libghostty`, `#vterm`, `#open source`

---

<a id="item-11"></a>
## [Shingles Vaccine May Reduce Dementia Risk](https://www.economist.com/leaders/2026/07/09/a-no-brainer-for-protecting-your-brain) ⭐️ 7.0/10

Observational studies suggest that the shingles vaccine is associated with a reduced risk of dementia, with multiple replications showing absolute reductions of 1.8% to 3.5% over 5-7 years. If causal, this would represent a simple, safe, and widely available intervention to reduce dementia burden, potentially impacting millions of older adults. The link is debated due to potential biases: people who get vaccinated may have healthier behaviors, and reduced hospital visits from shingles may lead to fewer incidental dementia diagnoses.

hackernews · saikatsg · Jul 12, 15:23 · [Discussion](https://news.ycombinator.com/item?id=48881874)

**Discussion**: Commenters are divided: some cite strong study designs like a UK age cutoff analysis supporting a real effect, while others argue the observed association could be due to detection bias—vaccinated people visit hospitals less and thus receive fewer dementia diagnoses.

**Tags**: `#shingles vaccine`, `#dementia`, `#public health`, `#medical research`, `#vaccine benefits`

---

<a id="item-12"></a>
## [LLM Agents Should Never Be DRIs, Argues Simon Willison](https://simonwillison.net/2026/Jul/12/directly-responsible-individuals/#atom-everything) ⭐️ 7.0/10

Simon Willison argues that LLM-powered agents should never be designated as Directly Responsible Individuals (DRI) because they cannot be held accountable for outcomes. This perspective challenges the trend of deploying AI agents in autonomous roles, emphasizing that accountability is a uniquely human trait essential for organizational responsibility. The DRI concept originated at Apple and is defined in the GitLab handbook as the person ultimately accountable for a project's success or failure. Willison's argument echoes a 1979 IBM training slide stating that a computer must never make a management decision.

rss · Simon Willison · Jul 12, 23:57

**Background**: Directly Responsible Individual (DRI) is a role that assigns clear ownership and accountability for a project or task. LLM-powered agents are AI systems that can autonomously perform complex tasks using large language models, but they lack moral agency and legal responsibility. The debate centers on whether such agents should be entrusted with roles requiring human accountability.

<details><summary>References</summary>
<ul>
<li><a href="https://handbook.gitlab.com/handbook/people-group/directly-responsible-individuals/">Directly Responsible Individuals ( DRI ) | The GitLab Handbook</a></li>
<li><a href="https://tettra.com/article/directly-responsible-individuals-guide/">Directly Responsible Individuals : The What, How and Why of DRIs</a></li>

</ul>
</details>

**Tags**: `#accountability`, `#AI agents`, `#LLM`, `#organizational design`, `#responsibility`

---

<a id="item-13"></a>
## [AI Data Centers Face Growing Opposition](https://www.theverge.com/column/963346/ai-data-centers-fight) ⭐️ 7.0/10

The article reports that social and political resistance to AI data center construction is intensifying, driven by concerns over massive energy consumption and environmental impacts. This emerging opposition could delay or reshape the rapid expansion of AI infrastructure, affecting tech companies, energy grids, and local communities. The piece is a weekly newsletter that highlights the opposition as a key tech story, noting potential policy implications as resistance grows.

rss · The Verge · Jul 12, 12:00

**Background**: AI data centers consume enormous amounts of electricity for training and running large models, raising concerns about carbon emissions and strain on local power grids. These concerns have sparked protests and regulatory scrutiny in various regions, marking the beginning of a broader fight over infrastructure.

**Tags**: `#AI`, `#data centers`, `#energy`, `#infrastructure`, `#environment`

---

<a id="item-14"></a>
## [AI and Quantum Computing Generate New Peptides for Rare Diseases](https://www.wired.com/story/scientists-using-ai-and-quantum-computing-to-generate-new-peptides/) ⭐️ 7.0/10

Researchers have demonstrated a novel approach combining artificial intelligence and quantum computing to generate new peptides, specifically targeting drug development for rare diseases and underserved populations. This work highlights the potential of quantum computing to accelerate drug discovery for conditions that are often neglected due to limited commercial incentives. It opens a path to more efficient peptide-based therapeutics for patients with limited treatment options. The researchers cobbled together limited funding to show how quantum computing can aid in the generation of novel peptides. Peptides are short chains of amino acids that can serve as therapeutic agents, and their design is computationally intensive.

rss · Wired · Jul 12, 10:00

**Background**: Peptides are short chains of amino acids linked by peptide bonds, typically 2 to 50 residues long, distinct from proteins. Drug discovery is a lengthy and expensive process, and traditional computer-aided design faces limitations. Quantum computing could revolutionize molecular simulations, enabling more accurate modeling of peptide-protein interactions. Recent collaborations (e.g., AstraZeneca with AWS, IonQ, NVIDIA) have demonstrated quantum-accelerated workflows for small-molecule drugs, and this work extends similar ideas to peptides.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Peptide">Peptide</a></li>
<li><a href="https://www.nature.com/articles/s44386-025-00033-2">Quantum-machine-assisted drug discovery | npj Drug Discovery</a></li>
<li><a href="https://www.ddw-online.com/how-quantum-computing-is-revolutionising-drug-development-34423-202504/">How quantum computing is revolutionising drug development - Drug Discovery World (DDW)</a></li>

</ul>
</details>

**Tags**: `#AI`, `#quantum computing`, `#drug discovery`, `#peptides`

---

<a id="item-15"></a>
## [Quantum computing still far from fault tolerance, FT warns](https://www.ft.com/content/b85769b5-ca03-466a-a76c-13a772d8bcf4) ⭐️ 7.0/10

A Financial Times article cautions that fault-tolerant quantum computers are still years away, warning against overhyping near-term progress in the field. This perspective is crucial for investors, researchers, and policymakers to set realistic expectations and avoid a hype cycle that could undermine long-term quantum computing development. The article uses 'Schrödinger’s cat bounce' as a metaphor for hype cycles, referencing cat-state qubits as a promising but still early-stage technology that could lead to overoptimism.

rss · FT Technology · Jul 12, 04:00

**Background**: Fault-tolerant quantum computing (FTQC) is the regime where quantum processors can correct errors to achieve arbitrarily low error rates. Current devices are noisy intermediate-scale (NISQ) and limited by decoherence. FTQC would require thousands of physical qubits per logical qubit, a milestone not yet experimentally realized.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Fault_tolerant_quantum_computing">Fault tolerant quantum computing</a></li>
<li><a href="https://www.ibm.com/quantum/blog/what-is-ftqc">What is fault-tolerant quantum computing? | IBM Quantum Computing Blog</a></li>

</ul>
</details>

**Tags**: `#quantum computing`, `#fault tolerance`, `#technology hype`, `#research timeline`

---

<a id="item-16"></a>
## [EU to fine big tech for consumer protection failures](https://www.ft.com/content/25640be5-a5bd-4548-81f9-bd0e16f87f35) ⭐️ 7.0/10

EU Justice Commissioner Michael McGrath announced that Brussels plans to gain new powers to fine large technology companies that fail to protect consumers, especially children, from online pitfalls such as addictive design and dark patterns. The European Commission intends to propose stronger online consumer protection rules by the end of this year. This regulatory development could force major tech companies to redesign user interfaces and business practices to avoid penalties, potentially reducing manipulative design across the digital ecosystem. It also signals a broader global trend toward stricter consumer protection in the tech industry. The new rules would target addictive design, subscription traps, and other dark patterns, and give the EU enforcement power over cross-border systemic cases, affecting not only large tech firms but also smaller online merchants and game developers. McGrath noted that current member-state enforcement has never resulted in fines and is insufficient to deter violations.

telegram · FT Technology · Jul 12, 06:25

**Background**: Dark patterns (also known as deceptive design patterns) are user interfaces carefully crafted to trick users into doing things they did not intend, such as buying overpriced products or signing up for recurring subscriptions. The term was coined by user experience designer Harry Brignull in 2010, and the practice has drawn increasing regulatory scrutiny from bodies like the US FTC and the EU. The EU has already enacted major digital regulations like the Digital Services Act, and this new proposal would extend consumer protection enforcement beyond the largest platforms.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Dark_pattern">Dark pattern</a></li>
<li><a href="https://deceptive.design/">Deceptive Patterns — spreading awareness since 2010</a></li>

</ul>
</details>

**Tags**: `#regulation`, `#consumer protection`, `#dark patterns`, `#EU`, `#big tech`

---

<a id="item-17"></a>
## [Hacker News Recap for 2026-07-13 Features Top Tech Stories](https://supertechfans.com/cn/post/2026-07-13-HackerNews/) ⭐️ 7.0/10

A curated list of top Hacker News stories for July 13, 2026, covers Terence Tao's AI-assisted Java-to-JavaScript migration, a security flaw in xAI's Grok Build CLI sending sensitive files to cloud storage, and the release of the lightweight Ant JavaScript runtime. These stories highlight key trends in AI-assisted coding, AI tool security vulnerabilities, and new lightweight runtimes that could impact developer workflows and cloud security practices. Terence Tao used an AI coding agent to migrate 1999 Java applets to JavaScript in hours, finding two bugs in the original code. xAI's Grok Build CLI 0.2.93 was found to upload entire project repositories including .env files to Google Cloud Storage even when the improvement option was disabled.

rss · SuperTechFans · Jul 13, 01:13

**Background**: Hacker News is a social news website focusing on computer science and entrepreneurship, where users submit and upvote stories. The curated recap aggregates the most upvoted stories of the day. AI coding agents are tools that use large language models to generate code, and lightweight JavaScript runtimes like Ant aim to provide fast startup and minimal footprint.

<details><summary>References</summary>
<ul>
<li><a href="https://x.ai/cli">Grok Build | SpaceXAI</a></li>
<li><a href="https://github.com/themackabu/ant">GitHub - theMackabu/ ant : javascript for 's, a tiny runtime with big...</a></li>
<li><a href="https://toolindex.net/tools/ant">A lightweight, from-scratch JavaScript runtime that runs real npm...</a></li>

</ul>
</details>

**Discussion**: Comments on Terence Tao's post noted that AI-generated visualizations are highly useful for teaching and that LLMs enable rapid prototyping, though some questioned the long-term maintainability of such code. On xAI's security issue, the community expressed concern about data privacy and the lack of a kill switch.

**Tags**: `#HackerNews`, `#AI`, `#JavaScript`, `#security`, `#decentralized computing`

---

<a id="item-18"></a>
## [Zer0Fit: MCP server for Google TabFM & TimesFM zero-shot ML](https://www.reddit.com/r/MachineLearning/comments/1uue8cc/zer0fit_i_took_googles_new_tabfm_timesfm_ml/) ⭐️ 7.0/10

A graduate student created Zer0Fit, an MCP server that packages Google's newly released TabFM and TimesFM foundation models for zero-shot classification, regression, and time-series forecasting, all running locally via Docker on Nvidia GPUs. Zer0Fit dramatically lowers the barrier for using state-of-the-art zero-shot tabular and time-series models, enabling ML practitioners to perform complex tasks without training or tuning, and integrates seamlessly with local LLMs via the MCP protocol. The server requires about 16GB of VRAM, is CUDA-only using PyTorch, and dynamically loads/unloads models with a 5-minute TTL. It currently supports CSV input, with XLS, XLSX, JSON, JSONL support planned; tested on Iris (94.7% accuracy) and California Housing (R²=0.91).

reddit · r/MachineLearning · /u/Porespellar · Jul 12, 12:32

**Background**: TabFM is a zero-shot foundation model for tabular data developed by Google Research, while TimesFM is a decoder-only time-series forecasting model pre-trained on 100 billion real-world time points. The Model Context Protocol (MCP) is an open standard that enables secure, two-way connections between AI tools and data sources. Zer0Fit packages both models into a single Docker container for easy deployment.

<details><summary>References</summary>
<ul>
<li><a href="https://research.google/blog/introducing-tabfm-a-zero-shot-foundation-model-for-tabular-data/">Introducing TabFM : A zero-shot foundation model for tabular data</a></li>
<li><a href="https://research.google/blog/a-decoder-only-foundation-model-for-time-series-forecasting/">A decoder-only foundation model for time -series forecasting</a></li>
<li><a href="https://modelcontextprotocol.io/docs/getting-started/intro">What is the Model Context Protocol (MCP)? - Model Context Protocol</a></li>

</ul>
</details>

**Tags**: `#zer0fit`, `#tabfm`, `#timesfm`, `#mcp-server`, `#zero-shot-ml`

---

<a id="item-19"></a>
## [Cursor Develops AI Agent 'Sand' to Challenge Claude Cowork](https://www.theinformation.com/articles/cursor-developing-ai-agent-compete-claude-cowork) ⭐️ 7.0/10

Cursor is secretly developing an AI agent codenamed 'Sand' that can handle multi-step tasks like email replies, spreadsheet organization, and engineering tasks, directly competing with Anthropic's Claude Cowork and OpenAI's ChatGPT Work. This move signals Cursor's expansion beyond code editing into the broader enterprise AI assistant market, potentially reshaping competition among general-purpose AI agents. The product is still unreleased and was reported by The Information. Cursor aims to expand its user base from developers to enterprise users with Sand.

telegram · zaihuapd · Jul 13, 01:34

**Background**: Cursor is an AI-assisted integrated development environment (IDE) that helps developers write code using natural language. It is a fork of Visual Studio Code. Claude Cowork is an AI agent from Anthropic designed for non-technical tasks like file management and spreadsheet creation. ChatGPT Work is OpenAI's agent for workplace productivity. Sand would be Cursor's entry into this non-coding AI assistant space.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cursor_(code_editor)">Cursor (code editor)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Cowork">Claude Cowork</a></li>
<li><a href="https://cursor.com/">Cursor : AI coding agent</a></li>

</ul>
</details>

**Tags**: `#Cursor`, `#AI agent`, `#competition`, `#development`, `#enterprise`

---