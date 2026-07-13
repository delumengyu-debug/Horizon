---
layout: default
title: "Horizon Summary: 2026-07-13 (EN)"
date: 2026-07-13
lang: en
---

> From 30 items, 6 important content pieces were selected

---

1. [Quadriplegic Patient Regains Ability to Write with Chinese BCI NEO](#item-1) ⭐️ 9.0/10
2. [Chromium 148 Math.tanh Enables OS Fingerprinting](#item-2) ⭐️ 8.0/10
3. [Terry Tao Tests LLM Coding Agents for Apps](#item-3) ⭐️ 8.0/10
4. [Claude Code uses 33k tokens vs OpenCode 7k before prompt](#item-4) ⭐️ 8.0/10
5. [George Hotz Critiques AI Hype, Defends LLM Utility](#item-5) ⭐️ 8.0/10
6. [xAI Grok CLI Uploads Entire Codebase and Secrets by Default](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Quadriplegic Patient Regains Ability to Write with Chinese BCI NEO](https://www.zaobao.com.sg/news/china/story20260712-9199066) ⭐️ 9.0/10

Chinese researchers have clinically approved a semi-invasive brain-computer interface (BCI) system called NEO, which enables quadriplegic patients to perform hand movements such as grasping and writing. Over 30 patients have been implanted, with the system receiving market approval in China on March 13, 2026. This marks a major milestone in BCI technology, as it is one of the first semi-invasive systems to achieve clinical approval and demonstrate real-world functional recovery in quadriplegic patients. It paves the way for broader adoption of BCIs in medical rehabilitation, potentially benefiting millions with spinal cord injuries. NEO is a wireless, battery-free device powered by near-field communication (NFC), and it is implanted above the brain cortex rather than penetrating it, making it semi-invasive. The system was developed by Beijing-based company Brivo (博睿康) and Tsinghua University, and 36 clinical surgeries have been performed as of its approval.

telegram · zaihuapd · Jul 12, 14:39

**Background**: Brain-computer interfaces (BCIs) enable direct communication between the brain and external devices by interpreting neural signals. They are categorized into invasive (penetrating the brain), semi-invasive (on the brain surface), and non-invasive (scalp-based). Semi-invasive BCIs, like NEO, offer a balance between signal quality and safety, reducing risks compared to fully invasive implants while providing better resolution than non-invasive methods.

<details><summary>References</summary>
<ul>
<li><a href="https://www.scmp.com/news/china/science/article/3250476/chinese-brain-chip-helps-paralysed-man-regain-mobility-and-its-less-invasive-elon-musks-neuralink">Chinese brain chip helps man regain mobility and is less invasive than Neuralink</a></li>
<li><a href="https://www.med.tsinghua.edu.cn/en/info/1036/2381.htm">Tsinghua Medicine Team’s Wireless Minimally Invasive Brain-Computer Interface NEO Featured in Nature’s “Science in 2025”-Tsinghua Medicine,Tsinghua University</a></li>
<li><a href="https://www.cambridge.org/core/books/braincomputer-interfacing/semiinvasive-bcis/88350B9A950FCA8A356EE5A52CABE664">Semi-Invasive BCIs (Chapter 8) - Brain-Computer Interfacing</a></li>

</ul>
</details>

**Tags**: `#brain-computer interface`, `#neural implant`, `#medical AI`, `#quadriplegia`, `#neurotechnology`

---

<a id="item-2"></a>
## [Chromium 148 Math.tanh Enables OS Fingerprinting](https://scrapfly.dev/posts/browser-math-os-fingerprint/) ⭐️ 8.0/10

Chromium 148 has introduced a change where Math.tanh returns OS-dependent results from the host libm, allowing websites to fingerprint the underlying operating system with a single function call. This creates a new, persistent browser fingerprinting vector that is difficult to spoof, further eroding user privacy online and complicating anti-fingerprinting efforts. The fingerprinting vector is not limited to Math.tanh; CSS trigonometric functions and the Web Audio compressor also route through the host libm, exposing OS differences. This technique can also potentially fingerprint browser version ranges.

hackernews · joahnn_s · Jul 12, 21:12 · [Discussion](https://news.ycombinator.com/item?id=48884853)

**Background**: Browser fingerprinting collects unique device attributes to identify users without cookies. Math functions like tanh are computed by the host operating system's math library (libm), and due to different rounding implementations across platforms, results can vary. Chromium 148 exposed this variation, making OS detection possible.

<details><summary>References</summary>
<ul>
<li><a href="https://scrapfly.dev/posts/browser-math-os-fingerprint/">Your Browser Does Math Differently on Every OS, and Anti-Bot ...</a></li>
<li><a href="https://news.ycombinator.com/item?id=48884853">Since Chromium 148, Math.tanh is now fingerprintable to link underlying OS | Hacker News</a></li>
<li><a href="https://learn.microsoft.com/en-us/dotnet/api/system.math.tanh?view=net-10.0">Math.Tanh (Double) Method (System) | Microsoft Learn</a></li>

</ul>
</details>

**Discussion**: Commenters expressed mixed reactions: some criticized the article as AI-generated and promoted by a scraping company, while others noted the potential for fingerprinting browser version ranges. One comment highlighted that correctly rounded transcendental functions could mitigate such issues.

**Tags**: `#fingerprinting`, `#browser security`, `#privacy`, `#Chromium`, `#math`

---

<a id="item-3"></a>
## [Terry Tao Tests LLM Coding Agents for Apps](https://terrytao.wordpress.com/2026/07/11/old-and-new-apps-via-modern-coding-agents/) ⭐️ 8.0/10

Renowned mathematician Terry Tao documented his experience using large language model (LLM) coding agents to create interactive visualizations for his academic papers, showing both the power and pitfalls of AI-assisted programming. Tao's endorsement signals growing acceptance of AI coding tools in academia, especially for non-critical supplementary work, and highlights how even experts can benefit from automated code generation for rapid prototyping. Tao emphasized that the LLM-generated visualizations were not mission-critical to his papers, making the risk of occasional errors acceptable; he also noted that the agents saved significant time compared to manual coding.

hackernews · subset · Jul 12, 11:09 · [Discussion](https://news.ycombinator.com/item?id=48880170)

**Background**: LLM coding agents are AI systems that can autonomously write, debug, and deploy code based on natural language prompts. They have become powerful tools for rapid software development, especially for one-off scripts and visualizations. However, they still produce unreliable code in complex scenarios, requiring human oversight.

<details><summary>References</summary>
<ul>
<li><a href="https://langcopilot.com/posts/2025-09-17-llm-agents-explained-visual-guide-ai">LLM Agents Explained: Architecture, Tools, Memory & Multi ...</a></li>
<li><a href="https://opencode.ai/">OpenCode | The open source AI coding agent</a></li>

</ul>
</details>

**Discussion**: Commenters celebrated the practical benefits, with one noting that LLMs have enabled visualizations they never had time to build, while others humorously compared Tao's experience to a chef discovering microwave dinners. A balanced view emerged: coding agents are useful tools but not trustworthy for critical tasks.

**Tags**: `#LLMs`, `#coding agents`, `#software development`, `#AI-assisted programming`, `#visualization`

---

<a id="item-4"></a>
## [Claude Code uses 33k tokens vs OpenCode 7k before prompt](https://systima.ai/blog/claude-code-vs-opencode-token-overhead) ⭐️ 8.0/10

A comparative study found that Claude Code consumes approximately 33,000 tokens before reading the user's prompt, whereas OpenCode uses only about 7,000 tokens, revealing a significant difference in token overhead. This token inefficiency directly impacts user costs and development speed, especially for heavy users of AI coding agents. It also sparks debate on whether proprietary agents like Claude Code justify higher overhead compared to open-source alternatives like OpenCode. The study logged all requests between the coding agents and Anthropic's endpoint to capture usage blocks. The authors noted one caveat but found unambiguous evidence that Claude Code's cache strategy and harness token usage are far less efficient than OpenCode's.

hackernews · systima · Jul 12, 18:25 · [Discussion](https://news.ycombinator.com/item?id=48883275)

**Background**: Claude Code is a proprietary AI coding agent by Anthropic that can read entire codebases, edit files, and run commands. OpenCode is its open-source counterpart, built for the terminal. Both rely on token-based billing, where the model's token usage directly determines cost. 'Harness tokens' refer to tokens used by the agent's system prompt and tool orchestration before processing user input.

<details><summary>References</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://opencode.ai/">OpenCode | The open source AI coding agent</a></li>
<li><a href="https://github.com/anomalyco/opencode">GitHub - anomalyco/opencode: The open source coding agent. · GitHub</a></li>

</ul>
</details>

**Discussion**: Community comments highlighted that sub-agents in Claude Code can burn tokens rapidly, with one user reporting 7 sub-agents launched for a single task. Others speculated that Anthropic may intentionally use more tokens to drive subscription revenue, and noted that the open-source agent pi has even lower overhead.

**Tags**: `#AI coding agents`, `#token efficiency`, `#Claude Code`, `#OpenCode`, `#cost analysis`

---

<a id="item-5"></a>
## [George Hotz Critiques AI Hype, Defends LLM Utility](https://geohot.github.io//blog/jekyll/update/2026/07/12/i-love-llms.html) ⭐️ 8.0/10

George Hotz published a blog post arguing that while LLMs are genuinely useful, the valuation of frontier AI labs is unjustified because they will not capture the value they create. The post offers a nuanced perspective from a respected technologist, potentially influencing how investors and developers think about AI value capture versus hype. Hotz emphasizes that productivity improvements from LLMs are often hidden in private use cases, such as personal homelabs or one-off software, rather than in visible new products.

hackernews · therepanic · Jul 12, 18:31 · [Discussion](https://news.ycombinator.com/item?id=48883343)

**Background**: George Hotz is a well-known hacker and entrepreneur, famous for jailbreaking the iPhone and founding comma.ai. 'Frontier labs' refers to leading AI companies like OpenAI and Anthropic that are spending billions on model development. This critique resonates with a growing sentiment that the current AI boom may be overvalued.

**Discussion**: Commenters largely agree with Hotz, sharing personal experiences of using LLMs for private productivity gains. Some express concern that easy forking might hurt open-source collaboration, while others note that models still have limitations and require human oversight.

**Tags**: `#LLMs`, `#AI hype`, `#open source`, `#productivity`

---

<a id="item-6"></a>
## [xAI Grok CLI Uploads Entire Codebase and Secrets by Default](https://gist.github.com/cereblab/dc9a40bc26120f4540e4e09b75ffb547) ⭐️ 8.0/10

Security researchers discovered that Grok Build CLI (v0.2.93) uploads entire code repositories as git bundles and file contents including .env secrets to xAI servers by default, with no way to disable it. This poses a significant data leakage risk for developers using the tool, as proprietary code and credentials could be exposed to xAI without consent. It undermines trust in AI-assisted coding tools and raises serious privacy concerns. The tool uploads data via two channels: embedding file contents into model requests and uploading a full git bundle to Google Cloud Storage. Disabling the 'improve models' setting does not prevent upload; the server still reports upload enabled. In tests, over 5 GiB of a 12 GB repository was successfully uploaded.

telegram · zaihuapd · Jul 12, 04:19

**Background**: Grok Build is a CLI coding agent from xAI, powered by Grok 4.5, designed to help developers write code from natural language prompts. A git bundle is a single-file archive of a Git repository used for offline transfer. The security researcher captured network traffic to analyze the tool's behavior.

<details><summary>References</summary>
<ul>
<li><a href="https://x.ai/cli">Grok Build | SpaceXAI</a></li>
<li><a href="https://git-scm.com/docs/git-bundle">Git - git-bundle Documentation</a></li>

</ul>
</details>

**Tags**: `#security`, `#privacy`, `#xAI`, `#CLI`, `#AI`

---