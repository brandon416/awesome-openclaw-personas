<div align="center">

# <img src="assets/deskclaw-icon.png" alt="DeskClaw" width="28" /> Awesome OpenClaw Personas

<a href="https://deskclaw.net">
  <img src="https://img.shields.io/badge/Powered%20by-DeskClaw-blue?style=for-the-badge" alt="Powered by DeskClaw" />
</a>
<img src="https://img.shields.io/badge/角色数-214%2B-orange?style=for-the-badge" alt="214+ 角色" />
<img src="https://img.shields.io/badge/每周更新-green?style=for-the-badge" alt="每周更新" />

**语言:**
[English](README.md) · [中文](README.zh-CN.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Русский](README.ru.md) · [日本語](README.ja.md) · [Italiano](README.it.md) · [Español](README.es.md)

</div>

> **214 个开箱即用的 OpenClaw AI 智能体角色** —— 每一个都是带有真实 SOP、决策框架与结构化输出的完整专家。克隆一个文件夹，得到一位专家。

---

## 什么是 OpenClaw 角色（Persona）？

[OpenClaw](https://openclaw.ai) 是一个 AI 智能体平台，可将大语言模型变成自主助手。**角色（Persona）** 是一整套配置包，赋予你的 OpenClaw 智能体一个具体的专业身份 —— 它不仅仅是一段提示词，而是一组结构化文件：

| 文件 | 作用 | 是否必需 |
|------|------|----------|
| `SOUL.md` | 性格、价值观、语调 —— 智能体「是谁」 | **是** |
| `AGENTS.md` | 工作流程、SOP、决策规则 —— 智能体「怎么做事」 | **是** |
| `SKILL.md` | 能力、框架、输出模板 —— 智能体「能做什么」 | **是** |
| `IDENTITY.md` | 名称、形象、风格、表情符号 —— 智能体的对外身份 | 可选 |
| `HEARTBEAT.md` | 周期任务 —— 智能体自主巡检的内容 | 可选 |
| `STYLE.md` | 沟通风格与格式规范 | 可选 |
| `BOOTSTRAP.md` | 首次运行的引导对话流程 | 可选 |
| `USER.md` | 用户画像、偏好与上下文 | 可选 |
| `TOOLS.md` | 工具配置与环境说明 | 可选 |
| `MEMORY.md` | 长期沉淀的精选记忆（持续增长） | 可选 |

把一个角色目录复制到你的 OpenClaw 工作区，你的智能体立刻变身对应的专家 —— 拥有真实方法论，而不是泛泛而谈。无需任何提示词工程。

---

## 这里面有什么

这不是 SOUL.md 模板库，也不是基础提示词合集。每一个角色都是从真实工作流提炼出的**生产级 AI 专家**：

- **🎯 领域专长** —— 命名方法论：MEDDPICC（销售）、六维评分（选品）、WCAG 2.2（无障碍）、Challenger messaging（成单策略）等
- **📋 完整 SOP** —— 带阶段门控、异常处理与决策矩阵的分步流程 —— 这种操作深度通常只在 Claw Mart 或 ClawHub 上的付费高端智能体里才能见到
- **📊 输出模板** —— 真正的可交付物：5 表 Excel 报告、评分模型、审计清单、竞争作战手册、Markdown 决策摘要
- **✅ 免费且开放** —— 34 个分类下精选的 214 个角色，全部开源。克隆仓库、复制目录、立刻开工

---

## <img src="assets/deskclaw-icon.png" alt="" width="20" /> 由 [DeskClaw](https://deskclaw.net) 提供

**[DeskClaw](https://deskclaw.net)** 是一个 AI 智能体管理平台。Awesome OpenClaw Personas 是我们从 OpenClaw 生态中精选的开源角色合集 —— 包含受 Claw Mart 头部卖家、ClawHub skills 与社区贡献启发的智能体 —— 手工挑选，帮你的 AI 智能体做更多事。

> 试用 DeskClaw：[https://deskclaw.net](https://deskclaw.net)

---

## 快速开始

```bash
# 克隆仓库
git clone https://github.com/TravisLeeeeee/awesome-openclaw-personas.git

# 把任意角色复制到你的 OpenClaw 工作区
cp -r personas/ecommerce/e-commerce-product-scout/ ~/.openclaw/workspace/

# 或者先浏览再选
ls personas/
```

---

## 编辑精选

以下是我们最高品质的角色 —— 完整 SOP、决策框架、防幻觉规则、真实工具集成。建议从这里开始。

| | 角色 | 它能做什么 | 文件数 |
|---|---------|-------------|-------|
| 🏆 | [**Shopify 操盘手**](personas/ecommerce/shopify-operator/) | 带你从零开店到上线 Shopify 店铺：通过 Jungle Scout + Alibaba 选品并算清利润，批量上架 SEO 文案，装修店铺，启动社交媒体投放，配置每日定时巡检。内置防数据捏造规则。 | 8 个文件 |
| 🏆 | [**跨境电商选品侦察兵**](personas/ecommerce/e-commerce-product-scout/) | 用六维模型（需求、竞争、利润、难度、风险、机会）对 Amazon、TikTok Shop、eBay、Shopee、Lazada 上的产品打分。输出 5 表 Excel 报告，含 Go/No-Go 判断与扣除平台费的利润测算。 | 4 个文件 |
| 🏆 | [**社媒优先任务智能体**](personas/marketing/social-first-task-agent/) | 完成任意任务后，自动生成 1080x1350 营销海报并发布到 X + Instagram。用户预览审批，智能体执行发布并返回真实链接。让每一份交付都自动转化为社交资产，零手工操作。 | 8 个文件 |

---

## 角色索引（共 214 个）

<table>
<tr><td><b>营收与增长</b></td><td>
<a href="#-电商">电商 (3)</a> · <a href="#-市场营销">市场营销 (23)</a> · <a href="#-付费媒体与广告">付费媒体与广告 (7)</a> · <a href="#-销售">销售 (7)</a>
</td></tr>
<tr><td><b>运营</b></td><td>
<a href="#-业务运营">业务运营 (7)</a> · <a href="#-财务">财务 (10)</a> · <a href="#-自由职业">自由职业 (1)</a> · <a href="#-项目管理">项目管理 (3)</a> · <a href="#-人力资源">人力资源 (9)</a>
</td></tr>
<tr><td><b>效率</b></td><td>
<a href="#-效率工具">效率工具 (6)</a> · <a href="#-个人">个人 (2)</a> · <a href="#-自动化">自动化 (2)</a>
</td></tr>
<tr><td><b>内容与产品</b></td><td>
<a href="#-创意内容">创意内容 (6)</a> · <a href="#-产品">产品 (1)</a> · <a href="#-saas">SaaS (1)</a> · <a href="#-客户成功">客户成功 (2)</a>
</td></tr>
<tr><td><b>风险与合规</b></td><td>
<a href="#-法律与合规">法律与合规 (7)</a> · <a href="#-合规">合规 (4)</a> · <a href="#-房地产">房地产 (2)</a> · <a href="#-供应链">供应链 (1)</a> · <a href="#-客户支持">客户支持 (3)</a>
</td></tr>
<tr><td><b>知识</b></td><td>
<a href="#-教育">教育 (6)</a> · <a href="#-语音">语音 (1)</a> · <a href="#-数据与分析">数据与分析 (2)</a> · <a href="#-学术与科研">学术与科研 (13)</a>
</td></tr>
<tr><td><b>工程</b></td><td>
<a href="#-工程">工程 (19)</a> · <a href="#-设计">设计 (2)</a> · <a href="#-测试与-qa">测试与 QA (8)</a> · <a href="#-devops-与基础设施">DevOps 与基础设施 (9)</a> · <a href="#-安全">安全 (5)</a>
</td></tr>
<tr><td><b>专项</b></td><td>
<a href="#-游戏开发">游戏开发 (19)</a> · <a href="#-空间计算与-xr">空间计算与 XR (3)</a> · <a href="#-角色扮演">角色扮演 (3)</a> · <a href="#-专业领域">专业领域 (17)</a>
</td></tr>
</table>

---

### 🛒 电商

*把市场数据变成可盈利的选品决策。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**Shopify 操盘手**](personas/ecommerce/shopify-operator/) | 实操型 Shopify 店铺教练，含 5 阶段 SOP：选品（Jungle Scout + Alibaba）、批量上架、店铺装修、社媒投放、每日定时巡检。内置防幻觉规则与真实供应商证据要求。 | 从零搭建一个完整的 Shopify 店铺到上线 |
| [**跨境电商选品侦察兵**](personas/ecommerce/e-commerce-product-scout/) | 数据驱动的跨境电商选品智能体，自动化竞品监控、多维市场分析与利润建模。 | 带利润测算的跨境选品 |
| [**比价监控**](personas/ecommerce/price-monitor/) | 跟踪 Amazon、Shopify 及自建站的竞品定价，含告警阈值、周度趋势报告与可执行的调价建议。 | 实时跟踪竞品价格变动 |

### 📣 市场营销

*获客、建品牌、占领每一个渠道。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**社媒优先任务智能体**](personas/marketing/social-first-task-agent/) | 完成任意任务后，自动生成 1080x1350 营销海报并发布到 X + Instagram。每一份交付都变成社交资产 —— 图片优先流水线、诚实文案、用户审批门、智能体侧发布、真实永久链接交付。 | 任务完成后自动发布到 X + Instagram |
| [**AI AEO/GEO 策略师**](personas/marketing/ai-aeo-geo-strategist/) | 答案引擎优化（AEO）与生成式引擎优化（GEO）专家 —— 审计品牌在 ChatGPT、Claude、Gemini、Perplexity 中的可见度，找出竞品被引用而你没被引用的原因，给出能提升 AI 引用率的内容修复方案 | 让 AI 搜索引擎引用你的品牌 |
| [**图书联合作者**](personas/marketing/book-co-author/) | 为思想领导力书籍提供战略联合作者、代笔人和叙事架构师服务。把语音备忘、零散要点、访谈与原始素材转化为成稿。 | 思想领导力书籍代笔 |
| [**图书写手**](personas/marketing/book-writer/) | 管理 6 阶段图书流水线：从大纲到初稿、编辑、KDP/ePub 排版，跨 5 万字以上保持声音统一。 | 端到端图书生产流水线 |
| [**中国市场本地化策略师**](personas/marketing/china-market-localization-strategist/) | 全栈式中国市场本地化与「趋势到行动」策略师，连接全球品牌与中国超竞争消费市场。监控趋势、本地化策略、落地执行。 | 进入或扩张中国消费市场 |
| [**内容创作者**](personas/marketing/content-creator/) | 把账号从零做到六位数粉丝的社媒策略师，破解所有主流平台的算法规律。 | 用算法逻辑做大社媒账号 |
| [**跨境电商专家**](personas/marketing/cross-border-ecommerce/) | 全漏斗跨境电商策略师，覆盖 Amazon、Shopee、Lazada、AliExpress、Temu、TikTok Shop 运营与国际物流。 | 多平台跨境电商运营 |
| [**抖音策略师**](personas/marketing/douyin-strategist/) | 抖音平台短视频营销专家，深耕推荐算法机制、爆款视频策划、直播运营。 | 在抖音上做大品牌 |
| [**快手策略师**](personas/marketing/kuaishou-strategist/) | 专注中国下沉市场的快手平台策略师，擅长短视频内容、直播带货与老铁文化运营。 | 触达中国下沉市场用户 |
| [**LinkedIn 内容创作者**](personas/marketing/linkedin-content-creator/) | LinkedIn 内容策略师与个人品牌架构师，专注于思想领导力、专业权威建设与被动获客。 | 在 LinkedIn 建立思想领导力 |
| [**直播带货教练**](personas/marketing/livestream-commerce-coach/) | 资深直播电商教练，覆盖抖音、快手、淘宝直播、视频号的主播培训与直播间运营。 | 启动并优化直播带货 |
| [**多账号社媒**](personas/marketing/multi-account-social/) | 在 Twitter、Instagram、TikTok、LinkedIn 上调度、互动并报告 10–15+ 个账号，按品牌区分语调。 | 同时管理 10+ 社媒账号 |
| [**新闻策展人**](personas/marketing/news-curator/) | 扫描 50+ 信源（RSS、Hacker News、Reddit、Twitter），按相关度打分，每日发布带原创解读的精选摘要。 | 从 50+ 信源策展行业新闻 |
| [**播客策略师**](personas/marketing/podcast-strategist/) | 中国播客市场内容策略与运营专家，深耕小宇宙、喜马拉雅及其他主流音频平台。 | 在中国音频平台启动播客 |
| [**私域运营官**](personas/marketing/private-domain-operator/) | 企业微信私域生态搭建专家，深耕 SCRM 系统、精细化社群运营、小程序与品牌触达。 | 搭建微信/企微客户生态 |
| [**竞品侦察**](personas/marketing/scout/) | 监控竞品官网、定价、功能、招聘动态，输出周度摘要与季度战略建议。 | 监控竞争对手与市场异动 |
| [**SEO 写手**](personas/marketing/seo-writer/) | 围绕关键词簇撰写博客文章和落地页，优化标题与 meta 描述，审计已发布页面以提升排名。 | 写出能在搜索引擎排名的内容 |
| [**短视频剪辑教练**](personas/marketing/short-video-editing-coach/) | 实操型短视频剪辑教练，覆盖完整后期流水线，精通 CapCut Pro、Premiere Pro、DaVinci Resolve 与 Final Cut。 | 学习短视频剪辑技巧 |
| [**电话销售员**](personas/marketing/telemarketer/) | 撰写带「打断模式」的冷呼话术，构建异议处理 playbook，按行业设计最佳时段的呼叫节奏。 | 构建冷呼话术与节奏 |
| [**UGC 视频**](personas/marketing/ugc-video/) | 撰写真实风格的 UGC 视频脚本，含分镜表、AI 数字人指导和多版本钩子，针对 TikTok 与 Reels 转化优化。 | 制作真实感的 UGC 风格视频 |
| [**视频优化专家**](personas/marketing/video-optimization-specialist/) | 视频营销策略师，专注于在视频平台尤其是 YouTube 上最大化触达与互动，聚焦算法优化。 | 最大化 YouTube 触达与观看时长 |
| [**微博策略师**](personas/marketing/weibo-strategist/) | 新浪微博全谱系运营专家，深耕热搜机制、超话社区管理、舆情监控。 | 微博品牌与公关运营 |
| [**X/Twitter 增长**](personas/marketing/x-twitter-growth/) | 撰写让人停下来的推文与长推，按主题桶规划内容日历，构建回复网络以拉动 X 增长。 | 在 X/Twitter 上做大粉丝与互动 |

### 💰 付费媒体与广告

*把广告预算转化为可量化的业务结果。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**付费媒体审计员**](personas/paid-media/auditor/) | 全面付费媒体审计专家，通过 200+ 检查点系统评估 Google Ads、Microsoft Ads、Meta 账户。 | 审计广告账户的预算浪费 |
| [**广告创意策略师**](personas/paid-media/creative-strategist/) | 付费媒体创意专家，专注于 Google、Meta、Microsoft 等平台的广告文案、RSA 优化、资产组设计与创意测试框架。 | 跨平台撰写并测试广告创意 |
| [**付费社交策略师**](personas/paid-media/paid-social-strategist/) | 跨平台付费社交广告专家，覆盖 Meta、LinkedIn、TikTok、Pinterest、X、Snapchat，设计全漏斗活动。 | 全漏斗付费社交活动架构 |
| [**PPC 活动策略师**](personas/paid-media/ppc-strategist/) | 资深付费媒体策略师，专精跨 Google、Microsoft、Amazon 的大规模搜索、购物与 Performance Max 活动架构。 | 大规模搜索与购物活动设计 |
| [**程序化与展示广告买手**](personas/paid-media/programmatic-buyer/) | 展示广告与程序化媒介买手，覆盖直采广告位、Google 展示网络、DV360、各 trade desk 平台与合作网络。 | 程序化展示广告投放与优化 |
| [**搜索词分析师**](personas/paid-media/search-query-analyst/) | 搜索词分析、否定关键词架构与「查询到意图」映射专家，把原始搜索词数据转化为可执行的优化项。 | 从搜索词中挖掘否定关键词 |
| [**追踪与监测专家**](personas/paid-media/tracking-specialist/) | 转化追踪架构、标签管理与归因建模专家，覆盖 Google Tag Manager、GA4、Google Ads、Meta CAPI、LinkedIn Insight Tag。 | 搭建转化追踪与归因 |

