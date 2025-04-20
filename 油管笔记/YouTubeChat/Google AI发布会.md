



**I. 引言与谷歌云愿景**
- 开场强调全球组织正利用创新解决方案推动变革、提升效率、赋能员工、吸引客户和促进增长。
- 谷歌云CEO Thomas Kurian回顾过去一年的成就：
    - 2024年发布超过3000项产品更新。
    - 谷歌云区域扩展至42个，并计划进一步扩展。
    - 扩展了200万英里的陆地和海底光纤网络，并宣布了新的海底光缆项目。
- 谷歌AI发展势头强劲：
    - 超过400万开发者使用Gemini。
    - Vertex AI使用量去年增长 $20$ 倍。
    - Google Workspace每月提供超过20亿次AI辅助。
- 本次大会将分享超过500个客户利用AI实现业务创新的成功案例。
- 谷歌正投资于技术和生态系统，以支持客户的增长和转型。
- 谷歌与Alphabet CEO Sundar Pichai发言：
    - AI是推进谷歌及客户使命的最重要方式。
    - 谷歌投资全栈AI创新，从基础设施到模型和产品。
    - 计划在2025年投资约 $750$ 亿美元的总资本支出，主要用于服务器和数据中心，支持AI计算和云业务。
    - 谷歌基础设施支持全球数十亿用户，并用于训练最强大的Gemini模型。

**II. 基础设施创新**
- 推出Cloud Wide Area Network (WAN)：
    - 利用谷歌全球规模的网络。
    - 优化应用性能，性能提升超过 $40\%$，总拥有成本降低高达 $40\%$。
    - Citadel Securities和雀巢等公司已在使用。
- 宣布第七代TPU - Ironwood：
    - 将于今年晚些时候推出。
    - 性能是首款公开TPU的 $3600$ 倍，能效提升 $29$ 倍。
    - 是谷歌有史以来最强大的芯片，支持下一代AI模型。
- 量子计算进展：
    - 最新量子芯片Willow解决了困扰研究人员三十年的量子纠错关键挑战。
- AI计算需求增长迅猛：
    - 过去8年，年复合增长率超过 $10$ 倍，总增长达 $10^8$ 倍。
- Ironwood TPU Pods细节：
    - 每个Pod拥有超过9000个芯片，计算能力达 $42.5$ exaflops，是世界第一超算的 $24$ 倍以上。
- AI Hypercomputer：
    - 旨在简化AI部署、提高性能、优化成本的超级计算系统。
    - 支持多种硬件平台（包括NVIDIA的GB200, B200 GPU，未来将支持Vera Rubin GPU）和统一软件栈。
    - 推出Cluster Director管理大规模加速器。
- 存储创新：
    - Hyperdisk Exapools：提供业界领先的聚合性能和容量。
    - Anywhere Cache：数据靠近加速器，存储延迟降低高达 $70\%$。
    - Rapid Storage：区域对象存储，随机读写延迟降低 $5$ 倍。
- 软件与编排增强：
    - Google Kubernetes Engine (GKE) 新增推理能力：降低成本达 $30\%$，尾延迟降低 $60\%$，吞吐量提高 $40\%$。
    - Pathways：Google DeepMind开发的分布式机器学习运行时首次向云客户开放，支持多主机推理。
    - vLLM on TPUs：支持已为GPU优化PyTorch与vLLM的客户在TPU上运行。
- 性能与成本效益：
    - Gemini 2.0 Flash 在AI Hypercomputer上实现每美元智能输出比GPT-4o高 $24$ 倍，比DeepSeek R1高 $5$ 倍。
- Google Distributed Cloud (GDC)：
    - 将谷歌硬件和软件带到客户环境（本地或气隙环境）。
    - 宣布Gemini可在GDC上本地运行。
    - 支持NVIDIA Confidential Computing和Blackwell系统。
    - GDC气隙产品已获美国政府Secret和Top Secret任务授权。
- 与NVIDIA的合作：
    - Jensen Huang强调双方深度合作，将通过GDC把最先进的AI带给受监管行业和国家。

**III. AI模型与平台**
- Gemini模型家族：
    - 推出Gemini 2.0，具有原生图像/音频输出和工具使用能力。
    - 推出Gemini 2.5 Pro：具备“思考”（Thinking）能力，是谷歌迄今最智能模型，ChatbotArena排名第一，在高级推理基准测试中表现优异。
    - 推出Gemini 2.5 Flash：低延迟、高性价比，内置思考能力。
    - Gemini已应用于谷歌所有主要产品（15个用户超5亿的产品）。
    - Gemini在Workspace中的应用：助力Rivian、Freshfields、Schwarz Group等客户。
    - Workspace新功能：Sheets中的“Help Me Analyze”、Docs中的“Audio Overviews”、Workspace Flows自动化流程。
- 其他生成式模型：
    - Imagen 3：更高质量的文本到图像模型，细节更丰富，伪影更少。
    - Chirp 3：通过短语音输入创建自定义语音。
    - Lyria：文本到音乐生成模型，首家提供此功能的超大规模云服务商。
    - Veo 2：行业领先的视频生成模型，可生成数分钟4K视频，带SynthID水印，提供高级编辑控制（镜头预设、首尾帧控制、动态修复/外扩）。
    - 谷歌是唯一提供跨所有模态（文本、图像、音频、视频、音乐）生成模型的公司。
