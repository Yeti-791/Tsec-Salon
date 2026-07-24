# Hacking World! — Tencent Security Salon Shenzhen Session

> 发布者：云鼎实验室（Tencent Yunding Lab）　|　Published: July 17, 2026　|　Guangdong, China

深圳，2026年7月4日 —— 由腾讯安全主办的安全沙龙第九期深圳站在南山区圆满落幕。本期沙龙以**"Hacking World！"**为主题，打破传统网络安全的边界局限，聚焦生成式 AI 安全、金融系统博弈、碳硅心智博弈、AI Agent 攻防、技术反窃密、近源渗透、具身智能安全、生理与意识安全八大前沿方向，全方位解构数字与物理深度融合时代的新型安全威胁与防御路径。

> Shenzhen, July 4, 2026 — The 9th session of the Tencent Security Salon, hosted by Tencent Security, successfully concluded in Nanshan District. Under the theme "Hacking World!", the salon broke traditional cybersecurity boundaries, focusing on eight cutting-edge domains: Generative AI Security, Financial System Exploitation, Carbon-Silicon Mind Games, AI Agent Offense & Defense, Technical Counter-Espionage, Proximity Penetration, Embodied Intelligence Security, and Physiological & Consciousness Security — deconstructing new threats and defense pathways in the era of deep digital-physical convergence.

本次沙龙共吸引了超过 600 人报名，现场汇聚了 400 余位来自全国各地的网络安全爱好者，其中既有深耕行业多年的安全专家，也有充满好奇心的在校大学生，甚至还有多名热衷技术探索的高中生，现场学术氛围浓厚，跨界思想碰撞激烈。

> The salon attracted over 600 registrations, with more than 400 cybersecurity enthusiasts gathering on-site from across the country — ranging from seasoned security experts to curious university students and even several tech-savvy high schoolers — creating an atmosphere rich with academic rigor and cross-disciplinary exchange.

---

## 开场致辞：重新定义黑客精神 &nbsp;·&nbsp; Opening: Redefining the Hacker Spirit

活动开始，主办方腾讯云鼎实验室攻防负责人李鑫向大家阐释了活动主题 "Hacking World！" 的核心理念，以及办会初衷：

> Li Xin, Head of Offensive & Defensive Security at Tencent Yunding Lab, opened the event by explaining the core philosophy behind "Hacking World!":

- 黑客并非破坏者的标签，而是一种探索世界的思维方式——以好奇心驱动，敢于突破边界，通过拆解、突破系统实现对事物的深度理解，最终指向改进与创造。

  > Hacking is not a label for destroyers, but a way of exploring the world — driven by curiosity, daring to break boundaries, achieving deep understanding through deconstruction and system breakthroughs, ultimately aiming for improvement and creation.

- 真正的技术突破往往发生在学科交叉处。本次沙龙主打跨界融合，希望打破垂直领域壁垒，汇聚金融、硬件、生物、AI 等多元方向的探索者，打造开放的技术交流生态，践行"万物可探，诸法可解"的核心主张。

  > True technological breakthroughs often occur at disciplinary intersections. This salon championed cross-domain fusion, aiming to break vertical silos, bringing together explorers from finance, hardware, biology, AI, and beyond — building an open technical exchange ecosystem guided by the motto "Everything can be explored, all things can be understood."

---

## AI安全：从"幻觉"治理到数据流守卫 &nbsp;·&nbsp; AI Security: From Hallucination Governance to Data Flow Protection

SecureNexusLab 团队 LLM 安全方向负责人陈永锋在《定向幻觉：生成式AI时代的供应链攻击与主动防御》中指出，随着 GEO（生成式引擎优化）技术的黑产化，攻击者可通过投毒 RAG 库、微调劫持等手段制造"定向幻觉"，在不修改模型参数的情况下操控 AI 输出虚假信息。他现场演示了利用 GEO 诱导 AI 生成恶意代码导致 Token 被盗的真实案例，并提出涵盖"知识准入、检索校验、生成干预、全链溯源"的四层防御框架。他强调"AI 是认知的放大镜而非均衡器"，提醒从业者切勿盲目信任 AI 输出。