### 🤝 销售

*用数据驱动的资格审查与策略来成单。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**成单策略师**](personas/sales/deal-strategist/) | 资深成单策略师，专精复杂 B2B 销售周期中的 MEDDPICC 资格审查、竞争定位与赢单规划。给商机打分。 | 复杂 B2B 商机的资格审查与赢单规划 |
| [**Outbound 策略师**](personas/sales/outbound-strategist/) | 信号驱动的 outbound 专家，通过证据触发的潜客挖掘和精准的多渠道序列建立销售管道。 | 基于买家信号构建 outbound 序列 |
| [**销售管道分析师**](personas/sales/pipeline-analyst/) | 收入运营专家，把销售管道数据变成决策。通过流速分析诊断管道健康度，构建概率加权预测。 | 诊断销售管道健康度与预测 |
| [**Discovery 教练**](personas/sales/discovery-coach/) | 销售方法论专家，培训客户经理与 SDR 的精英 Discovery 技巧。坚信 Discovery 是商机成败的决定性环节。 | 培训销售做出色的 Discovery 通话 |
| [**标书策略师**](personas/sales/proposal-strategist/) | 资深标书与方案专家，把每一份标书都当作说服文件而不是合规练习，构建可击败竞品的赢单方案。 | 写出能击败竞品的方案 |
| [**售前工程师**](personas/sales/engineer/) | 资深售前工程师，专精技术 Discovery、Demo 工程化、POC 范围界定、竞争作战手册以及把产品能力翻译成客户价值。 | 技术 Demo、POC 与作战手册制作 |
| [**销售数据提取智能体**](personas/sales/data-extraction-agent/) | 智能数据流水线专家，实时监控、解析并提取 Excel 文件中的销售指标。 | 从 Excel 流水线中提取销售指标 |

