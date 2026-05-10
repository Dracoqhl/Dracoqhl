# 你好，我是 Draco 👋

欢迎来到我的 GitHub 主页！

我目前的研究方向是面向复杂场景的大语言模型决策问题，主要关注 **LLM 后训练、Reasoning、Agent** 等方向。博士期间，我持续探索如何提升大语言模型在复杂决策任务中的学习效率与决策鲁棒性。

---

## 关于我

- 🎓 博士研究方向：面向复杂场景的大语言模型决策问题研究
- 🔬 主要研究兴趣：LLM Post-training、Reasoning、Agent
- 💻 熟悉 Linux 开发环境，熟练使用 Python / PyTorch（尤其擅长Vibe Coding）
- 🧠 近期关注：大语言模型在复杂决策问题中的能力提升、推理蒸馏中的数据分布问题、Agentic RL 及 Agent 系统设计
- 📫 联系我: haolongq@163.com
- 😄 兴趣爱好: 编程、运动🏃🏻‍♀️、音乐🎵

---

## 研究经历

### Microsoft Research Asia, MSRA  
**Research Intern｜2024.12 - 2026.04**

在 MSRA 实习期间，我主要专注于大语言模型推理与后训练相关研究工作，探索大语言模型在复杂决策问题中的能力提升，重点关注含噪数据环境下的模型训练、奖励建模、长链推理以及决策鲁棒性等问题。产出两篇人工智能顶会（NeurIPS 2025、ICML 2026）。

---

## 代表性论文

### NaDRO: Leveraging Dual-Reward Strategies for LLMs Training on Noisy Data  
**NeurIPS 2025 Poster｜一作**  
代码仓库: [microsoft/HeurAgenix - NaDRO](https://github.com/microsoft/HeurAgenix/tree/NaDRO)

- **核心发现**：RLVR 范式依赖正确且可验证的答案作为奖励，而决策领域由于庞大的决策空间天然具有含噪属性，使得 RLVR 难以直接迁移到模型决策任务中。
- **核心贡献**：提出 NaDRO 框架，通过双奖励策略提升模型在不完美数据环境下的学习效率与决策鲁棒性。
  - 提出基于偏好的结果奖励 **Preference-based Outcome Reward, POR**，通过学习噪声数据中的相对排序，从根源上缓解因评估不准导致的学习偏差问题。
  - 设计 **上下文感知奖励** 作为过程奖励，在决策前引导模型对问题状态进行准确的定性评估，为长链推理提供稳定且独立的中间训练信号。
- **项目成果**：在 TSP 与 CVRP 等复杂决策任务上进行系统实验，训练后的 Qwen-7B 与 Llama-8B 模型在多个设置下超过 GPT-4o、DeepSeek-R1 等主流大模型。

---

### The Quality-Utility Paradox: Why High-Reward Data Impairs Small Model Reasoning  
**ICML 2026 Poster｜一作**

- **核心发现**：首次发现并系统分析大模型数学推理微调中的 **质量-效用悖论**：强模型生成的高分数据虽然质量更高，但由于存在表达偏差，可能显著增加小模型的学习成本，并导致下游推理性能反常下降。
- **核心贡献**：通过系统实验论证，强模型介入导致的性能下降并非源于逻辑内容本身，而是句法风格层面引入的分布不匹配。进一步发现，加入简单的风格对齐指令即可在修复逻辑错漏的同时，尽可能维持小模型的原生概率分布。
- **项目成果**：在 Qwen2.5、LLaMA-3、DeepSeek 等不同系列与规模的模型上验证了该悖论的普遍存在，并在 MATH500、AIME2024 等数学推理任务上提升了拒绝采样微调 RFT 的性能上限，证明了数据分布在知识蒸馏中的重要作用。

---


## 我的项目

### PhD Workspace / 博士生工作台

项目描述：作为业余爱好开发的博士生科研工作台，面向博士生任务管理与个人提升，通过定制化工具提升自己的工作效率。

使用技术栈：Python, LLM, Vibe Coding

项目链接：[GitHub链接](https://github.com/Dracoqhl/phd-workspace.git)

---

### NaDRO: LLM Post-training on Noisy Decision Data

项目描述：面向含噪复杂决策数据的大语言模型后训练框架，通过结果奖励与过程奖励相结合的方式，提升模型在复杂决策问题中的学习效率与泛化能力。

使用技术栈：Python, PyTorch, LLM Post-training, RLVR, Decision Reasoning

项目链接：[GitHub链接](https://github.com/microsoft/HeurAgenix/tree/NaDRO)

---

### 域泛化 Domain Generalization, DG 任务

项目描述：23 年 SIGS 大数据机器学习课程大作业。我阅读并复现了多篇 ICCV、ECCV 和 CVPR 论文，最终整合三篇域泛化论文的创新点，在课程项目中取得了较高排名。

使用技术栈：Python, PyTorch

项目链接：[GitHub链接](https://github.com/Dracoqhl/DG_model)

---