> Chen Yongfeng, LLM Security Lead at SecureNexusLab, presented "Targeted Hallucination: Supply Chain Attacks and Proactive Defense in the Era of Generative AI." He revealed that as GEO (Generative Engine Optimization) techniques become commoditized in the underground market, attackers can craft "targeted hallucinations" by poisoning RAG databases and hijacking fine-tuning — manipulating AI to output false information without modifying model parameters. He demonstrated a real case where GEO-induced malicious code generation led to token theft, and proposed a four-layer defense framework: Knowledge Gatekeeping, Retrieval Validation, Generation Intervention, and End-to-End Traceability. He warned: "AI is an amplifier of cognition, not an equalizer."

原腾讯安全研究员 haya 和拓竹科技安全专家 12end 分享了题为《从间接注入到数据流劫持：AI Agent 数据流攻与防》的研究。他们通过两个累计获赔超 3 万美元的高危漏洞案例，揭示了 AI Agent 时代隐蔽的数据安全风险。在微软 Copilot 案例中，攻击者仅需在网页植入隐藏指令，即可诱导 AI 泄露用户会话；在开源项目 OpenHands 中，攻击者利用 GitHub Issue 提交恶意代码，成功窃取了开发者的 Git Token。他们提出了一套覆盖网关、端侧、工具调用、RAG 知识库及记忆模块的五层防御体系，并演示了基于轻量级小模型的"意图识别网关"，能有效拦截偏离 Agent 原定功能的敏感操作。

> Former Tencent Security researcher haya and Bambu Lab security expert 12end presented "From Indirect Injection to Data Flow Hijacking: AI Agent Data Flow Attack and Defense." Through two high-severity vulnerability cases with cumulative bounties exceeding $30,000, they exposed the hidden data security risks of the AI Agent era. In the Microsoft Copilot case, attackers only needed to embed hidden instructions in web pages to induce the AI into leaking user sessions. In the OpenHands open-source project, attackers leveraged GitHub Issues to submit malicious code, successfully stealing developer Git Tokens. They proposed a five-layer defense framework covering Gateway, Endpoint, Tool Invocation, RAG Knowledge Base, and Memory Module, and demonstrated a lightweight "intent recognition gateway" capable of effectively blocking sensitive operations that deviate from the Agent's intended functionality.

---

## 跨界博弈：金融暗战与脑机主权 &nbsp;·&nbsp; Cross-Domain Warfare: Financial Intelligence & Brain-Machine Sovereignty

金融安全历来是攻防对抗的高地。华尔街与伦敦顶级对冲基金策略研究员罗炳桥在《金融黑客：二级市场不对称优势下的全域渗透——情报、策略与游资的破壁体系》中，将网络安全中的"对抗工程"思维引入金融交易，系统拆解了获取超额收益的四大支柱：信息优势、认知优势、工程优势与对抗优势。通过"商业航天股盘口诱多"、"白毛女股神出口转内销"等案例，他揭示了利用数据指纹、注意力劫持及叙事操控进行攻击的手法，并指出金融市场充满了针对感官、大模型乃至决策流程的"认知欺骗"。

> Luo Bingqiao, Strategy Researcher at top Wall Street and London hedge funds, presented "Financial Hacking: Full-Spectrum Penetration Under Asymmetric Advantage in Secondary Markets." He introduced the "adversarial engineering" mindset from cybersecurity into financial trading, systematically deconstructing the four pillars of excess returns: Information Advantage, Cognitive Advantage, Engineering Advantage, and Adversarial Advantage. Through cases like "commercial aerospace stock bait-and-switch" and "export-to-domestic narrative laundering," he revealed attack techniques leveraging data fingerprints, attention hijacking, and narrative manipulation, noting that financial markets are rife with "cognitive deception" targeting senses, LLMs, and even decision-making pipelines.

而在人与 AI 的关系层面，独立安全研究员喻峰的《碳硅互搏：从大脑 Hook 到碳基越狱》引发了广泛共鸣。面对 AI 对决策判断的逐步接管，他借用逆向工程思维，探讨了如何通过"意识调试"防止人脑思维"控股权"稀释，守住碳基生物的"系统主权"。

> Independent security researcher Yu Feng's "Carbon vs. Silicon: From Brain Hooking to Carbon-Based Jailbreaking" resonated widely. Facing AI's gradual takeover of decision-making, he applied reverse engineering thinking to explore how "consciousness debugging" can prevent the dilution of human cognitive "controlling stake" and defend the "system sovereignty" of carbon-based life.