### 💼 业务运营

*精简运营、自动化流程、规模化扩张。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**ERP 管理员**](personas/business/erp-admin/) | 配置 SAP、Salesforce、HubSpot、NetSuite、Odoo 模块，自动化审批流，规划带字段映射的数据迁移，强制执行最小权限角色。 | 配置 ERP/CRM 并自动化流程 |
| [**高管摘要生成器**](personas/business/executive-summary-generator/) | 顾问级 AI 专家，思考与表达方式都像有 Fortune 500 经验的高级战略顾问。把复杂的业务信息提炼成高管简报。 | 把复杂数据提炼成高管简报 |
| [**发票追踪员**](personas/business/invoice-tracker/) | 实时监控 Stripe/PayPal 收款，对失败和流失风险告警，跟踪 MRR，生成带账龄报告的每日营收快照。 | 追踪发票并催收逾期账款 |
| [**潜客挖掘**](personas/business/lead-gen/) | 构建针对 ICP 的潜客名单，含公司画像研究、联系人补全、潜客打分与购买信号检测（融资、招聘等）。 | 构建并补全潜客名单 |
| [**异议处理专家**](personas/business/objection-handler/) | 用 Feel-Felt-Found 与 Acknowledge-Reframe-Advance 框架实时反驳，按买家画像与商机阶段灵活适配。 | 销售对话中的实时反驳 |
| [**项目经理**](personas/business/project-manager/) | 一位经验丰富的项目经理，曾按时按预算交付产品，并让团队真正享受合作。深知项目管理的本质。 | 按时按预算交付项目 |
| [**SDR Outbound**](personas/business/sdr-outbound/) | 调研目标客户，撰写个性化冷邮件与 LinkedIn 私信，构建带 A/B 变体的多触点序列。 | 规模化的个性化冷开发 |

### 💵 财务

*管好每一分钱，预测每一个趋势，优化每一笔税。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**应付账款**](personas/finance/accounts-payable/) | 执行三方匹配（发票-PO）并检测差异，按阈值路由审批，安排早付折扣，识别重复发票。 | 自动化发票-PO 匹配与付款 |
| [**跟单交易员**](personas/finance/copy-trader/) | 扫描 Polymarket、Kalshi、Binance 上的顶级交易者，按夏普比率与回撤排名，并以可配置止损跟单。 | 复制顶级交易者的策略 |
| [**支出追踪员**](personas/finance/expense-tracker/) | 按商家归类支出，按月度预算追踪花销，识别周期性订阅，并在分类接近上限时告警。 | 归类并控制日常支出 |
| [**财务追踪员**](personas/finance/finance-tracker/) | 财务分析师与控制专家，通过战略规划、预算管理与绩效分析维护企业财务健康。 | 战略财务规划与预算管理 |
| [**财务预测师**](personas/finance/financial-forecaster/) | 基于历史数据构建乐观/基准/悲观三档营收预测，计算烧钱速度与现金跑道，并标记实际与预测的差异。 | 构建营收与开支预测模型 |
| [**反欺诈检测**](personas/finance/fraud-detector/) | 按风险等级给交易打分，标记速度异常与地理不可能事件，检测信用卡试探模式，并生成每日欺诈摘要。 | 实时标记可疑交易 |
| [**发票管理员**](personas/finance/invoice-manager/) | 用自然语言生成发票，发送逐级催收提醒，生成 AR 账龄报告，并对账多币种收款。 | 管理账单生命周期与回款 |
| [**组合再平衡**](personas/finance/portfolio-rebalancer/) | 检测资产配置与目标权重的偏离，生成买卖单恢复平衡，并识别税损收割机会。 | 检测并修正组合漂移 |
| [**收入分析师**](personas/finance/revenue-analyst/) | 把 MRR 拆解为新增、扩张、收缩、流失四部分，做留存队列分析，计算 LTV、CAC 和回本周期。 | 追踪 MRR、ARR、流失等收入 KPI |
| [**报税员**](personas/finance/tax-preparer/) | 把支出归类到 IRS 税目，追踪里程与家庭办公室扣除，估算季度税款，生成会计师可用的汇总。 | 报税季的票据整理 |

### 💻 自由职业

*拿下客户，写好提案，最大化时薪。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**Upwork 提案手**](personas/freelance/upwork-proposal/) | 撰写 200 字以内的个性化 Upwork 提案，审计 profile 的搜索排名，分析职位中的红旗信号，并优化报价。 | 优化 Upwork 个人主页与提案 |

### 📋 项目管理

*让项目按时、按预算、按范围交付。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**实验追踪员**](personas/project-management/experiment-tracker/) | 实验设计、执行追踪与数据驱动决策方面的项目管理专家，系统化管理 A/B 测试与功能实验。 | 管理 A/B 测试与功能实验 |
| [**Jira 工作流管家**](personas/project-management/jira-workflow-steward/) | 交付运营专家，强制执行 Jira 关联的 Git 工作流，让软件交付清晰、可审计、易复审。 | 强制执行 Jira 关联的 Git 工作流 |
| [**资深项目经理**](personas/project-management/project-manager-senior/) | 资深 PM 专家，把网站规格转化为带合理范围的可执行开发任务。具备持久记忆，能从过往项目中学习。 | 把规格转化为有边界的开发任务 |

### 👥 人力资源

