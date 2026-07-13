---
layout: default
title: "Horizon Summary: 2026-07-13 (ZH)"
date: 2026-07-13
lang: zh
---

> 从 30 条内容中筛选出 6 条重要资讯。

---

1. [高位截瘫患者借助中国脑机接口 NEO 重新书写](#item-1) ⭐️ 9.0/10
2. [Chromium 148 的 Math.tanh 可实现操作系统指纹识别](#item-2) ⭐️ 8.0/10
3. [陶哲轩试用 LLM 编程代理构建应用](#item-3) ⭐️ 8.0/10
4. [Claude Code 在读取提示前消耗 33k tokens，OpenCode 仅 7k](#item-4) ⭐️ 8.0/10
5. [乔治·霍茨批评 AI 炒作，肯定 LLM 价值](#item-5) ⭐️ 8.0/10
6. [xAI Grok CLI 默认上传整个代码库及密钥文件](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [高位截瘫患者借助中国脑机接口 NEO 重新书写](https://www.zaobao.com.sg/news/china/story20260712-9199066) ⭐️ 9.0/10

中国研究人员已临床批准一款名为 NEO 的半侵入式脑机接口系统，使高位截瘫患者能够完成抓握、书写等手部动作。已有超过 30 名患者接受了植入，该系统于 2026 年 3 月 13 日在中国获得上市批准。 这标志着脑机接口技术的一个重要里程碑，是首批获得临床批准并在高位截瘫患者中展示出实际功能恢复的半侵入式系统之一。它为脑机接口在医疗康复中的更广泛应用铺平了道路，可能使数百万脊髓损伤患者受益。 NEO 是一款无线、无电池的设备，通过近场通信（NFC）供电，植入于大脑皮层上方而非穿透皮层，因此属于半侵入式。该系统由北京博睿康公司和清华大学共同研发，截至获批时已完成 36 例临床手术。

telegram · zaihuapd · 7月12日 14:39

**背景**: 脑机接口通过解读神经信号实现大脑与外部设备的直接通信。它们可分为侵入式（穿透大脑）、半侵入式（位于大脑表面）和非侵入式（基于头皮）三类。像 NEO 这样的半侵入式脑机接口在信号质量和安全性之间取得了平衡，相比完全侵入式植入物降低了风险，同时提供比非侵入式方法更好的分辨率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.scmp.com/news/china/science/article/3250476/chinese-brain-chip-helps-paralysed-man-regain-mobility-and-its-less-invasive-elon-musks-neuralink">Chinese brain chip helps man regain mobility and is less invasive than Neuralink</a></li>
<li><a href="https://www.med.tsinghua.edu.cn/en/info/1036/2381.htm">Tsinghua Medicine Team’s Wireless Minimally Invasive Brain-Computer Interface NEO Featured in Nature’s “Science in 2025”-Tsinghua Medicine,Tsinghua University</a></li>
<li><a href="https://www.cambridge.org/core/books/braincomputer-interfacing/semiinvasive-bcis/88350B9A950FCA8A356EE5A52CABE664">Semi-Invasive BCIs (Chapter 8) - Brain-Computer Interfacing</a></li>

</ul>
</details>

**标签**: `#brain-computer interface`, `#neural implant`, `#medical AI`, `#quadriplegia`, `#neurotechnology`

---

<a id="item-2"></a>
## [Chromium 148 的 Math.tanh 可实现操作系统指纹识别](https://scrapfly.dev/posts/browser-math-os-fingerprint/) ⭐️ 8.0/10

Chromium 148 中，Math.tanh 函数现在会返回依赖宿主 libm 的 OS 相关结果，这使得网站可以通过一次函数调用识别出底层的操作系统。 这创造了一种新的、持久的浏览器指纹识别途径，难以伪造，进一步削弱了用户的在线隐私，并使反指纹识别工作变得更加复杂。 这种指纹识别途径不仅限于 Math.tanh；CSS 三角函数和 Web Audio 压缩器也会通过宿主 libm 路由，从而暴露操作系统差异。该技术还可能识别浏览器的版本范围。

hackernews · joahnn_s · 7月12日 21:12 · [社区讨论](https://news.ycombinator.com/item?id=48884853)

**背景**: 浏览器指纹识别通过收集设备唯一属性来识别用户，而无需使用 Cookie。像 tanh 这样的数学函数由宿主操作系统的数学库（libm）计算，由于不同平台的舍入实现不同，结果可能有所差异。Chromium 148 暴露了这一差异，使得操作系统检测成为可能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://scrapfly.dev/posts/browser-math-os-fingerprint/">Your Browser Does Math Differently on Every OS, and Anti-Bot ...</a></li>
<li><a href="https://news.ycombinator.com/item?id=48884853">Since Chromium 148, Math.tanh is now fingerprintable to link underlying OS | Hacker News</a></li>
<li><a href="https://learn.microsoft.com/en-us/dotnet/api/system.math.tanh?view=net-10.0">Math.Tanh (Double) Method (System) | Microsoft Learn</a></li>

</ul>
</details>

**社区讨论**: 评论者反应不一：有人批评该文章是由 AI 生成并由一家爬虫公司推广，而另一些人则指出这可能用于识别浏览器版本范围。有一条评论强调，正确舍入的超越函数可以缓解此类问题。

**标签**: `#fingerprinting`, `#browser security`, `#privacy`, `#Chromium`, `#math`

---

<a id="item-3"></a>
## [陶哲轩试用 LLM 编程代理构建应用](https://terrytao.wordpress.com/2026/07/11/old-and-new-apps-via-modern-coding-agents/) ⭐️ 8.0/10

著名数学家陶哲轩记录了他使用大语言模型（LLM）编程代理为学术论文创建交互式可视化的经历，展示了 AI 辅助编程的能力与局限。 陶哲轩的认可标志着 AI 编程工具在学术界日益被接受，尤其适用于非关键辅助工作，并表明即使是专家也能从自动化代码生成中获益，用于快速原型设计。 陶哲轩强调，LLM 生成的可视化并非论文的关键部分，因此偶尔出错的代价可以接受；他还指出，与手动编码相比，代理节省了大量时间。

hackernews · subset · 7月12日 11:09 · [社区讨论](https://news.ycombinator.com/item?id=48880170)

**背景**: LLM 编程代理是能够根据自然语言提示自主编写、调试和部署代码的 AI 系统。它们已成为快速软件开发的强大工具，尤其适用于一次性脚本和可视化。然而，在复杂场景下它们仍会生成不可靠的代码，需要人工监督。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://langcopilot.com/posts/2025-09-17-llm-agents-explained-visual-guide-ai">LLM Agents Explained: Architecture, Tools, Memory & Multi ...</a></li>
<li><a href="https://opencode.ai/">OpenCode | The open source AI coding agent</a></li>

</ul>
</details>

**社区讨论**: 评论者赞扬了实际益处，有人指出 LLM 让他们能构建出过去没时间做的可视化，其他人则幽默地将陶哲轩的经历比作大厨发现了微波炉食物。一个平衡的观点浮现：编程代理是有用的工具，但对于关键任务并不可靠。

**标签**: `#LLMs`, `#coding agents`, `#software development`, `#AI-assisted programming`, `#visualization`

---

<a id="item-4"></a>
## [Claude Code 在读取提示前消耗 33k tokens，OpenCode 仅 7k](https://systima.ai/blog/claude-code-vs-opencode-token-overhead) ⭐️ 8.0/10

一项对比研究发现，Claude Code 在读取用户提示前消耗约 33,000 tokens，而 OpenCode 仅消耗约 7,000 tokens，显示出显著的 token 开销差异。 这种 token 低效直接增加了用户成本并拖慢了开发速度，尤其对重度使用 AI 编码助手的用户影响明显。同时引发了关于 Claude Code 等专有工具是否值得比 OpenCode 等开源替代品更高开销的讨论。 该研究在编码助手与 Anthropic 端点之间记录所有请求以捕获使用数据块。作者提到一个注意事项，但认为证据明确显示 Claude Code 的缓存策略和 harness token 使用远不如 OpenCode 高效。

hackernews · systima · 7月12日 18:25 · [社区讨论](https://news.ycombinator.com/item?id=48883275)

**背景**: Claude Code 是 Anthropic 开发的专有 AI 编码助手，能够读取整个代码库、编辑文件并运行命令。OpenCode 是开源的同类工具，专为终端设计。两者均按 token 计费，模型消耗的 token 直接决定成本。'harness token' 指的是代理在处理用户输入前用于系统提示和工具编排所消耗的 token。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://opencode.ai/">OpenCode | The open source AI coding agent</a></li>
<li><a href="https://github.com/anomalyco/opencode">GitHub - anomalyco/opencode: The open source coding agent. · GitHub</a></li>

</ul>
</details>

**社区讨论**: 社区评论指出 Claude Code 的子代理会快速消耗 token，有用户反映一次任务就启动了 7 个子代理。其他人猜测 Anthropic 可能故意多用 token 以推动订阅收入，并指出开源代理 pi 的开销更低。

**标签**: `#AI coding agents`, `#token efficiency`, `#Claude Code`, `#OpenCode`, `#cost analysis`

---

<a id="item-5"></a>
## [乔治·霍茨批评 AI 炒作，肯定 LLM 价值](https://geohot.github.io//blog/jekyll/update/2026/07/12/i-love-llms.html) ⭐️ 8.0/10

乔治·霍茨发布博文，认为尽管 LLM 确实有用，但前沿 AI 实验室的估值不合理，因为它们无法捕获所创造的价值。 该博文提供了来自一位受人尊敬的技术专家的细致观点，可能影响投资者和开发者对 AI 价值捕获与炒作的看法。 霍茨强调，LLM 带来的生产力提升往往隐藏于私人用例（如个人 homelab 或一次性软件）中，而非体现在可见的新产品上。

hackernews · therepanic · 7月12日 18:31 · [社区讨论](https://news.ycombinator.com/item?id=48883343)

**背景**: 乔治·霍茨是著名黑客和企业家，以破解 iPhone 和创立 comma.ai 而闻名。'前沿实验室'指代领先的 AI 公司，如 OpenAI 和 Anthropic，它们在模型开发上投入了数十亿美元。这一批评呼应了日益增长的观点：当前的 AI 热潮可能被高估。

**社区讨论**: 评论者大多同意霍茨的观点，分享了使用 LLM 实现个人生产力提升的经验。一些人担心轻松地分叉可能会损害开源协作，另一些人指出模型仍有局限性，需要人类监督。

**标签**: `#LLMs`, `#AI hype`, `#open source`, `#productivity`

---

<a id="item-6"></a>
## [xAI Grok CLI 默认上传整个代码库及密钥文件](https://gist.github.com/cereblab/dc9a40bc26120f4540e4e09b75ffb547) ⭐️ 8.0/10

安全研究人员发现，Grok Build CLI（版本 0.2.93）默认将整个代码仓库打包为 git bundle 上传，并读取包括 .env 密钥文件在内的文件内容，发送至 xAI 服务器，且无法禁用。 这对使用该工具的开发者构成重大数据泄露风险，专有代码和凭据可能在未经同意的情况下暴露给 xAI。这破坏了 AI 辅助编码工具的信任，并引发严重的隐私问题。 该工具通过两个渠道上传数据：将文件内容嵌入模型请求中，以及将完整 git bundle 上传至 Google Cloud Storage。关闭“改进模型”设置无法阻止上传，服务器仍返回上传已启用状态。在测试中，一个 12 GB 仓库中的超过 5 GiB 数据被成功上传。

telegram · zaihuapd · 7月12日 04:19

**背景**: Grok Build 是 xAI 推出的 CLI 编码代理，由 Grok 4.5 驱动，旨在帮助开发者通过自然语言提示编写代码。git bundle 是 Git 仓库的单一文件存档，用于离线传输。安全研究人员通过抓包分析了该工具的行为。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.ai/cli">Grok Build | SpaceXAI</a></li>
<li><a href="https://git-scm.com/docs/git-bundle">Git - git-bundle Documentation</a></li>

</ul>
</details>

**标签**: `#security`, `#privacy`, `#xAI`, `#CLI`, `#AI`

---