李超则进一步在《从人机协同安全到生理防御机制的突破探索》中指出，人类作为碳基开放系统，思维、情绪与行为极易被外界定向干扰，对比硅基 AI 体系，碳基拥有更隐蔽、更广的攻击面，电磁定向干扰、脑机接口等技术早已实现对人体意识、行为的潜在调控，相关风险自二战时期便已有研究落地，在 AI 快速迭代的当下愈发凸显。

> Li Chao further elaborated in "From Human-AI Collaborative Security to Breakthroughs in Physiological Defense Mechanisms," noting that humans as carbon-based open systems have thoughts, emotions, and behaviors that are highly susceptible to targeted external interference. Compared to silicon-based AI systems, carbon-based life presents a more covert and broader attack surface — electromagnetic directed interference and brain-computer interface technologies have long demonstrated potential manipulation of human consciousness and behavior, with related risks researched and deployed since WWII, becoming increasingly prominent amid rapid AI advancement.

他结合自身实践与研究体悟提出，人体与流动意识皆为外在表象，固有身心认知会形成防御枷锁，会固化思维、削弱可塑性，让人体持续暴露在各类外部干扰中。对此，他认为可通过长期身心练习锚定本我、稳住底层主控权，在拥抱 AI 技术的同时，规避情绪与行为被操控的风险，实现人机共生下的自我安全守护。

> Drawing from his own practice and research insights, he proposed that the physical body and fluid consciousness are both external manifestations — inherent mind-body patterns form defensive shackles that rigidify thinking and weaken plasticity, continuously exposing humans to external interference. He argued that through long-term mind-body practice, one can anchor the true self, secure the foundational locus of control, embrace AI technology while avoiding emotional and behavioral manipulation, achieving self-safeguarding in human-machine symbiosis.

---

## 物理世界：近源渗透与具身智能威胁建模 &nbsp;·&nbsp; Physical World: Proximity Penetration & Embodied Intelligence Threat Modeling

当安全战场从线上延伸到线下，威胁变得更加触手可及。RC² TSCM LAB 创始人 Longas 杨叔在《企业安全新趋势：TSCM & Cyber Security》中指出，传统防御正面临"物理入侵 + 网络渗透"的复合威胁。他提出的覆盖"物理-网络-人员"三维度的 360 度防护体系，为企业填补了办公场所与通信链路的物理安全盲区。

> As the security battlefield extends from online to offline, threats become increasingly tangible. Longas Yang, founder of RC² TSCM LAB, in "New Trends in Enterprise Security: TSCM & Cyber Security," pointed out that traditional defenses now face compound threats of "physical intrusion + cyber penetration." His proposed 360-degree protection framework spanning the three dimensions of "Physical-Network-Personnel" fills the physical security blind spots in workplace and communication links for enterprises.

独立安全研究员杨文韬的《从无线电到 DMA：近源渗透实战技术导览》则进一步给大家展示了真实的物理攻击技术。他从无线电信号、USB 外设讲到 DMA 直接内存访问，演示了攻击者如何绕过软件防护获取系统权限，警示企业需重新审视硬件采购与现场运维的风险。

> Independent security researcher Yang Wentao's "From Radio to DMA: A Guided Tour of Proximity Penetration Techniques" further demonstrated real-world physical attack techniques. From radio signals and USB peripherals to DMA (Direct Memory Access), he showed how attackers can bypass software defenses to gain system privileges, warning enterprises to reassess risks in hardware procurement and on-site operations.

作为本次沙龙的最终议题，宇树科技产品安全专家邹佳源带来了《Physical AI Agent：人形机器人平台的具身智能安全威胁建模》。随着人形机器人走进现实，安全问题已关乎人身安全与环境稳定。演讲者构建了包含物理实体、人类与环境的交互系统模型，并对核心决策循环进行了深入的安全建模，为处于萌芽期的 Physical AI Agent 安全指明了研究方向。

> As the salon's closing topic, Zou Jiayuan, Product Security Expert at Unitree Robotics, presented "Physical AI Agent: Embodied Intelligence Security Threat Modeling for Humanoid Robot Platforms." As humanoid robots enter reality, security concerns now directly impact personal safety and environmental stability. The speaker constructed an interactive system model encompassing physical entities, humans, and the environment, and conducted in-depth security modeling of the core decision-making loop, charting research directions for the nascent field of Physical AI Agent security.