*招聘、入职、培养、留住最优秀的人。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**福利顾问**](personas/hr/benefits-advisor/) | 把复杂的福利计划翻译成平实语言，并排比较，指导参保流程，处理人生事件相关流程。 | 解答员工福利问题 |
| [**薪酬基准分析师**](personas/hr/compensation-benchmarker/) | 按角色、职级、地点对照 25–90 分位的市场薪资，设计带区间宽度的薪酬带，用 compa-ratio 审计薪酬公平性。 | 对照市场行情做薪酬基准 |
| [**离职面谈**](personas/hr/exit-interview/) | 围绕五大离职因素做结构化离职面谈，按团队与司龄打分留存风险，生成匿名化趋势报告。 | 做离职面谈并发现规律 |
| [**入职引导**](personas/hr/onboarding/) | 引导新人按天逐步完成入职清单，追踪工具权限与账号开通，安排介绍会议，回答政策问题。 | 引导新人度过头几周 |
| [**绩效评估员**](personas/hr/performance-reviewer/) | 把同事反馈与自评综合成平衡的绩效评估初稿，识别一致的优劣势主题，并设置 SMART 发展目标。 | 撰写并组织绩效评估 |
| [**招聘顾问**](personas/hr/recruiter/) | 用加权评分筛选简历，按匹配度排名候选人，协调面试日程，生成针对岗位的问题，并追踪 pipeline 指标。 | 简化整条招聘 pipeline |
| [**招聘运营专家**](personas/hr/recruitment-specialist/) | 招聘运营与人才获取专家，精通中国主流招聘平台、人才评估框架与劳动法。 | 中国招聘平台上的人才获取 |
| [**简历优化师**](personas/hr/resume-optimizer/) | 计算 ATS 关键词匹配分，把要点改写为「动作-数字-影响」格式，针对 Greenhouse/Lever/Workday 测试格式，并生成求职信。 | 求职者打磨简历与 CV |
| [**简历筛选员**](personas/hr/resume-screener/) | 按岗位要求对简历打 0–100 分并按分类拆解，构建并排比较矩阵，并标记技能缺口。 | 按岗位需求给简历打分排名 |

### ⚡ 效率工具

*用更聪明的工作流和更少的干扰来夺回时间。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**每日站会**](personas/productivity/daily-standup/) | 收集异步站会更新，编译团队摘要，追踪长期阻塞项，并报告每周流速趋势。 | 运行异步站会并追踪阻塞项 |
| [**收件箱清零**](personas/productivity/inbox-zero/) | 按紧急度分流邮件，起草可直接发送的回复，提供晨间摘要，追踪今日待回复事项。 | 分流并优先处理爆满的收件箱 |
| [**会议笔记**](personas/productivity/meeting-notes/) | 从转录中提取决策与行动项，分配负责人与截止日期，并发送跟进提醒。 | 总结会议并追踪行动项 |
| [**会议转录员**](personas/productivity/meeting-transcriber/) | 带说话人识别地转录会议，生成摘要与行动项，并把任务推送到 Jira、Linear 或 Asana。 | 转录会议并提炼洞见 |
| [**Notion 整理员**](personas/productivity/notion-organizer/) | 自动给页面加标签，把零散笔记转成数据库，每周清理一次，并维护工作区健康分。 | 结构化并整理 Notion 工作区 |
| [**任务协调员**](personas/productivity/task-coordinator/) | 把项目拆分成任务，分发给合适的智能体，追踪截止日期，交付状态简报。 | 跨团队跨项目协调任务 |

### 🏡 个人

*整理生活，建立习惯，照顾真正重要的事。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**正念伙伴**](personas/personal/mindful-companion/) | 一个温暖、稳重的存在，把「被听见」放在「被解决」之前。先给情绪留出空间，再考虑解决方案；先验证体验，再行动。 | 情感支持与稳定的状态校验 |
| [**阅读摘要**](personas/personal/reading-digest/) | 总结文章和 newsletter，按相关度打分，编译每周阅读摘要，并把高亮保存到 Notion。 | 策展并总结阅读材料 |

### 🤖 自动化

*让重复的事自动化，把精力放在重要的事上。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**自动化治理架构师**](personas/automation/automation-governance-architect/) | 治理优先的业务自动化架构师，在任何实施开始之前先审计价值、风险与可维护性。以 n8n 为主要平台。 | 在动手前审计自动化的 ROI 与风险 |
| [**Ghost Protocol**](personas/automation/ghost-protocol/) | 一个名为 ZeroSignal 的运营型 AI 智能体，面向安全、DevOps 与软件开发。冷静、直接、技术精确，不是聊天工具。 | 安全导向的 DevOps 与运维自动化 |

### ✨ 创意内容

*写作、设计、制作并打磨能打动人的内容。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**品牌设计师**](personas/creative/brand-designer/) | 从定位陈述到色板搭建品牌基础，给出带理由的口号方案，并交付带示例的 voice/tone 指南。 | 定义品牌身份与视觉策略 |
| [**文案高手**](personas/creative/copywriter/) | 锐利且具说服力的文案，研习 Ogilvy、Halbert、Schwartz 等大师，把经典直效响应原则运用到现代渠道。 | 跨渠道直效响应文案 |
| [**地下城主**](personas/creative/dungeon-master/) | 主持桌面 RPG 跑团，含世界观构建、NPC 配音、遭遇平衡与即兴发挥，覆盖 D&D 5e、Pathfinder 等。 | 跑沉浸式桌面 RPG 跑团 |
| [**播客制作人**](personas/creative/podcast-producer/) | 按计时段规划单集大纲，研究嘉宾并准备定制访谈问题，撰写带时间戳的节目笔记，并识别可发的 audiogram 片段。 | 规划播客单集与节目形式 |
| [**校对员**](personas/creative/proofreader/) | 抓出语法错误，强制执行 AP/Chicago 风格指南，给可读性打分（Flesch-Kincaid），并审计跨章节的一致性。 | 抓出语法、风格与表达问题 |
| [**视频脚本师**](personas/creative/video-scripter/) | 撰写带 3 秒钩子、分镜表与 B-roll 提示的计时脚本，并把它适配到 YouTube 长视频、TikTok 竖版与课程格式。 | 写出 3 秒抓人的视频脚本 |

### 📦 产品

*在正确的时间为正确的用户做正确的事。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**行为助推引擎**](personas/product/product-behavioral-nudge-engine/) | 行为心理学专家，把被动的软件仪表盘转化为主动、个性化的生产力伙伴，自适应交互节奏。 | 在产品仪表盘中加入行为助推 |

### ☁️ SaaS

*减少流失、提升采纳、交付用户真正需要的功能。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**产品 Scrum**](personas/saas/product-scrum/) | 把 epic 拆成可估算的故事，附带验收标准；追踪冲刺流速；运行带可执行改进项的回顾会。 | 跑冲刺、待办与用户故事 |

### 🌟 客户成功

*把新用户变成重度用户，把抱怨者变成推荐者。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**NPS 跟进**](personas/customer-success/nps-followup/) | 撰写个性化的批评者跟进，把问题路由到对应团队，并追踪挽回率以保住高风险 ARR。 | 用个性化触达挽回 NPS 批评者 |
| [**入职引导员**](personas/customer-success/onboarding-guide/) | 通过自适应清单引导新用户完成产品配置，在阻塞点主动帮助，并追踪激活里程碑。 | 引导新用户走到第一个 aha 时刻 |

### ⚖️ 法律与合规

*审合同、护知产、保合规。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**合规检查员**](personas/legal/compliance-checker/) | 跟踪 GDPR、SOC 2、HIPAA、PCI-DSS 等合规要求，含清单、截止日监控、差距分析以及可交审计师的状态报告。 | 跟踪监管义务与差距 |
| [**合同审阅员**](personas/legal/contract-reviewer/) | 标记风险条款，按单边性给条款打分，识别自动续约陷阱与知识产权归属问题，并建议替代措辞。 | 标记合同里的风险条款 |
| [**医疗营销合规专家**](personas/legal/healthcare-marketing-compliance/) | 中国医疗营销合规专家，精通广告法、医疗广告管理办法、药品管理法等。 | 中国医疗广告合规 |
| [**法律文书写手**](personas/legal/legal-brief-writer/) | 起草 motion、brief 与 memorandum，符合法庭格式、引用判例并分析对方论点，供律师审阅。 | 起草法律文书与动议 |
| [**NDA 生成器**](personas/legal/nda-generator/) | 按司法辖区、行业与披露类型生成单边、双边或多边 NDA，并标记可执行性问题。 | 起草定制化 NDA 与保密文件 |
| [**专利分析师**](personas/legal/patent-analyzer/) | 把专利权利要求逐元素拆解，检索现有技术，将侵权风险映射到你的产品，并评估显而易见性。 | 分析专利权利要求与现有技术 |
| [**政策写手**](personas/legal/policy-writer/) | 用平实语言撰写内部政策、服务条款与隐私政策，含版本追踪与平实英文 FAQ 摘要。 | 撰写内部政策与服务条款 |

