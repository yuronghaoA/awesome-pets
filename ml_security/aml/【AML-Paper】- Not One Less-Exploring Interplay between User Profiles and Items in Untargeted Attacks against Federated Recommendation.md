## ✅ 推荐类别：

顶会论文

## ✅ 标题：

Not One Less: Exploring Interplay between User Profiles and Items in Untargeted Attacks against Federated Recommendation

## ✅ 收录会议：

ACM CCS 2024 (Computer and Communications Security, CCF A类会议)

## ✅ 论文链接：

https://doi.org/10.1145/3658644.3670365

## ✅ 原文作者：

Yurong Hao; Xihui Chen; Xiaoting LV; Jiqiang Liu; Yongsheng Zhu; Zhiguo Wan; Sjouke Mauw; Wei Wang.

## ✅ 推荐理由：

### 📘 论文

### 内容简介：

本文是首个系统性探讨非定向投毒攻击（Untargeted Poisoning Attacks）在联邦推荐系统（Federated Recommendation, FR）中的研究工作，围绕“用户画像与物品之间的相互作用”这一核心视角，构建理论框架、设计攻击方案并提出对抗机制，体现出较强的原创性与现实指导意义。

### 技术/理论亮点：

#### 🔷 1. 框架系统性强，揭示攻击本质

* 作者提出首个用于建模联邦推荐系统中非定向攻击的通用攻击框架，将攻击过程细化为两个关键模块：用户画像采样（User Embedding Sampling）与交互样本采样（Interaction Sampling）。

* 框架首次强调攻击效果的核心来源在于用户与物品之间匹配关系的扰乱（即“相互作用的破坏”），突破以往仅对 item embedding 操作的局限。

* 指出若攻击者仅操控单个用户视角构造攻击目标，难以有效逼近总体用户分布，限制了攻击能力。

#### 🔷 2. 攻击设计精细，兼顾实效与隐蔽

* 提出的 FRecAttack2 支持多种攻击场景配置，结合模型类型（secret-hiding / DP-based）及是否具备用户间通信能力（collusion），适应不同联邦推荐系统架构。

* 引入推荐得分“变化速率（velocity）”指标，构建动态切换机制，精准识别最具破坏性的交互样本，显著提升攻击早期效果。

* 攻击策略高度拟合真实用户行为分布，可有效规避主流异常检测与鲁棒聚合防御。

#### 🔷 3. 同步提出通用防御机制 GuardCQ，填补对抗空白

* GuardCQ 为首个从正向建模角度出发的 FR 防御机制，量化用户对推荐系统“正确相互作用”的贡献度以识别潜在恶意用户。

* 设计无需额外标签信息，且可与任意鲁棒聚合机制结合部署，具有良好的扩展性和实际落地潜力。

* 实验验证 GuardCQ 能有效缓解 FRecAttack2 带来的性能劣化，在多个真实场景中展现出高鲁棒性。

### 学习收获或阅读价值：

🔷 1. 提供一种统一视角理解联邦推荐攻击机制的方法论，便于未来构建、分类、比较不同攻击策略。
🔷 2. 明确提出“攻击成功的关键在于破坏用户-物品交互关系”，启发防御研究从“正向建模”视角识别异常行为。
🔷 3. 攻防方法覆盖多个现实数据集与模型场景，体现了方法的普适性与实证严谨性，为联邦推荐安全研究提供有力参考。

文章在理论建模、攻击策略、场景覆盖与防御机制设计方面均具突破性，是当前联邦推荐系统安全研究中的代表性成果，特推荐纳入论文清单。