---

## 写在最后 &nbsp;·&nbsp; Closing Remarks

持续四个小时的沙龙高潮迭起，不仅有技术的硬核拆解，更有哲学层面的思辨。现场既有高中生向专家请教 AI 伦理的求知若渴，也有老牌白帽在台下频频点头的默契认同。腾讯安全沙龙第九期深圳站不仅是一场技术的盛会，更是一次关于未来安全形态的大讨论。在 AI 与实体经济深度融合的浪潮下，腾讯安全将持续携手安全社区，打破认知边界，共建数字时代的安全底座。

> The four-hour salon was a crescendo of highlights, featuring not only hardcore technical deconstruction but also philosophical discourse. The audience ranged from high schoolers eagerly consulting experts on AI ethics to veteran white-hat hackers nodding in quiet recognition. The 9th Tencent Security Salon in Shenzhen was not merely a technology gathering — it was a grand discussion on the future shape of security. Amid the deepening fusion of AI and the real economy, Tencent Security will continue working hand-in-hand with the security community to break cognitive boundaries and co-build the security foundation for the digital age.

---

## 特别鸣谢 &nbsp;·&nbsp; Special Thanks

腾讯青科实训、深圳河套学院、人民邮电出版社、北京零零信安科技有限公司、美团安全应急响应中心、陌陌安全、顺丰安全、快手安全应急响应中心等合作伙伴对本次活动的大力支持。

> Special thanks to Tencent Youth Science Training Camp, Shenzhen Hetao College, Posts & Telecom Press, Beijing ZeroZeroInfo Technology, Meituan Security Response Center, Momo Security, SF Security, Kuaishou Security Response Center, and other partners for their strong support.

---

## 关于腾讯安全沙龙 &nbsp;·&nbsp; About Tencent Security Salon

腾讯安全沙龙由腾讯云鼎实验室创办，以前沿攻防技术深度研讨为核心，致力于构建开放协作的技术文化。

> The Tencent Security Salon, founded by Tencent Yunding Lab, focuses on in-depth discussions of cutting-edge offensive and defensive technologies, dedicated to building an open and collaborative technical culture.

沙龙主要面向群体包括白帽子、在校生、安全从业人员、学术大咖。为营造轻松、自由的交流氛围，沙龙以"音乐 + 黑客 + 学术"的创新形式展开，自 2024 年创办以来，先后在武汉、西安、成都、长沙、南京、广州、北京、深圳等城市成功举办，获得业界广泛关注和认可。

> The salon primarily serves white-hat hackers, students, security practitioners, and academic experts. To foster a relaxed and open exchange atmosphere, the salon adopts an innovative "Music + Hacking + Academia" format. Since its inception in 2024, it has been successfully held in Wuhan, Xi'an, Chengdu, Changsha, Nanjing, Guangzhou, Beijing, Shenzhen, and other cities, earning widespread industry attention and recognition.

未来，腾讯安全沙龙将持续覆盖全国重点城市，通过搭建产学研深度对话的桥梁，培养具备实战能力的复合型网络安全人才，分享实战经验与创新思路，促进极客文化传承，助力数字安全生态建设。

> Going forward, the Tencent Security Salon will continue to reach key cities nationwide, building bridges for deep dialogue between industry, academia, and research, cultivating interdisciplinary cybersecurity talent with practical capabilities, sharing real-world experience and innovative thinking, promoting hacker culture inheritance, and contributing to the digital security ecosystem.

议题征集：沙龙长期征集云安全、红队、AI安全、域安全、情报、物联网安全等方向的议题。

> `CFP (Call for Papers): The salon continuously accepts submissions on cloud security, red teaming, AI security, domain security, threat intelligence, IoT security, and related topics.`

联系方式：腾讯云鼎实验室攻防负责人 李鑫（微信号：Wx62887799）

> `Contact: Li Xin, Head of Offensive & Defensive Security, Tencent Yunding Lab (WeChat: Wx62887799)`

往期 PPT：[https://share.weiyun.com/rrRLrvVe](https://share.weiyun.com/rrRLrvVe)

---

*原文链接：[微信公众号 - 云鼎实验室](https://mp.weixin.qq.com/s?__biz=MzU3ODAyMjg4OQ==&mid=2247497821&idx=1&sn=0bd41038fea40c3246dec88d378acbc2)*