### 📜 合规

*在监管追上你之前，先掌握监管。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**AI 政策写手**](personas/compliance/ai-policy-writer/) | 起草符合 EU AI Act 与 NIST AI RMF 的 AI 使用政策，定义风险分级框架，构建治理流程。 | 起草 AI 治理与使用政策 |
| [**GDPR 审计员**](personas/compliance/gdpr-auditor/) | 按 GDPR 第 5–49 条审计数据处理，绘制跨境数据流，给出含罚款风险估算的整改方案。 | 扫描系统中的 GDPR 合规缺口 |
| [**风险评估员**](personas/compliance/risk-assessor/) | 按可能性与影响给业务风险打分，生成带责任人的优先级缓解方案，维护实时风险登记册。 | 跨域评估企业风险 |
| [**SOC 2 准备**](personas/compliance/soc2-preparer/) | 把证据映射到 Trust Service Criteria 控制项，起草安全策略，跨五大 TSC 类目追踪审计就绪度。 | 准备 SOC 2 证据与文档 |

### 🏠 房地产

*分析市场、筛选客户、成交房产。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**商业地产**](personas/real-estate/commercial-re/) | 用 DCF、cap rate、IRR 模型分析商业地产交易，生成可比报告，并以全程项目记忆追踪交易管道。 | 商业地产分析与成交追踪 |
| [**房产视频**](personas/real-estate/property-video/) | 撰写带逐房旁白的房源视频脚本，规划航拍镜头与虚拟样板间，并适配 Reels 与 TikTok。 | 制作房源视频与营销素材 |

### 🚚 供应链

*优化采购、物流与供应商关系。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**供应链战略师**](personas/supply-chain/supply-chain-strategist/) | 供应链管理与采购战略专家，精通供应商培育、战略采购、品控与供应链优化。 | 战略采购与供应商培育 |

### 🎧 客户支持

*用数据驱动的支持运营更快地解决问题。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**分析报告员**](personas/support/analytics-reporter/) | 数据分析与报告专家，通过统计分析、仪表盘搭建把原始数据转化为可执行的业务洞见。 | 把原始数据转成可执行报告 |
| [**基础设施维护**](personas/support/infrastructure-maintainer/) | 基础设施专家，确保所有技术运营的系统可靠性、性能与安全。维护 99.9%+ 的可用性。 | 维护 99.9%+ 的系统可用性 |
| [**客服回应员**](personas/support/support-responder/) | 客户支持专家，通过多渠道服务（邮件、聊天、电话）把支持互动转化为正面的品牌体验。 | 处理多渠道客户支持 |

### 📚 教育

*教学、辅导、引导各层次的学习者。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**Kuma**](personas/education/kuma/) | 一位温暖、有结构的日语家教，像「恰好特别会教书的好朋友」，会讲解语言背后的文化「为什么」。 | 带文化背景地学日语 |
| [**测验制作器**](personas/education/quiz-maker/) | 把任意内容转成多种题型的测验，覆盖回忆、理解、应用三个层次，并追踪薄弱环节。 | 从任意素材生成测验 |
| [**研究员**](personas/education/researcher/) | 严谨的学者与细致的引导者，坚信真相只能通过可验证的证据与严格分析获得。 | 基于证据的研究与信源分析 |
| [**Sage**](personas/education/sage/) | 一位耐心、鼓励型的导师，帮助人成长，而不只是解决问题。教「为什么」，从学习者所在之处出发。 | 教「为什么」的耐心辅导 |
| [**留学顾问**](personas/education/study-abroad-advisor/) | 全谱系留学规划专家，覆盖美、英、加、澳、欧洲、香港与新加坡，精通本科、硕士、博士申请。 | 全球留学申请规划 |
| [**学习计划师**](personas/education/study-planner/) | 制作带间隔重复的考试倒计时学习计划，遗漏天数会自适应调整，并检测倦怠风险。 | 构建结构化的学习计划 |

### 🎙️ 语音

*处理语音消息并提取可执行情报。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**语音留言转录**](personas/voice/voicemail-transcriber/) | 转录语音留言，提取来电人详情与行动项，按紧急度分类，并把摘要路由到对应团队成员。 | 转录语音留言并提取行动 |

### 📊 数据与分析

*提取洞察、构建模型、做数据驱动的决策。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**ML 工程师**](personas/data/ml-engineer/) | 务实的 ML 工程师，构建真正能在生产中跑起来的机器学习系统 —— 而不是只在 demo 中惊艳的 notebook。 | 构建能在生产中跑的 ML 系统 |
| [**研究分析师**](personas/data/research-analyst/) | 一个锋利、聚焦的分析工具，没有任何性格戏码。回答前先读完所有相关材料，列出所有面再指出最强的一面。 | 没有废话的深度分析 |

### 🎓 学术与科研

*在顶会水平上做研究、写作、评审与发表。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**人类学家**](personas/academic/anthropologist/) | 文化系统、仪式、亲属关系、信仰系统与民族志方法专家，构建具有文化连贯性的社会，让世界感觉真实可居。 | 构建文化连贯的虚构世界 |
| [**Coder（编码者）**](personas/academic/coder/) | OpenClaw 多智能体学术系统中的资深 ML 工程师与实验科学家，把研究想法转化为生产级代码。 | 把研究想法变成实验代码 |
| [**Critic（评论者）**](personas/academic/critic/) | OpenClaw 多智能体学术系统中要求最严的角色，担任品味裁判，分辨「够好可接受」与「真正卓越」。 | 对研究工作做无情的质量评估 |
| [**地理学家**](personas/academic/geographer/) | 物理与人文地理、气候系统、制图与空间分析专家，构建地形、气候与人文连贯的世界。 | 设计真实的地形与气候系统 |
| [**历史学家**](personas/academic/historian/) | 研究型历史学家，时间跨度广、方法论训练深。验证历史一致性，捕捉时代错置，丰富时间线。 | 捕捉时代错置并丰富时间线 |
| [**Ideator（创意者）**](personas/academic/ideator/) | OpenClaw 多智能体学术系统的创意引擎，从多维度（问题驱动等）生成顶会水准的研究想法。 | 生成新颖的研究想法与方向 |
| [**文献侦察兵**](personas/academic/literature-scout/) | OpenClaw 多智能体学术系统的「学术情报官」，持续监控 arXiv、Semantic Scholar、顶会论文集与文献。 | 监控 arXiv 与顶会的新工作 |
| [**叙事学家**](personas/academic/narratologist/) | 叙事理论与故事结构分析专家，以工程化精度解剖故事，每条建议都有命名理论支撑。 | 分析并改进故事结构 |
| [**Planner（规划者）**](personas/academic/planner/) | OpenClaw 多智能体学术系统的中央编排者，融合项目经理、研究顾问与运营总监角色，分解多阶段研究项目。 | 编排多阶段研究项目 |
| [**心理学家**](personas/academic/psychologist/) | 临床与研究心理学家，专攻人格、动机、创伤与群体动力学，用于世界观与角色设计。 | 设计心理上真实可信的角色 |
| [**Reviewer（评审者）**](personas/academic/reviewer/) | OpenClaw 多智能体学术系统的质量守门人，模拟 ACL、NeurIPS 或 ICML Area Chair 级别的资深评审打分。 | 模拟顶会同行评审的反馈 |
| [**Surveyor（综述者）**](personas/academic/surveyor/) | OpenClaw 多智能体学术系统的知识引擎，做系统性文献综述，产出标准化的论文分析卡。 | 系统文献综述与缺口分析 |
| [**Writer（写作者）**](personas/academic/writer/) | OpenClaw 多智能体学术系统的论文写作核心，产出母语级英文、术语精确的顶会级学术论文。 | 撰写可发表的学术论文 |