- Vertex AI平台：
    - 提供发现、定制、部署基础模型和构建管理AI智能体的综合平台。
    - 客户案例：Intuit（Document AI简化报税）、Nokia、Wayfair、AES、Commerzbank、Seattle Children's、UWM、Honeywell。
    - 增长迅速：Gemini在Vertex AI上的使用量增长超 $40$ 倍，每月数十亿次API调用。
    - Model Garden：提供超过200个模型，包括谷歌自有模型、第三方模型（如Meta Llama 4）和开源模型（如Ai2模型）。
    - 增强的Grounding能力：连接任意数据源/向量数据库（新增支持NetApp存储）、企业应用（Oracle, SAP等），结合Google Search、企业数据、Google Maps等确保模型回复的事实性。
    - 客户案例：Deutsche Bank使用Gemini和Vertex AI构建AI研究助手DB Lumina。

**IV. AI智能体 (AI Agents)**
- A. 智能体框架与开发：
    - 定义：智能体是展现推理、规划、记忆和工具使用能力的系统。
    - 推出Agent Development Kit (ADK)：简化复杂多智能体系统构建的开源框架，支持Gemini。
    - 支持Model Context Protocol (MCP)：统一模型与数据源/工具交互方式。
    - 推出Agent2Agent Protocol (A2A)：实现不同模型/框架构建的智能体间通信，得到Lang Graph、Crew AI等伙伴支持。
- B. 智能体应用空间 (Agentspace)：
    - 推出Google Agentspace：面向员工，用于查找/综合信息、与AI智能体对话并让其代为操作企业应用的平台。
    - 集成企业搜索、对话AI、Gemini及第三方智能体、工具（连接器）、安全与合规性。
    - Agentspace演示：模拟银行客户经理使用场景，创建个人监控智能体、调用深度研究智能体、进行现金流预测、起草邮件。
    - Agentspace与Chrome浏览器集成，可直接在搜索框访问企业数据。
    - 内置Google专家智能体：NotebookLM（笔记与研究）、Idea Generation（创意生成）、Enterprise Deep Research（企业深度研究）。
    - 客户案例：KPMG、Cohesity、Gordon Food Services、Rubrik、Wells Fargo。
- C. 智能体应用领域：
    - 1. 客户智能体：
        - Vertex AI Search赋能客户发现（Reddit Answers, Lowe's, Mercado Libre）。
        - Customer Engagement Suite (CES) 提升客户服务（DBS银行、Loveholidays、YouTube、Verizon）。
        - 下一代CES：更自然的语音与情感理解、流视频支持、无代码构建、工具集成。
        - CES演示：模拟家居园艺购物场景，展示语音/视频交互、升级人工座席干预流程。
        - 行业特定智能体：Wendy's（汽车穿梭点餐）、Mercedes-Benz（车载对话搜索）、Home Depot（家居改善指导）。
    - 2. 创意智能体：
        - 赋能媒体、营销、设计等创意团队。
        - 案例：Sphere《绿野仙踪》项目（使用Veo 2）、WPP Open平台、Monks.Flow、Brandtech Group Pencil、Mondelez。
        - 与Adobe合作：将Imagen 3和Veo 2模型引入Adobe Express等应用。
    - 3. 数据智能体：
        - 帮助数据团队管理数据，业务团队激活数据。
        - 案例：Mattel（利用Gemini分析消费者反馈）。
        - BigQuery平台：支持结构化与非结构化数据，支持开放格式，跨云访问，集成Oracle OCI。
        - 推出面向数据工程、数据科学、业务分析师的专业智能体。
        - 案例：Spotify、Unilever、Bayer、Nuro、内华达州政府（加速福利审批）。
        - 数据科学演示：使用BigQuery Data Canvas和Notebooks，结合Gemini智能体分析现金流问题，展示从数据准备到模型预测的全流程自动化。
    - 4. 编码智能体：
        - Gemini Code Assist：企业版理解代码库、标准和惯例。
        - 案例：雷诺集团Ampere、Broadcom、CME Group、Paypal、WiPro。
        - 推出新的Code Assist智能体：支持代码现代化、完整软件开发生命周期，提供看板交互界面。
        - 集成Atlassian、Sentry、Snyk等伙伴工具。
        - Gemini也可在Aider、Cursor、GitHub Copilot、Replit等第三方工具中使用。
    - 5. 安全智能体：
        - 提升安全分析师速度和效率。
        - 整合Mandiant威胁情报、SecOps平台、云安全（虚拟红队）、Mandiant服务。
        - 推出新的安全智能体：分析恶意软件、分类警报。
        - 案例：Charles Schwab、Vertiv、Dun & Bradstreet、Vodafone、新加坡政府。
        - 推出Google Unified Security (GUS)：融合安全能力的一体化解决方案。
        - GUS演示：展示如何检测开发者误操作导致的数据泄露、VM遭受攻击，并自动响应、推荐加固措施（Model Armor）。

**V. 生态系统与互操作性**
- 宣布收购网络安全公司Wiz的最终协议。
- 谷歌云通过四种方式促进创新整合：
    - 跨云连接：Cross-Cloud Interconnect、联合身份认证（Microsoft Entra ID）、BigQuery/AlloyDB跨云访问。
    - ISV集成：通过Google Cloud Marketplace提供预集成解决方案。
    - 服务伙伴：Accenture、Capgemini、Deloitte等合作伙伴基于谷歌云推出智能体。
    - 主权云：与合作伙伴共同提供满足国际法规的Google Cloud Sovereign AI服务。

**VI. 总结**
- 谷歌致力于提供领先的企业级AI优化平台、开放的多云平台和互操作性，帮助客户创新并加速AI投资回报。
- 感谢与会者，并宣布下一届Google Cloud Next将于2026年4月22日至24日在拉斯维加斯举行。