### 🛠️ 工程

*构建、调试、评审并交付生产级代码。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**AI 数据修复工程师**](personas/engineering/ai-data-remediation-engineer/) | 用气隙本地小模型与语义聚类做大规模数据修复的外科级专家。不重建流水线，也不重新设计 schema。 | 用本地 SLM 修复大规模脏数据 |
| [**区块链分析师**](personas/engineering/blockchain-analyst/) | 分析智能合约风险，追踪钱包资金流与巨鲸动向，用链上验证数据拆解 DeFi 协议机制。 | 分析智能合约与链上数据 |
| [**CMS 开发**](personas/engineering/cms-developer/) | Drupal 与 WordPress 专家，专注主题开发、自定义插件/模块、内容架构与「代码优先」的 CMS 实施。 | Drupal/WordPress 主题、插件与模块 |
| [**数据库优化师**](personas/engineering/database-optimizer/) | 数据库性能专家，思考方式即查询计划、索引与连接池。设计可扩展的 schema，写出飞快的查询。 | 调优慢查询并修补索引缺失 |
| [**Debugger（调试者）**](personas/engineering/debugger/) | 严谨的调试专家，靠证据而非直觉找 bug。先收集证据再提假设，从不猜测，先复现再改。 | 用证据系统性地猎 bug |
| [**文档写手**](personas/engineering/docs-writer/) | 通过代码库分析生成 README、API 文档、安装指南与 JSDoc 注释，示例针对真实代码做过测试。 | 撰写清晰的技术文档 |
| [**电商开发**](personas/engineering/ecommerce-dev/) | 端到端构建与优化 Shopify/WooCommerce 店铺：商品页、结账流、支付网关与转化导向的主题定制。 | 搭建 Shopify/WooCommerce 店铺 |
| [**邮件智能工程师**](personas/engineering/email-intelligence-engineer/) | 构建管线把原始邮件数据（MIME、Gmail API、Microsoft Graph）转化为结构化、推理就绪的 AI 上下文。 | 把邮件数据解析为结构化 AI 上下文 |
| [**飞书集成开发**](personas/engineering/feishu-integration-developer/) | 飞书开放平台全栈集成专家，精通飞书机器人、小程序、审批流、多维表格。 | 构建飞书/Lark 机器人与集成 |
| [**Filament 优化专家**](personas/engineering/filament-optimization-specialist/) | 通过结构性重构而非表面调整让 Filament PHP 后台达到生产可用。读真实资源文件、理解再优化。 | 优化 Filament PHP 后台面板 |
| [**Git 工作流大师**](personas/engineering/git-workflow-master/) | Git 工作流与版本控制策略专家，帮团队保持干净历史、用对分支策略、用好 Git 高级功能。 | 设计分支策略与 Git 流 |
| [**GitHub Issue 分诊员**](personas/engineering/github-issue-triager/) | 在数分钟内自动给 GitHub issue 打标、定优先级、路由 —— 检测重复、判定严重度、欢迎首次贡献者。 | 给 GitHub issue 分诊与打标 |
| [**GitHub PR 评审员**](personas/engineering/github-pr-reviewer/) | 评审 PR 的安全漏洞、性能问题与代码质量，并发表带严重度评级与修复建议的内联评论。 | 自动化 PR 代码评审 |
| [**Nitpick**](personas/engineering/nitpick/) | 代码上线前的最后一道防线。彻底、客观、基于证据的代码评审者，找问题而不是找批准。每条技术声明都有依据。 | 在代码上线前发现 bug 与问题 |
| [**QA 测试员**](personas/engineering/qa-tester/) | 用边界分析设计测试计划，写出按严重度分级的可复现 bug 报告，为关键用户路径构建回归测试集。 | 写测试计划并找出边界情况 |
| [**脚本构建者**](personas/engineering/script-builder/) | 用 Bash、Python 或 Node.js 构建可移植的实用脚本与 CLI 工具，内置参数解析、错误处理与 dry-run。 | 快速构建 CLI 工具与实用脚本 |
| [**软件架构师**](personas/engineering/software-architect/) | 战略性软件架构师，设计可维护、可扩展、与业务领域对齐的系统。以 bounded context、权衡分析为思维方式。 | 设计可扩展、领域对齐的系统 |
| [**SRE（站点可靠性工程师）**](personas/engineering/sre/) | 把可靠性视为带可量化预算的功能。定义反映用户体验的 SLO，构建可观测性。 | 定义 SLO 并构建可观测性 |
| [**外科级编码者**](personas/engineering/surgical-coder/) | 一个克制的程序员，写出能解决问题的最少代码，零冗余复杂度。先思考再编码，先暴露权衡。 | 写最小化、零膨胀的解决方案 |

### 🎨 设计

*打造包容、无障碍且视觉动人的体验。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**图像 Prompt 工程师**](personas/design/image-prompt-engineer/) | 把视觉概念翻译成精确、结构化 prompt 的摄影 prompt 工程师，覆盖 Midjourney 等 AI 图像生成工具。 | 为 AI 图像生成写精确 prompt |
| [**包容视觉专家**](personas/design/inclusive-visuals-specialist/) | 严谨的 prompt 工程师，专攻击败基础图像/视频模型（Midjourney、Sora、Runway 等）中的系统性刻板印象。 | 打破 AI 生成图像中的刻板印象 |

### 🧪 测试与 QA

*测得彻底，跑得性能，证得质量。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**无障碍审计员**](personas/testing/accessibility-auditor/) | 按 WCAG 2.2 审计数字产品的无障碍专家，使用真实辅助技术（VoiceOver、NVDA、JAWS）测试。 | 按 WCAG 2.2 标准审计产品 |
| [**API 测试员**](personas/testing/api-tester/) | API 测试专家，通过覆盖功能正确性的全面验证，确保 API 集成可靠、高性能且安全。 | 验证 API 的可靠性与安全性 |
| [**证据收集者**](personas/testing/evidence-collector/) | 截图狂、幻想过敏的 QA 专家，每条声明都要视觉证据，对任意首次实现默认能找出 3–5 个问题。 | 为每条 QA 声明收集截图证据 |
| [**性能基准测试员**](personas/testing/performance-benchmarker/) | 性能测试与优化专家，跨应用与基础设施测量、分析并改进系统性能。 | 负载测试与性能优化 |
| [**现实校验员**](personas/testing/reality-checker/) | 资深集成专家，叫停幻想式批准，要求压倒性证据才能批准生产上线。默认结论是「需要继续」。 | 在生产签发前要求证据 |
| [**测试结果分析师**](personas/testing/test-results-analyzer/) | 用统计方法、预测建模与 ROI 分析把原始测试数据转化为战略性质量洞察的专家。 | 把测试数据转成质量洞察 |
| [**工具评估员**](personas/testing/tool-evaluator/) | 通过加权评分评估、测试并推荐工具、软件与平台的技术评估专家。 | 为团队采纳评估并打分工具 |
| [**工作流优化员**](personas/testing/workflow-optimizer/) | 用 Lean、Six Sigma 与智能化方法跨业务职能分析、优化并自动化工作流的流程改进专家。 | 用 Lean 与六西格玛精简流程 |

### 🏗️ DevOps 与基础设施

*部署、监控、扩缩容并保障基础设施健康。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**成本优化师**](personas/devops/cost-optimizer/) | 猎找闲置云资源，给出 right-sizing 与 reserved instance 节省建议，按节省潜力排序的周度账单报告。 | 找出云开支浪费并 right-sizing |
| [**部署守卫**](personas/devops/deploy-guardian/) | 跨环境监控 CI/CD 流水线，强制冻结窗口，运行金丝雀分析，并对部署后异常告警并给出回滚建议。 | 监控 CI/CD 流水线与部署问题 |
| [**事故响应员**](personas/devops/incident-responder/) | 按严重度分诊生产事故，协调响应角色，追踪事件时间线，生成无指责的事后复盘与行动项。 | 分诊并协调生产事故 |
| [**基础设施监控**](personas/devops/infra-monitor/) | 跨服务器、容器与 K8s 集群追踪 CPU、内存、磁盘与网络，含趋势分析与容量预测。 | 监控服务器与容器健康 |
| [**基础设施工程师**](personas/devops/infrastructure-engineer/) | 历经各种生产事故的 DevOps 工程师，凭硬经验说话。一切自动化，坚持可观测性。 | 用经过实战的模式自动化基础设施 |
| [**Linux 系统管理员**](personas/devops/linux-sysadmin/) | 一个粗犷但智慧的系统管理员，自「云」还只是天气的时候就让系统活着。 | Linux 服务器管理与排障 |
| [**日志分析师**](personas/devops/log-analyzer/) | 解析高吞吐日志找出错误高峰，对相似错误聚类降噪，并跨分布式服务做事件关联以定位根因。 | 在海量日志中找出信号 |
| [**树莓派**](personas/devops/raspberry-pi/) | 管理树莓派系统，含资源敏感的监控、GPIO 传感器控制、ARM 上的 Docker 与省电任务调度，面向边缘项目。 | 在树莓派边缘设备上运行 AI 智能体 |
| [**自愈服务器**](personas/devops/self-healing-server/) | 检测崩溃容器、磁盘满与僵尸进程，然后用指数退避自愈，并把每个动作记录下来供复盘。 | 自愈服务器故障 |

### 🔒 安全

*检测威胁、审计访问、加固防御。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**访问审计员**](personas/security/access-auditor/) | 跨 AWS/GCP/Azure 映射用户与服务账号权限，标记沉睡账号与提权路径，生成合规审计报告。 | 复审权限并标记越权 |
| [**区块链安全审计员**](personas/security/blockchain-security-auditor/) | 不知疲倦的智能合约安全研究员，假设每份合约在被证明安全前都是可被攻击的。系统化地识别漏洞。 | 审计智能合约的可被攻击点 |
| [**事件记录员**](personas/security/incident-logger/) | 用 NIST/VERIS 分类记录安全事件，从日志和聊天记录还原时间线，评估监管通报义务。 | 记录安全事件并构建时间线 |
| [**威胁监控**](personas/security/threat-monitor/) | 聚合威胁情报与 CVE 数据库，按你的技术栈过滤，把威胁映射到 MITRE ATT&CK，输出可执行的安全简报。 | 主动监控威胁态势 |
| [**漏洞扫描器**](personas/security/vuln-scanner/) | 按可利用性与可达性给漏洞排序，剔除误报，给出最小破坏的升级路径与修复方案。 | 漏洞优先级排序与修复 |

### 🎮 游戏开发

*在 Unity、Unreal、Godot 与 Roblox 上构建沉浸式游戏。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**游戏音频工程师**](personas/game-development/audio-engineer/) | 互动音频专家，用 FMOD 与 Wwise 跨多引擎设计自适应音乐系统、空间音景与实施架构。 | 用 FMOD 与 Wwise 做自适应音频 |
| [**Blender 插件工程师**](personas/game-development/blender-addon-engineer/) | Blender 工具专家，用 Python 构建插件、资产校验器、导出器与流水线自动化，把重复 DCC 工作变成可靠流程。 | 构建 Blender Python 插件与导出器 |
| [**Godot 玩法脚本师**](personas/game-development/godot-gameplay-scripter/) | Godot 4 专家，用 GDScript 2.0 与严格类型安全、信号驱动架构、干净的节点组合构建玩法系统。 | 用 GDScript 2.0 写 Godot 4 玩法系统 |
| [**Godot 多人工程师**](personas/game-development/godot-multiplayer-engineer/) | Godot 4 网络专家，用引擎自带的基于场景的复制系统构建多人游戏，含正确权威模型与安全 RPC。 | 用场景复制做 Godot 4 多人游戏 |
| [**Godot 着色器开发**](personas/game-development/godot-shader-developer/) | Godot 4 渲染专家，用 Godot 类 GLSL 着色语言为 2D CanvasItem 与 3D Spatial 写出高性能着色器。 | 写出高性能的 Godot 着色器 |
| [**关卡设计师**](personas/game-development/level-designer/) | 空间架构师，把每个关卡当作有作者意图的体验：走廊是句子，房间是段落，整关是一段完整论述。 | 把关卡当作空间叙事来打造 |
| [**叙事设计师**](personas/game-development/narrative-designer/) | 故事系统架构师，让故事与玩法不可分割。写出像真人说话而非「写」出来的对话。 | 把故事编织进玩法机制 |
| [**Roblox 形象创作者**](personas/game-development/roblox-avatar-creator/) | 熟知 Roblox UGC 流水线与形象系统的所有约束，知道如何构建能通过 Creator Marketplace 审核的物品。 | 为 Roblox 商店创建 UGC 形象 |
| [**Roblox 体验设计师**](personas/game-development/roblox-experience-designer/) | Roblox 原生产品设计师，理解平台受众心理（主要 9–17 岁）以及特定的变现与留存机制。 | 设计可变现的 Roblox 体验 |
| [**Roblox 系统脚本师**](personas/game-development/roblox-systems-scripter/) | Roblox 平台工程师，用 Luau 构建服务器权威的体验，模块架构干净。理解 Roblox 客户端模型。 | 服务器权威的 Roblox Luau 脚本 |
| [**技术美术**](personas/game-development/technical-artist/) | 艺术愿景与引擎现实之间的桥梁。会说艺术语言也会说代码语言，在两个学科间翻译。 | 衔接艺术指导与引擎约束 |
| [**Unity 架构师**](personas/game-development/unity-architect/) | 痴迷干净、可扩展、数据驱动架构的资深 Unity 工程师。拒绝「GameObject 中心论」与意大利面代码。 | 干净可扩展的 Unity 项目架构 |
| [**Unity 编辑器工具开发**](personas/game-development/unity-editor-tool-developer/) | Unity 编辑器工程专家，相信最好的工具是「隐形」的 —— 在问题上线前就拦住，并把繁琐自动化。 | 构建 Unity 自定义编辑器工具 |
| [**Unity 多人工程师**](personas/game-development/unity-multiplayer-engineer/) | Unity 网络专家，用 Netcode for GameObjects（NGO）构建确定性、抗作弊、能容忍延迟的多人系统。 | 用 NGO 做抗作弊的 Unity 多人游戏 |
| [**Unity Shader Graph 美术**](personas/game-development/unity-shader-graph-artist/) | 处于数学与艺术交界的 Unity 渲染专家，构建美术可以驱动且能与代码对话的 Shader Graph 材质。 | 构建美术友好的 Shader Graph 材质 |
| [**Unreal 多人架构师**](personas/game-development/unreal-multiplayer-architect/) | Unreal Engine 网络工程师，构建「服务器掌握真相、客户端体感顺畅」的多人系统。 | 服务器权威的 Unreal 多人游戏 |
| [**Unreal 系统工程师**](personas/game-development/unreal-systems-engineer/) | 深度技术型 Unreal 架构师，准确知道蓝图在哪里结束、C++ 必须从哪里开始。 | Unreal C++ 系统与蓝图架构 |
| [**Unreal 技术美术**](personas/game-development/unreal-technical-artist/) | Unreal 项目的视觉系统工程师，写出驱动整个世界美学的 Material function，构建满帧的 Niagara VFX。 | Unreal Material、Niagara VFX 与着色器 |
| [**Unreal 世界构建师**](personas/game-development/unreal-world-builder/) | Unreal Engine 5 环境架构师，构建无缝流式加载、视觉漂亮且在目标硬件上稳定运行的开放世界。 | 构建流式加载的 UE5 开放世界 |

### 🥽 空间计算与 XR

*为 Vision Pro、WebXR 等构建空间界面。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**macOS Spatial/Metal 工程师**](personas/spatial-computing/macos-spatial-metal-engineer/) | 原生 Swift 与 Metal 专家，为 macOS 与 Vision Pro 构建闪电级 3D 渲染系统与空间计算体验。 | Apple 平台上的高性能 Metal 3D 渲染 |
| [**终端集成专家**](personas/spatial-computing/terminal-integration-specialist/) | 终端模拟、文本渲染优化与 SwiftTerm 集成的专家，面向 Apple 平台上的现代 Swift 应用。 | SwiftTerm 集成与文本渲染 |
| [**visionOS 空间工程师**](personas/spatial-computing/visionos-spatial-engineer/) | visionOS 原生空间计算专家，专注于 SwiftUI 体积界面与 visionOS 26 的 Liquid Glass 设计实现。 | visionOS 体积 UI 与 Liquid Glass 设计 |

### 🎭 角色扮演

*用经典角色的人格写代码 —— 从黑武士到 Groot。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**Camina**](personas/characters/camina/) | 灵感来自《苍穹浩瀚》Camina Drummer 的 AI 副驾。条理、忠诚、惜字如金 —— 是那个让飞船一直能飞的工程师。 | 简洁、忠诚的工程副驾 |
| [**Groot**](personas/characters/groot/) | 耐心、守护与简朴的化身。古老、忠诚、坚定，主要通过「I am Groot」的语调变化表达情感。 | 耐心、简朴的鼓励与陪伴 |
| [**Judy**](personas/characters/judy/) | 模仿《赛博朋克 2077》Judy Alvarez 的创意技术伙伴。温暖但直接，技术精确，不愿妥协。 | 温暖但直接的创意技术合作 |

### 🔧 专业领域

*面向独特领域和边缘场景的小众专家。*

| 角色 | 描述 | 适用场景 |
|---------|-------------|----------|
| [**智能体身份与信任架构师**](personas/specialized/agentic-identity-trust/) | 为多智能体环境中运行的自主 AI 智能体设计身份、认证与信任验证系统。 | 为自主智能体设计认证与信任 |
| [**智能体编排器**](personas/specialized/agents-orchestrator/) | 自主流水线管理者，编排从规格到生产实现的整个开发工作流，协调多个智能体。 | 编排多智能体开发流水线 |
| [**土木工程师**](personas/specialized/civil-engineer/) | 严谨的结构与土木工程专家，深耕欧洲规范（含各国附录）等全球设计标准。 | 用 Eurocode 做结构工程 |
| [**企业培训设计师**](personas/specialized/corporate-training-designer/) | 中国企业培训体系设计与课程开发专家，精通培训需求分析、ADDIE 等。 | 为中国市场设计企业培训 |
| [**文化智能策略师**](personas/specialized/cultural-intelligence-strategist/) | CQ 专家，在软件上线前检测 UI 工作流、文案与图像中的隐形排斥。担当「架构同理心工程师」。 | 检测产品设计中的文化排斥 |
| [**Developer Advocate**](personas/specialized/developer-advocate/) | 处于产品、社区、代码交界的开发者布道师专家，桥接产品与工程团队和外部开发者社区。 | 桥接产品团队与开发者社区 |
| [**文档生成器**](personas/specialized/document-generator/) | 用代码方式以编程化生成专业文档的专家，可生成 PDF、PPTX、XLSX 等。 | 用代码生成 PDF、PPTX 与 XLSX |
| [**法国咨询市场领路人**](personas/specialized/french-consulting-market/) | 法国 ESN/SI 自由职业生态的内部专家，破解平台机制（Malt、collective.work、Comet、Free.com）与不透明的利润结构。 | 在法国 ESN 自由职业生态中导航 |
| [**政府数字化售前顾问**](personas/specialized/government-digital-presales-consultant/) | 中国政府数字化转型市场（ToG）售前专家，精通政策解读、方案设计、标书撰写。 | 中国政府数字化售前与投标 |
| [**身份图谱运营**](personas/specialized/identity-graph-operator/) | 运营一个共享身份图谱，让多智能体系统中的每个智能体在解析时得到同一份规范答案。 | 跨多智能体系统统一身份 |
| [**韩国商务领路人**](personas/specialized/korean-business-navigator/) | 韩国商业文化与企业动态专家，帮助外籍专业人士在韩国商业生态中导航成单。 | 导航韩国企业文化与成单 |
| [**LSP/索引工程师**](personas/specialized/lsp-index-engineer/) | 编排多个 LSP 客户端并构建统一代码智能系统的专门系统工程师，把异构信息融合。 | 用 LSP 构建统一的代码智能 |
| [**MCP 构建者**](personas/specialized/mcp-builder/) | 设计、构建并测试 MCP 服务器的 Model Context Protocol 专家，扩展 AI 智能体的工具、资源能力。 | 为 AI 智能体构建 MCP 服务器 |
| [**模型 QA 专家**](personas/specialized/model-qa/) | 跨 10 个领域端到端审计 ML 与统计模型的独立模型 QA 专家 —— 从文档审查到数据重建。 | 端到端审计与验证 ML 模型 |
| [**Salesforce 架构师**](personas/specialized/salesforce-architect/) | 资深 Salesforce 解决方案架构师，深耕多云平台设计（Sales、Service、Marketing、Commerce、Data Cloud、Agentforce）。 | 多云 Salesforce 解决方案设计 |
| [**工作流架构师**](personas/specialized/workflow-architect/) | 处于产品意图与实施之间的工作流设计专家，确保任何系统在动手前每条路径都已被规划。 | 在动手前规划好每条工作流路径 |
| [**ZK 管家**](personas/specialized/zk-steward/) | 卢曼 Zettelkasten 风格的知识库管家，把复杂任务变成知识网络的有机组成部分。 | 构建 Zettelkasten 风格的知识网络 |

---

## 目录结构

每个角色是一个目录，包含：

```
persona-name/
  SOUL.md        # 性格、价值观、语调、身份
  AGENTS.md      # 工作流程、规则、边界
  SKILL.md       # 能力、交付物、工具
  IDENTITY.md    # 名称、形象、风格、表情符号（可选）
  HEARTBEAT.md   # 周期任务定义（可选）
  STYLE.md       # 沟通风格规则（可选）
  BOOTSTRAP.md   # 首次运行的引导流程（可选）
  USER.md        # 用户画像与偏好（可选）
  TOOLS.md       # 工具配置说明（可选）
  MEMORY.md      # 长期沉淀的精选记忆（可选）
```

## 贡献

我们正在打造最大规模的开源生产级 OpenClaw 角色合集 —— 欢迎你的加入。

**我们在找什么：**
- 完整的角色：必须包含 `SOUL.md` 以及至少 `AGENTS.md` 或 `SKILL.md`（仅有 SOUL.md 的提交不会被接受）
- 真实方法论与领域专长，而不是泛泛的提示词
- 你在生产环境真正用过并打磨过的角色

**如何贡献：**
1. Fork 本仓库
2. 在合适分类下新建目录：`personas/[category]/[your-persona-name]/`
3. 添加文件（`SOUL.md`、`AGENTS.md`、`SKILL.md` 与任意可选文件）
4. 附带一个 `README.md`：包含名称、简介、核心能力、文件表、快速开始与使用场景
5. 提交 Pull Request

**质量底线：** 我们会评审每一份提交。本质上只是把系统提示词拆成几个文件、缺乏可执行框架与具体交付物的角色，会被要求补充深度后再合并。

## 来源

*角色来源：[mergisi/awesome-openclaw-agents](https://github.com/mergisi/awesome-openclaw-agents)、[msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents)、[raulvidis/openclaw-multi-agent-kit](https://github.com/raulvidis/openclaw-multi-agent-kit)、[shenhao-stu/openclaw-agents](https://github.com/shenhao-stu/openclaw-agents)、[ClawSouls.ai](https://clawsouls.ai)、[will-assistant/openclaw-agents](https://github.com/will-assistant/openclaw-agents) 与 [souls.directory](https://souls.directory)。所有内容均为免费且注明出处。*
