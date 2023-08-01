# Medical_NLP

医疗NLP领域  评测/比赛，数据集，论文和预训练模型资源汇总。

Summary of medical NLP evaluations/competitions, datasets, papers and pre-trained models.

[中文版本](https://github.com/FreedomIntelligence/Chinese_medical_NLP) [English_version](https://github.com/FreedomIntelligence/Chinese_medical_NLP/blob/master/English_vision.md)

> 由于[Cris Lee](https://github.com/lrs1353281004)2021年离开医疗NLP领域，此repo现由[Xidong Wang](https://github.com/wangxidong06)继续维护。



* [Medical_NLP](#medical_nlp)
   * [1. 评测](#1-评测)
      * [1.1  中文医疗基准测评：CMB / CMExam / PromptCBLUE](#11--中文医疗基准测评cmb--cmexam--promptcblue)
      * [1.2  英文医疗基准测评:](#12--英文医疗基准测评)
   * [2. 比赛](#2-比赛)
      * [2.1 正在进行的比赛](#21-正在进行的比赛)
      * [2.2 已经结束的比赛](#22-已经结束的比赛)
   * [3. 数据集](#3-数据集)
      * [3.1 中文](#31-中文)
      * [3.2 英文](#32-英文)
   * [4. 开源预训练模型](#4-开源预训练模型)
      * [4.1 中文医疗 请参考<a href="https://github.com/HqWu-HITCS/Awesome-Chinese-LLM#%E5%8C%BB%E7%96%97">这里</a>](#41-中文医疗-请参考这里)
      * [4.2 中文通用大模型 请参考<a href="https://github.com/HqWu-HITCS/Awesome-Chinese-LLM">这里</a>](#42-中文通用大模型-请参考这里)
   * [5. 相关论文](#5-相关论文)
   * [6. 开源工具包](#6-开源工具包)
   * [7. 工业级产品解决方案](#7-工业级产品解决方案)
   * [8. blog分享](#8-blog分享)
   * [9. 友情链接](#9-友情链接)
     



## 1. 评测

### 1.1  中文医疗基准测评：CMB / CMExam / PromptCBLUE 

| 名称        | 来源                                                         | 介绍                                                         | github地址                                  | 官方测评网站地址                                             |
| ----------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------- | ------------------------------------------------------------ |
| CMB         | 各个临床医学工种各阶段考试；临床复杂病例问诊                 | 300K选择题，高质量病例问诊题目；全方位多层次注入和测评医疗知识和复杂临床问诊能力 | https://github.com/FreedomIntelligence/CMB  | [https://cmedbenchmark.llmzoo.com](https://cmedbenchmark.llmzoo.com/) |
| CMExam      | 执业医师资格考试往年题                                       | 60K+ 多项选择题和 5 个附加问题注释                           | https://github.com/williamliujl/CMExam      |                                                              |
| PromptCBLUE | CBLUE                                                        | 将CBLUE基准进行二次开发，将16种不同的医疗场景NLP任务全部转化为基于提示的语言生成任务,形成首个中文医疗场景的LLM评测基准。 | https://github.com/michael-wzhu/PromptCBLUE | https://tianchi.aliyun.com/competition/entrance/532085/introduction |
| CBLUE       | CHIP会议往届的学术评测比赛和阿里夸克医疗搜索业务的数据集组成 | 医学文本信息抽取（实体识别、关系抽取）、医学术语归一化、医学文本分类、医学句子关系判定和医学QA共5大类任务8个子任务 | https://github.com/CBLUEbenchmark/CBLUE     | https://tianchi.aliyun.com/dataset/95414                     |

### 1.2  英文医疗基准测评: 

| 名称          | 来源   | 介绍                                                         | github地址 | 官方测评网站地址 |
| ------------- | ------ | ------------------------------------------------------------ | ---------- | ---------------- |
| MultiMedBench | Google | 是一种大型多模态生成模型，可以使用相同的模型权重集灵活地编码和解释生物医学数据，包括临床语言、成像和基因组学 |            |                  |



## 2. 比赛

### 2.1 正在进行的比赛

暂无 欢迎补充~

### 2.2 已经结束的比赛

**英文**

| 名称                                     | 来源                        | 介绍                                                         | 地址                                                         |
| ---------------------------------------- | --------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| BioNLP Workshop 2023 共享任务            | BioNLP Workshop             | 问题列表总结;放射学报告摘要;生物医学研究文章的外行摘要       | https://aclweb.org/aclwiki/BioNLP_Workshop#SHARED_TASKS_2023 |
| MedVidQA 2023                            | 美国国立卫生研究院          | 在线视频可用性的激增改变了获取信息和知识的方式。以类似的方式，医疗教学视频更适合和有益于通过视觉和口头交流向消费者需要指导的医疗保健问题传递关键信息。本任务由两个主要任务组成：视频语料库视觉答案定位  (VCVAL) 和医学教学问题生成 (MIQG)。 | https://medvidqa.github.io/index.html                        |
| MEDIQA-2021                              | NAACL-BioNLP 2021 workshop. | 解决医疗领域的三项摘要任务：消费者健康问题摘要、多答案摘要和放射报告摘要，并探索使用不同的评估指标进行总结。 | https://sites.google.com/view/mediqa2021                     |
| ICLR-2021-医疗对话生成与自动诊断国际竞赛 | ICLR 2021 workshop          | 本次竞赛以自动医疗诊断对话系统的开发为主题，目前设置了两大赛道：医疗对话生成赛道和自动医疗诊断赛道。 | https://mlpcp21.github.io/pages/challenge                    |

**中文**

| 名称                                         | 来源                                | 介绍                                                         | 地址                                                         |
| -------------------------------------------- | ----------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 影像学NLP —— 医学影像诊断报告生成            | 2023全球人工智能技术创新大赛 赛道一 | 本赛道任务要求参赛队伍根据医生对CT的影像描述文本数据（即对医学影像特征的描述），生成诊断报告文本。与传统文本生成任务不同的是，医学影像诊断报告内容具有专业性、明确性和离散性，因此也需要针对性的算法与模型设计。报告生成结果按照指定评价指标进行评测和排名，得分最优者获胜。 | https://gaiic.caai.cn/ai2023/                                |
| 非标准化疾病诉求的简单分诊挑战赛2.0          | 科大讯飞                            | 进行简单分诊需要一定的数据和经验知识进行支撑。本次比赛提供了部分好大夫在线的真实问诊数据，经过严格脱敏，提供给参赛者进行单分类任务。具体为：通过处理文字诉求，给出20个常见的就诊方向之一和61个疾病方向之一。 | http://challenge.xfyun.cn/topic/info?type=disease-claims-2022&ch=ds22-dw-sq03 |
| 第八届中国健康信息处理大会(CHIP2022)测评任务 | CHIP2022                            | 面向“基因-疾病”的关联语义挖掘任务;  医疗因果实体关系抽取任务;从医疗文本中抽取诊疗决策树;医疗纸质文档电子档(ePaper)OCR识别;临床诊断编码任务 | http://cips-chip.org.cn/)                                    |
| 科大讯飞-医疗实体及关系识别挑战赛            | 科大讯飞                            | 针对医技报告单(一种半结构化的数据，不同医生的表述风格不一致，文本形式缺乏统一的规范)的命名实体识别和实体关系抽取。 | http://www.fudan-disc.com/sharedtask/imcs21/index.html       |





## 3. 数据集

### 3.1 中文

| 名称                              | 介绍                                                         | 地址                                                         |
| --------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Huatuo-26M                        | Huatuo-26M 是迄今为止最大的中医问答数据集。该数据集包含超过 2600  万条高质量医学问答对，涵盖疾病、症状、治疗和药物信息等广泛主题。Huatuo-26M  对于希望增强医疗领域人工智能应用（例如聊天机器人、智能诊断系统等）的研究人员、开发人员和公司来说是宝贵的资源。 | https://github.com/FreedomIntelligence/Huatuo-26M            |
| Yidu-S4K                          | 命名实体识别,实体及属性抽取                                  | http://openkg.cn/dataset/yidu-s4k                            |
| Yidu-N7K                          | 临床语标准化                                                 | http://openkg.cn/dataset/yidu-n7k                            |
| 中文医药方面的问答数据集          | 医疗问答                                                     | https://github.com/zhangsheng93/cMedQA2                      |
| 中文医患问答对话数据              | 医疗问答                                                     | https://github.com/UCSD-AI4H/Medical-Dialogue-System         |
| 中文医疗对话数据集                | 包含六个科室的医学问答数据，github开源数据 ，来源不明。      | https://github.com/Toyhom/Chinese-medical-dialogue-data      |
| CPubMed-KG (4.4M三元组)           | 中华医学会高质量全文期刊数据所构建的大规模中文开放医学知识图谱及开放式医学知识在线协同构建平台，旨在通过完全开放、协作的机制来打破中文医学知识的瓶颈，支撑智慧医疗技术的发展。 | https://cpubmed.openi.org.cn/graph/wiki                      |
| CBLUE                             | 涵盖了医学文本信息抽取（实体识别、关系抽取）、医学术语归一化、医学文本分类、医学句子语义相关性判定、医疗对话理解和生成5大类常见的医疗信息处理任务，共包含15个子任务。 | https://github.com/CBLUEbenchmark/CBLUE                      |
| 中文医学知识图谱 CMeKG (1M三元组) | CMeKG（Chinese Medical Knowledge  Graph）是利用自然语言处理与文本挖掘技术，基于大规模医学文本数据，以人机结合的方式研发的中文医学知识图谱。 | http://cmekg.pcl.ac.cn/                                      |
| cMedQA2 (108K)                    | 中文医药方面的问答数据集，超过10万条。                       | https://github.com/zhangsheng93/cMedQA2                      |
| xywy-KG(294K三元组)               | 44.1K实体 294.1K 三元组                                      | https://github.com/baiyang2464/chatbot-base-on-Knowledge-Graph |
| 39Health-KG (210K三元组)          | 包括15项信息，其中7类实体，约3.7万实体，21万实体关系。       | https://github.com/zhihao-chen/QASystemOnMedicalGraph        |
| CHIP历年测评 (官方测评)           | CHIP历年测评 (官方测评)                                      | http://cips-chip.org.cn/2022/callforeval ;  http://www.cips-chip.org.cn/2021/ ;   http://cips-chip.org.cn/2020/ |
| 瑞金医院糖尿病数据集 (糖尿病)     | 数据集来自天池大赛。此数据集旨在通过糖尿病相关的教科书、研究论文来做糖尿病文献挖掘并构建糖尿病知识图谱。参赛选手需要设计高准确率，高效的算法来挑战这一科学难题。第一赛季课题为“基于糖尿病临床指南和研究论文的实体标注构建”，第二赛季课题为“基于糖尿病临床指南和研究论文的实体间关系构建”。 | https://tianchi.aliyun.com/competition/entrance/231687/information |
| 天池新冠肺炎问句匹配比赛 (新冠)   | 本次大赛数据包括：脱敏之后的医疗问题数据对和标注数据。医疗问题涉及“肺炎”、“支原体肺炎”、“支气管炎”、“上呼吸道感染”、“肺结核”、“哮喘”、“胸膜炎”、“肺气肿”、“感冒”、“咳血”等10个病种。 | https://tianchi.aliyun.com/competition/entrance/231776/information |

### 3.2 英文

| 名称        | 介绍                                          | 地址                                          |
| ----------- | --------------------------------------------- | --------------------------------------------- |
| PubMedQA    | 基于Pubmed提取的医学问答数据集                | https://arxiv.org/abs/1909.06146              |
| COMETA      | 社交媒体中的医疗实体链接数据。发表于EMNLP2020 | https://www.siphs.org/                        |
| MedMentions | 基于Pubmed摘要的生物医学实体链接数据集        | https://github.com/chanzuckerberg/MedMentions |
| webMedQA    | 医疗问答                                      | https://github.com/hejunqing/webMedQA         |
| MediQA      | 文本概括                                      | https://sites.google.com/view/mediqa2021      |





## 4. 开源预训练模型

### 4.1 中文医疗 请参考[这里](https://github.com/HqWu-HITCS/Awesome-Chinese-LLM#%E5%8C%BB%E7%96%97)

### 4.2 中文通用大模型 请参考[这里](https://github.com/HqWu-HITCS/Awesome-Chinese-LLM)





## 5. 相关论文

此部分 更加侧重于收集 后ChatGPT时代的相关论文，大致以论文发表时间为序。

### 0. ChatGPT/GPT-4 从何而来？(Thanks to CloseAI, strictly speaking we don't know how ChatGPT and GPT-4 came about. But show the respect to the scientists and engineers at this institution who pushed the boundaries of AI's capability.)

#### 0.0 RLHF

##### 0.0.1 openai RLHF+NLP之前 出现在RLHF领域的工作

###### 0.0.1.1 从轨迹偏好查询中学习政策的贝叶斯方法(NIPS 2012)

- 论文地址：https://papers.nips.cc/paper/2012/hash/16c222aa19898e5058938167c8ab6c57-Abstract.html
- 摘要翻译：我们考虑通过向专家查询轨迹偏好来学习控制策略的问题。特别是，学习代理可以向专家展示源自同一状态的一对策略的短期运行，然后专家指示首选轨迹。代理的目标是用尽可能少的查询从专家那里引出一个潜在的目标策略。为了解决这个问题，我们提出了一种新颖的查询过程贝叶斯模型，并介绍了两种利用该模型主动选择专家查询的方法。四个基准问题的实验结果表明，我们的模型可以有效地从轨迹偏好查询中学习策略，并且主动查询选择可以比随机选择更有效。

###### 0.0.1.2 通过人类反馈训练机器人：案例研究(ICSR 2013)

- 论文地址：https://link.springer.com/chapter/10.1007/978-3-319-02675-6_46
- 摘要翻译：我们提出了一个案例研究，该案例研究将用于从数字人类反馈中学习的框架 - TAMER - 应用于物理体现的机器人。在此过程中，我们还首次展示了无需算法修改即可通过此类反馈训练多种行为的能力，以及机器人无需任何进一步指导或评估反馈即可从自由形式的人类生成的反馈中学习的能力。我们描述了从人类反馈和调整中学习以应对这些挑战的物理机器人所特有的透明度挑战。

###### 0.0.1.3 APRIL：基于主动偏好学习的强化学习(2012)

- 论文地址：https://arxiv.org/abs/1208.0984
- 摘要翻译：本文侧重于先验知识有限的强化学习 (RL)。例如，在群体机器人领域，专家很难设计奖励函数或展示目标行为，禁止使用标准 RL 和逆强化学习。尽管专业知识有限，人类专家仍然经常能够发出偏好并对代理演示进行排名。早期的工作提出了一种基于迭代偏好的 RL 框架：利用专家偏好来学习近似的策略回报，从而使代理能够实现直接策略搜索。迭代地，智能体选择一个新的候选策略并进行演示；专家将新的演示与之前的最佳演示进行比较；专家的排名反馈使代理能够细化近似的政策回报，并且这个过程是迭代的。在本文中，基于偏好的强化学习与主动排名相结合，以减少对产生令人满意的策略所需的专家的排名查询数量。在山地车和癌症治疗试验台上进行的实验证明，几十个排名能够学习出有效的策略。

###### 0.0.1.4 通过反馈编程(2014)

- 论文地址：https://hal.inria.fr/hal-00980839
- 摘要翻译：本文提倡一种新的基于 ML 的编程框架，称为反馈编程 (PF)，它涉及活动计算机和用户之间的一系列交互。后者仅提供对活动计算机提供的成对解决方案的偏好判断。主动计算机涉及一个学习和一个优化组件；学习部分估计用户的效用函数并说明用户的（可能有限的）能力；优化组件探索搜索空间并返回最合适的候选解决方案。提出了该方法的原理证明，表明 PF 需要少量交互才能解决一些离散和连续的基准问题。

###### 0.0.1.5 在 Atari 中从人类偏好和示范中进行奖励学习(2018)

- 论文地址：https://arxiv.org/abs/1811.06521
- 摘要翻译：要通过强化学习解决复杂的现实世界问题，我们不能依赖手动指定的奖励函数。相反，我们可以让人类直接向代理传达目标。在这项工作中，我们结合了两种从人类反馈中学习的方法：专家演示和轨迹偏好。我们训练一个深度神经网络来模拟奖励函数，并使用其预测奖励在 9 个 Atari 游戏上训练一个基于 DQN 的深度强化学习代理。我们的方法在 7 场比赛中击败了模仿学习基线，并在 2 场比赛中在不使用游戏奖励的情况下实现了严格的超人表现。此外，我们调查了奖励模型的拟合优度，提出了一些奖励黑客问题，并研究了人类标签中噪声的影响。

##### 0.0.2 openai RLHF思维链路(有一点个人主观biase)

###### 0.0.2.1 高效反馈(2015) Start from this [blog](https://ai-alignment.com/efficient-feedback-a347748b1557#.exjnsupts)！ 促成了0.0.2.3 的尝试

- 论文地址：https://ai-alignment.com/efficient-feedback-a347748b1557#.exjnsupts

- 摘要翻译：在某些机器学习领域，例如图像分类，我们可以产生一堆标记的训练数据，并使用相同的数据来训练许多模型。这种范式非常有效，但并不总是适用。例如：

  - 与其模仿人类的决定，我们可能更想训练一个系统来做出人类会积极评价的决定。如果可能输出的空间很大，反馈将有效地特定于正在训练的特定算法。

  - 如果一个学习系统与一个复杂的环境交互，不同的算法将以不同的方式塑造它们的环境，并发现自己处于不同的情况——需要不同的训练数据。

  这些情况很自然，但很难用通常的范例来解决。如果我们有兴趣将数据密集型算法应用于具有这些特征的领域，这就是一个问题。在这种情况下，每当我们想要训练一个新模型时，甚至在单个模型的训练过程中，我们可能需要收集大量新数据。

  这是实施反事实监督的一个特别重要的挑战；我认为这也是当今实施许多实用的AI控制项目的重要障碍。

###### 0.0.2.2 [使用损坏的奖励渠道进行强化学习](https://openai.com/research/faulty-reward-functions)(2017.3 openai) openai对RL Policy安全性的考虑 促成了0.0.2.4/5 的尝试

- 论文地址：https://arxiv.org/abs/1705.08417
- Blog: https://openai.com/research/faulty-reward-functions
- 摘要翻译：现实世界中没有一个奖励函数是完美的。感官错误和软件错误可能会导致 RL 智能体观察到比他们应有的更高（或更低）的奖励。例如，强化学习代理可能更喜欢感觉错误为其提供最大奖励但真正奖励实际上很小的状态。我们将此问题形式化为称为腐败奖励 MDP 的广义马尔可夫决策问题。传统的 RL 方法在 CRMDP 中表现不佳，即使在强大的简化假设下以及试图补偿可能腐败的奖励时也是如此。研究了解决该问题的两种方法。首先，通过为代理提供更丰富的数据，例如在逆向强化学习和半监督强化学习中，有时可能会完全控制由系统性感官错误引起的奖励腐败。其次，通过使用随机化来削弱代理的优化，奖励腐败可以在某些假设下得到部分管理。

###### 0.0.2.3 [从人类偏好中深度强化学习](https://openai.com/research/learning-from-human-preferences)(2017.6 openai) RLHF in RL 初探

- 论文地址：https://arxiv.org/abs/1706.03741
- Blog：https://openai.com/research/learning-from-human-preferences
- 摘要翻译：为了使复杂的强化学习 (RL) 系统与现实环境进行有效交互，我们需要将复杂的目标传达给这些系统。在这项工作中，我们探索了根据成对轨迹段之间的（非专家）人类偏好定义的目标。我们表明，这种方法可以有效地解决复杂的 RL 任务，而无需访问奖励功能，包括 Atari 游戏和模拟机器人运动，同时提供不到 1% 的智能体与环境交互的反馈。这大大降低了人类监督的成本，以至于它可以实际应用于最先进的 RL 系统。为了证明我们方法的灵活性，我们表明我们可以用大约一个小时的人类时间成功训练复杂的新行为。这些行为和环境比以前从人类反馈中学到的任何行为和环境都要复杂得多。



###### 0.0.2.4  [通过辩论提升人工智能安全](https://openai.com/research/debate) (2018.5 openai)  通过辩论 实现RL安全 解决0.0.2.2

- 论文地址：https://arxiv.org/abs/1805.00899
- Blog：https://openai.com/research/debate
- 摘要翻译：为了使人工智能系统广泛用于具有挑战性的现实世界任务，我们需要它们学习复杂的人类目标和偏好。一种指定复杂目标的方法要求人类在训练期间判断哪些代理行为是安全和有用的，但如果任务太复杂以至于人类无法直接判断，这种方法可能会失败。为了帮助解决这个问题，我们建议通过在零和辩论游戏中自我对弈来训练代理。给定一个问题或建议采取的行动，两个代理人轮流在一定限度内做出简短陈述，然后由人类判断哪个代理人提供了最真实、最有用的信息。类比于复杂性理论，最优玩法的辩论可以回答给定多项式时间判断的 PSPACE 中的任何问题（直接判断只回答 NP 问题）。在实践中，辩论是否有效涉及关于人类和我们希望人工智能执行的任务的经验问题，以及关于人工智能对齐意义的理论问题。我们报告了初始 MNIST 实验的结果，其中代理竞争说服稀疏分类器，将分类器的准确度从 59.4% 提高到 88.9%，给定 6 个像素，从 48.2% 提高到 85.2%，给定 4 个像素。最后，我们讨论了辩论模型的理论和实践方面，重点关注模型扩大时的潜在弱点，我们提出未来的人类和计算机实验来测试这些特性。9% 给定 6 个像素，48.2% 到 85.2% 给定 4 个像素。最后，我们讨论了辩论模型的理论和实践方面，重点关注模型扩大时的潜在弱点，我们提出未来的人类和计算机实验来测试这些特性。9% 给定 6 个像素，48.2% 到 85.2% 给定 4 个像素。最后，我们讨论了辩论模型的理论和实践方面，重点关注模型扩大时的潜在弱点，我们提出未来的人类和计算机实验来测试这些特性。



###### 0.0.2.5 [通过放大弱专家来监督强学习者](https://openai.com/research/learning-complex-goals-with-iterated-amplification) (2018.10 openai)   迭代放大的 RL 安全技术 解决0.0.2.2

- 论文地址：https://arxiv.org/abs/1810.08575
- Blog：https://openai.com/research/learning-complex-goals-with-iterated-amplification
- 摘要翻译：许多现实世界的学习任务涉及复杂或难以指定的目标，使用更容易指定的代理可能会导致性能不佳或行为失调。一种解决方案是让人类通过演示或判断性能来提供训练信号，但如果任务太复杂以至于人类无法直接评估，这种方法就会失败。我们提出了迭代放大，这是一种替代训练策略，它通过组合更简单的子问题的解决方案来逐步建立困难问题的训练信号。 Iterated Amplification 与 Expert Iteration 密切相关 (Anthony et al., 2017; Silver et al., 2017)，只是它不使用外部奖励函数。我们在算法环境中展示结果，表明迭代放大可以有效地学习复杂的行为。



###### 0.0.2.6 [根据人类偏好微调语言模型]( https://openai.com/research/fine-tuning-gpt-2)(根据人类偏好微调 GPT-2) (2019 openai) First NLP+RLHF!

- 论文地址：https://arxiv.org/abs/1909.08593
- Blog: https://openai.com/research/fine-tuning-gpt-2
- 代码地址：https://github.com/openai/lm-human-preferences
- 摘要翻译：奖励学习使强化学习 (RL) 能够应用于奖励由人类判断定义的任务，通过向人类提问来建立奖励模型。大多数关于奖励学习的工作都使用了模拟环境，但关于价值的复杂信息通常用自然语言表达，我们认为语言奖励学习是使 RL 在现实世界任务中实用和安全的关键。在本文中，我们基于语言模型生成预训练的进展，将奖励学习应用于四种自然语言任务：具有积极情绪的连续文本或物理描述性语言，以及 TL；DR 和 CNN/每日邮报数据集上的摘要任务。对于风格的延续，我们仅通过人工评估的 5,000 次比较就取得了良好的效果。对于总结，经过 60,000 次比较训练的模型从输入中复制整个句子，但跳过不相关的序言；根据我们的人类贴标机，这会导致合理的 ROUGE 分数和非常好的性能，但可能利用了贴标机依赖简单启发式的事实。



###### 0.0.2.7 [RLHF in 摘要生成](https://openai.com/research/learning-to-summarize-with-human-feedback)(openai 2020)  Second try NLP+RLHF!

- 论文地址：https://arxiv.org/abs/2009.01325
- Blog：https://openai.com/research/learning-to-summarize-with-human-feedback
- 代码地址：https://github.com/openai/summarize-from-feedback
- 摘要翻译：随着语言模型变得越来越强大，训练和评估越来越受到用于特定任务的数据和指标的瓶颈。例如，摘要模型通常经过训练以预测人类参考摘要并使用 ROUGE 进行评估，但这两个指标都粗略地代表了我们真正关心的内容——摘要质量。在这项工作中，我们表明可以通过训练模型来优化人类偏好来显着提高摘要质量。我们收集了一个大型、高质量的人类比较摘要数据集，训练一个模型来预测人类偏好的摘要，并将该模型用作奖励函数，以使用强化学习微调摘要策略。我们将我们的方法应用于 TL 的一个版本；Reddit 帖子的 DR 数据集发现我们的模型明显优于人类参考摘要和仅通过监督学习进行微调的更大模型。我们的模型还转移到 CNN/DM 新闻文章，生成的摘要几乎与人类参考一样好，无需任何新闻特定的微调。我们进行广泛的分析以了解我们的人类反馈数据集和微调模型我们确定我们的奖励模型可以推广到新的数据集，并且优化我们的奖励模型会比根据人类优化 ROUGE 产生更好的总结。我们希望我们论文中的证据能够激励机器学习研究人员更加关注他们的训练损失如何影响他们实际想要的模型行为。我们的模型还转移到 CNN/DM 新闻文章，生成的摘要几乎与人类参考一样好，无需任何新闻特定的微调。我们进行广泛的分析以了解我们的人类反馈数据集和微调模型我们确定我们的奖励模型可以推广到新的数据集，并且优化我们的奖励模型会比根据人类优化 ROUGE 产生更好的总结。我们希望我们论文中的证据能够激励机器学习研究人员更加关注他们的训练损失如何影响他们实际想要的模型行为。我们的模型还转移到 CNN/DM 新闻文章，生成的摘要几乎与人类参考一样好，无需任何新闻特定的微调。我们进行广泛的分析以了解我们的人类反馈数据集和微调模型我们确定我们的奖励模型可以推广到新的数据集，并且优化我们的奖励模型会比根据人类优化 ROUGE 产生更好的总结。我们希望我们论文中的证据能够激励机器学习研究人员更加关注他们的训练损失如何影响他们实际想要的模型行为。我们进行广泛的分析以了解我们的人类反馈数据集和微调模型我们确定我们的奖励模型可以推广到新的数据集，并且优化我们的奖励模型会比根据人类优化 ROUGE 产生更好的总结。我们希望我们论文中的证据能够激励机器学习研究人员更加关注他们的训练损失如何影响他们实际想要的模型行为。我们进行广泛的分析以了解我们的人类反馈数据集和微调模型我们确定我们的奖励模型可以推广到新的数据集，并且优化我们的奖励模型会比根据人类优化 ROUGE 产生更好的总结。我们希望我们论文中的证据能够激励机器学习研究人员更加关注他们的训练损失如何影响他们实际想要的模型行为。



###### 0.0.2.8 [TruthfulQA](https://openai.com/research/truthfulqa)：衡量模型如何模仿人类的谎言 (2021.8.9)  摘要最后一句话：最大的模型通常是最不真实的，我们建议单独扩大模型在提高真实性方面不如使用训练目标进行微调而不是模仿网络文本。   directly lead to 0.0.2.9

- 论文地址：https://arxiv.org/abs/2109.07958
- Blog:https://openai.com/research/truthfulqa
- 摘要翻译：我们提出了一个基准来衡量语言模型在生成问题答案时是否真实。该基准包括 817 个问题，涵盖 38 个类别，包括健康、法律、金融和政治。我们精心设计了一些人会由于错误的信念或误解而错误回答的问题。为了表现良好，模型必须避免生成从模仿人类文本中学到的错误答案。我们测试了 GPT-3、GPT-Neo/J、GPT-2 和基于 T5 的模型。最好的模型在 58% 的问题上是真实的，而人类的表现是 94%。模型生成了许多错误答案，模仿流行的误解并有可能欺骗人类。最大的模型通常是最不真实的。这与其他 NLP 任务形成对比，在其他 NLP 任务中，性能随模型大小而提高。然而，如果从训练分布中学习到错误答案，则此结果是预期的。我们建议单独扩大模型在提高真实性方面不如使用训练目标进行微调而不是模仿网络文本。



###### 0.0.2.9 [instruct GPT]( https://openai.com/research/instruction-following)(2022.1 openai)  0.0.2.6/7中探索的技术终于和GPT-3进行了对齐！  重点：尽管参数少了 100 多倍，但我们的标签制作者更喜欢1.3B InstructGPT模型的输出，而不是175BGPT-3模型的输出。 I have a question: What if ChatGPT IS MOE of instructGPT-1.3B/6B?

- 论文地址：https://arxiv.org/abs/2203.02155
- Blog: https://openai.com/research/instruction-following
- 摘要翻译：使语言模型更大并不能从本质上使它们更好地遵循用户的意图。例如，大型语言模型可能会生成不真实的、有毒的或对用户没有帮助的输出。换句话说，这些模型与其用户不一致。在本文中，我们展示了一种途径，可以通过根据人类反馈进行微调，使语言模型与用户对各种任务的意图保持一致。从一组标记器编写的提示和通过 OpenAI API 提交的提示开始，我们收集了所需模型行为的标记器演示数据集，我们用它来使用监督学习微调 GPT-3。然后，我们收集模型输出排名的数据集，我们使用该数据集通过人类反馈的强化学习进一步微调该监督模型。我们将生成的模型称为 InstructGPT。在对我们的提示分布的人工评估中，1.3B 参数 InstructGPT 模型的输出优于 175B GPT-3 的输出，尽管参数少 100 倍。此外，InstructGPT 模型显示了真实性的提高和有毒输出生成的减少，同时对公共 NLP 数据集的性能回归最小。尽管 InstructGPT 仍然会犯一些简单的错误，但我们的结果表明，根据人类反馈进行微调是使语言模型与人类意图保持一致的一个有前途的方向。
- **重点：尽管参数少了 100 多倍，但我们的标签制作者更喜欢 1.3B InstructGPT 模型的输出，而不是 175B GPT-3 模型的输出。**





#### 0.1 GPT-x 及其变体的迭代过程

##### 0.1.0 硬件资源和调度的迭代

###### 0.1.0.1 [kubernetes](https://kubernetes.io/)

###### 0.1.0.2 [将 Kubernetes 扩展到 2,500 个节点](https://openai.com/research/scaling-kubernetes-to-2500-nodes)

- Blog地址：https://openai.com/research/scaling-kubernetes-to-2500-nodes

###### 0.1.0.3 将 [Kubernetes 扩展到 7,500 个节点](https://openai.com/research/scaling-kubernetes-to-7500-nodes) 为大型模型提供了可扩展的基础设施。同时也为神经语言模型的缩放定律等快速小规模迭代研究提供了基础设施。

- Blog地址：https://openai.com/research/scaling-kubernetes-to-7500-nodes



##### 0.1.1 模型的迭代

###### 0.1.1.1 [GPT](https://openai.com/research/language-unsupervised)(2018.6.11 openai)

- 论文地址：https://cdn.openai.com/research-covers/language-unsupervised/language_understanding_paper.pdf
- 代码地址：https://github.com/openai/finetune-transformer-lm

- Blog地址：https://openai.com/research/language-unsupervised
- 摘要翻译：自然语言理解包括范围广泛的不同任务，例如文本蕴含、问答、语义相似性评估和文档分类。 尽管大量未标记的文本语料库很丰富，但用于学习这些特定任务的标记数据却很少，这使得经过判别训练的模型难以充分执行。 我们证明，通过在不同的未标记文本语料库上对语言模型进行生成式预训练，然后对每个特定任务进行判别式微调，可以实现这些任务的巨大收益。 与以前的方法相比，我们在微调期间使用任务感知输入转换来实现有效传输，同时需要对模型架构进行最少的更改。 我们证明了我们的方法在广泛的自然语言理解基准上的有效性。 我们的通用任务不可知模型优于使用专门为每项任务设计的架构的有区别训练的模型，显着改进了所研究的 12 项任务中的 9 项的最新技术水平。 例如，我们在常识推理（Stories Cloze Test）上实现了 8.9% 的绝对改进，在问题回答（RACE）上实现了 5.7%，在文本蕴含（MultiNLI）上实现了 1.5% 的绝对改进。

###### 0.1.1.2 [GPT-2](https://openai.com/research/better-language-models)(2019.2.14 openai)

- 论文地址：https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf

- BLog地址：https://openai.com/research/better-language-models
- 摘要翻译：自然语言处理任务，例如问答、机器翻译、阅读理解和摘要，通常通过对任务特定数据集的监督学习来处理。 我们证明，当在一个名为 WebText 的数百万网页的新数据集上接受训练时，语言模型在没有任何明确监督的情况下开始学习这些任务。 当以文档加问题为条件时，语言模型生成的答案在 CoQA 数据集上达到 55F1——在不使用 127、000+ 训练示例的情况下匹配或超过 3out of 4 基线系统的性能。 语言模型的容量对于零样本任务传输的成功至关重要，并且增加它可以跨任务以对数线性方式提高性能。 我们最大的模型 GPT-2 是一个 1.5B 参数 Transformer，它在零样本设置中的 8 个测试语言建模数据集中的 7 个上取得了最先进的结果，但仍然不适合 WebText。 模型中的示例反映了这些改进并包含连贯的文本段落。 这些发现为构建语言处理系统提供了一条有前途的途径，这些系统可以从自然发生的演示中学习执行任务。
- 代码地址：https://github.com/openai/gpt-2



###### 0.1.1.3 [GPT-3: 语言模型是小样本学习者](https://openai.com/research/language-models-are-few-shot-learners) (2020.3.28 openai)

- 论文地址：https://arxiv.org/abs/2005.14165
- Blog地址：https://openai.com/research/language-models-are-few-shot-learners
- 摘要翻译：最近的工作表明，通过对大量文本语料库进行预训练，然后对特定任务进行微调，许多 NLP 任务和基准测试取得了实质性进展。虽然在体系结构中通常与任务无关，但此方法仍然需要特定于任务的微调数据集，其中包含数千或数万个示例。相比之下，人类通常只能通过几个例子或简单的指令来执行一项新的语言任务——这是当前的 NLP 系统在很大程度上仍然难以做到的。在这里，我们展示了扩大语言模型极大地提高了与任务无关的、少样本的性能，有时甚至可以与之前最先进的微调方法相媲美。具体来说，我们训练 GPT-3，这是一种具有 1750 亿个参数的自回归语言模型，比以前的任何非稀疏语言模型多 10 倍，并测试其在少镜头设置中的性能。对于所有任务，GPT-3 都在没有任何梯度更新或微调的情况下应用，任务和小样本演示完全通过与模型的文本交互来指定。GPT-3 在许多 NLP 数据集上实现了强大的性能，包括翻译、问答和完形填空任务，以及一些需要即时推理或领域适应的任务，例如解读单词，在句子，或执行 3 位数算术。同时，我们还确定了一些 GPT-3 的少样本学习仍然困难的数据集，以及一些 GPT-3 面临与大型网络语料库训练相关的方法论问题的数据集。最后，我们发现 GPT-3 可以生成新闻文章样本，人类评估者很难将这些文章与人类撰写的文章区分开来。我们总体上讨论了这一发现和 GPT-3 的更广泛的社会影响。

###### 0.1.1.4 [CLIP](https://openai.com/research/clip) 从自然语言监督中学习可迁移视觉模型(2021.1.5openai)

- 论文地址：https://arxiv.org/abs/2103.00020
- Blog地址：https://openai.com/research/clip
- 摘要翻译：最先进的计算机视觉系统经过训练可以预测一组固定的预定对象类别。这种受限的监督形式限制了它们的通用性和可用性，因为需要额外的标记数据来指定任何其他视觉概念。直接从有关图像的原始文本中学习是一种很有前途的替代方案，它可以利用更广泛的监督资源。我们证明了预测哪个标题与哪个图像对应的简单预训练任务是一种有效且可扩展的方式，可以在从互联网收集的 4 亿（图像、文本）对数据集上从头开始学习 SOTA 图像表示。预训练后，使用自然语言来引用学习到的视觉概念（或描述新概念），从而实现模型到下游任务的零样本迁移。我们通过对 30 多个不同的现有计算机视觉数据集进行基准测试来研究这种方法的性能，涵盖 OCR、视频中的动作识别、地理定位和许多类型的细粒度对象分类等任务。该模型可以轻松地迁移到大多数任务，并且通常可以与完全监督的基线相媲美，而无需任何数据集特定的训练。例如，我们在 ImageNet 零镜头上匹配原始 ResNet-50 的准确性，而无需使用它所训练的 128 万个训练示例中的任何一个。我们发布我们的代码和预训练模型权重 该模型可以轻松地迁移到大多数任务，并且通常可以与完全监督的基线相媲美，而无需任何数据集特定的训练。例如，我们在 ImageNet 零镜头上匹配原始 ResNet-50 的准确性，而无需使用它所训练的 128 万个训练示例中的任何一个。我们发布我们的代码和预训练模型权重 该模型可以轻松地迁移到大多数任务，并且通常可以与完全监督的基线相媲美，而无需任何数据集特定的训练。例如，我们在 ImageNet 零镜头上匹配原始 ResNet-50 的准确性，而无需使用它所训练的 128 万个训练示例中的任何一个。

###### 0.1.1.5 [CodeX](https://openai.com/blog/openai-codex) 评估在代码上训练的大型语言模型 (2021.6.7 openai)

- 论文地址：https://arxiv.org/abs/2107.03374
- Blog地址：https://openai.com/blog/openai-codex
- 摘要翻译：我们介绍了 Codex，一种根据 GitHub 的公开可用代码进行微调的 GPT 语言模型，并研究了其 Python 代码编写能力。Codex 的独特生产版本为 GitHub Copilot 提供支持。在 HumanEval 上，我们发布了一个新的评估集来衡量从文档字符串合成程序的功能正确性，我们的模型解决了 28.8% 的问题，而 GPT-3 解决了 0%，GPT-J 解决了 11.4%。此外，我们发现从模型中重复抽样是一种非常有效的策略，可以为困难的提示生成有效的解决方案。使用这种方法，我们解决了 70.2% 的问题，每个问题有 100 个样本。对我们模型的仔细调查揭示了它的局限性，包括难以描述长操作链的文档字符串以及难以将操作绑定到变量。最后，我们讨论了部署强大的代码生成技术的潜在更广泛影响，涵盖安全性、保障性和经济性。

###### 0.1.1.6 [instruct GPT]( https://openai.com/research/instruction-following)(2022.6.27 openai)  

- 论文地址：https://arxiv.org/abs/2203.02155
- Blog: https://openai.com/research/instruction-following
- 摘要翻译：使语言模型更大并不能从本质上使它们更好地遵循用户的意图。例如，大型语言模型可能会生成不真实的、有毒的或对用户没有帮助的输出。换句话说，这些模型与其用户不一致。在本文中，我们展示了一种途径，可以通过根据人类反馈进行微调，使语言模型与用户对各种任务的意图保持一致。从一组标记器编写的提示和通过 OpenAI API 提交的提示开始，我们收集了所需模型行为的标记器演示数据集，我们用它来使用监督学习微调 GPT-3。然后，我们收集模型输出排名的数据集，我们使用该数据集通过人类反馈的强化学习进一步微调该监督模型。我们将生成的模型称为 InstructGPT。在对我们的提示分布的人工评估中，1.3B 参数 InstructGPT 模型的输出优于 175B GPT-3 的输出，尽管参数少 100 倍。此外，InstructGPT 模型显示了真实性的提高和有毒输出生成的减少，同时对公共 NLP 数据集的性能回归最小。尽管 InstructGPT 仍然会犯一些简单的错误，但我们的结果表明，根据人类反馈进行微调是使语言模型与人类意图保持一致的一个有前途的方向。
- **重点：0.0.2.6/7中探索的技术终于和GPT-3进行了对齐！  尽管参数少了 100 多倍，但我们的标签制作者更喜欢1.3B InstructGPT模型的输出，而不是175BGPT-3模型的输出。**



###### 0.1.1.7 [GPT-4](https://openai.com/research/gpt-4) (openai 2023.3.14)

- 论文地址：https://cdn.openai.com/papers/gpt-4.pdf
- Blog：https://openai.com/research/gpt-4
- 摘要翻译：我们报告了 GPT-4 的开发，这是一种大规模的多模式模型，可以接受图像和文本输入并产生文本输出。 虽然在许多现实场景中的能力不如人类，但 GPT-4 在各种专业和学术基准上表现出人类水平的表现，包括通过模拟律师考试，得分在应试者的前 10% 左右。 GPT-4 是一种基于 Transformer 的模型，经过预训练可以预测文档中的下一个标记。 培训后的对齐过程会提高真实性和遵守所需行为的措施的性能。 该项目的核心组成部分是开发可在广泛范围内表现可预测的基础设施和优化方法。 这使我们能够根据使用不超过 GPT-4 计算量的 1/1000 分之一训练的模型准确预测 GPT-4 性能的某些方面。





### 1. 后ChatGPT时代 可能有帮助的论文(持续更新)

#### 1.0 大型语言模型编码临床知识

- 论文地址：https://arxiv.org/abs/2212.13138

- 摘要翻译：大型语言模型 (LLM) 在自然语言理解和生成方面展示了令人印象深刻的能力，但医疗和临床应用的质量标准很高。如今，评估模型临床知识的尝试通常依赖于对有限基准的自动评估。没有标准来评估跨任务范围的模型预测和推理。为了解决这个问题，我们提出了 MultiMedQA，这是一个基准，它结合了六个现有的开放式问答数据集，涵盖专业医学检查、研究和消费者查询；和 HealthSearchQA，一个新的在线搜索医学问题的自由回答数据集。我们提出了一个框架，用于沿多个轴对模型答案进行人工评估，包括真实性、精确性、可能的危害和偏见。此外，我们在 MultiMedQA 上评估 PaLM（一个 5400 亿参数的 LLM）及其指令调整变体 Flan-PaLM。通过结合提示策略，Flan-PaLM 在每个 MultiMedQA 多项选择数据集（MedQA、MedMCQA、PubMedQA、MMLU 临床主题）上实现了最先进的准确率，包括 67.6% 在 MedQA（美国医学执照考试问题）上的准确率)，比之前的最先进技术高出 17% 以上。然而，人类评估揭示了 Flan-PaLM 响应中的关键差距。为了解决这个问题，我们引入了指令提示调整，这是一种使用一些示例将 LLM 与新域对齐的参数高效方法。由此产生的模型 Med-PaLM 表现令人鼓舞，但仍然不如临床医生。我们表明，理解、知识回忆和医学推理随着模型规模和指令提示调整而提高，表明法学硕士在医学中的潜在效用。我们的人类评估揭示了当今模型的重要局限性，强化了评估框架和方法开发在为临床应用创建安全、有用的 LLM 模型方面的重要性。

#### 1.1 **ChatGPT在USMLE上的表现**：使用大型语言模型进行 AI 辅助医学教育的潜力

- 论文地址：https://journals.plos.org/digitalhealth/article?id=10.1371/journal.pdig.0000198
- 摘要翻译：我们评估了名为 ChatGPT 的大型语言模型在美国医学执照考试 (USMLE) 上的表现，该考试由三门考试组成：Step1、Step2CK 和 Step3。 ChatGPT 在所有三项考试中的表现均达到或接近通过门槛，无需任何专门培训或强化。 此外，ChatGPT 在其解释中表现出高度的一致性和洞察力。 这些结果表明，大型语言模型可能有助于医学教育，并可能有助于临床决策。

#### 1.2 对 **ChatGPT 的医疗建议进行（图灵）测试**

- 论文地址：https://arxiv.org/abs/2301.10035
- 摘要翻译：目标：评估使用 ChatGPT 或类似的基于 AI 的聊天机器人进行患者与提供者沟通的可行性。 参与者：美国代表性样本 430 名年龄在 18 岁及以上的研究参与者。53.2% 的受访者为女性； 他们的平均年龄是47.1岁。 曝光：从 EHR 中提取了 10 个具有代表性的非管理性患者-提供者交互。 患者的问题被放置在 ChatGPT 中，要求聊天机器人使用与人类提供者的回答大致相同的字数来回答。 在调查中，每个患者的问题之后都会有提供者或 ChatGPT 生成的回复。 参与者被告知有五个响应是由提供者生成的，五个是由聊天机器人生成的。 参与者被要求并在经济上受到激励，以正确识别响应源。 参与者还被问及他们对聊天机器人在患者与提供者沟通中的功能的信任，使用李克特量表 1-5。 结果：不同问题的回答正确分类在49.0%到85.7%之间。 平均而言，聊天机器人响应在 65.5% 的时间内被正确识别，供应商响应在 65.1% 的时间内被正确识别。 平均而言，患者对聊天机器人功能的信任度反应较弱（李克特平均得分：3.4），随着问题任务的健康相关复杂性增加，信任度降低。 结论：ChatGPT 对患者问题的回答与提供者的回答难以区分。 外行似乎相信使用聊天机器人来回答风险较低的健康问题。

#### 1.3 **Toolformer**：语言模型可以自学使用工具

- 论文地址：https://arxiv.org/abs/2302.04761
- 摘要翻译：语言模型 (LM) 表现出非凡的能力，可以仅通过几个示例或文本指令来解决新任务，尤其是在规模上。 矛盾的是，它们还在基本功能上苦苦挣扎，例如算术或事实查找，而在这些功能中，更简单、更小的模型更胜一筹。 在本文中，我们展示了 LM 可以通过简单的 API 自学使用外部工具并实现两全其美。 我们介绍了 Toolformer，这是一个经过训练的模型，可以决定调用哪些 API、何时调用它们、传递哪些参数，以及如何最好地将结果纳入未来的代币预测。 这是以自我监督的方式完成的，只需要对每个 API 进行少量演示。 我们整合了一系列工具，包括计算器、问答系统、两个不同的搜索引擎、翻译系统和日历。 Toolformer 在各种下游任务中实现了显着改进的零样本性能，通常与更大的模型竞争，而不会牺牲其核心语言建模能力。

#### 1.4 检查你的事实并再试一次：**利用外部知识和自动反馈改进大型语言模型**

- 论文地址：https://arxiv.org/abs/2302.12813
- 摘要翻译：大型语言模型 (LLM)，例如 ChatGPT，能够为许多下游任务生成类似人类的流畅响应，例如面向任务的对话和问答。 然而，将 LLM 应用于现实世界的关键任务应用程序仍然具有挑战性，主要是因为它们倾向于产生幻觉并且无法使用外部知识。 本文提出了一个 LLM-Augmenter 系统，它使用一组即插即用模块来增强黑盒 LLM。 我们的系统使 LLM 生成基于外部知识的响应，例如存储在任务特定的数据库中。 它还迭代地修改 LLM 提示，以使用实用函数生成的反馈改进模型响应，例如LLM 生成的响应的真实性分数。 LLM-Augmenter 的有效性在两种类型的场景中得到了实证验证，即面向任务的对话和开放域问答。 LLM-Augmenter 在不牺牲其响应的流畅性和信息量的情况下显着减少了 ChatGPT 的幻觉。 我们公开提供源代码和模型。

#### 1.5  GPT-4 在医学挑战问题上的能力

- 论文地址：https://arxiv.org/abs/2303.13375
- 摘要翻译：大型语言模型 (LLM) 在包括医学在内的各个领域展示了自然语言理解和生成方面的卓越能力。我们对 GPT-4（一种最先进的 LLM）在医学能力考试和基准数据集上进行了全面评估。GPT-4 是一种通用模型，它不是专门用于通过训练解决医学问题，也不是为解决临床任务而设计的。我们的分析涵盖了 USMLE 的两套官方实践材料，USMLE 是一个三步考试程序，用于评估美国的临床能力和授予执照。我们还评估了 MultiMedQA 基准数据集套件的性能。除了测量模型性能外，还进行了实验以研究包含文本和图像的测试问题对模型性能的影响，探索训练期间对内容的记忆，并研究概率校准，这在医学等高风险应用中至关重要。我们的结果表明，在没有任何专门提示制作的情况下，GPT-4 比 USMLE 的及格分数高出 20 多分，并且优于早期的通用模型 (GPT-3.5) 以及专门针对医学知识进行微调的模型 (Med- PaLM，Flan-PaLM 540B 的快速调整版本）。此外，GPT-4 的校准明显好于 GPT-3.5，表明预测其答案正确可能性的能力大大提高。我们还通过一个案例研究定性地探索了模型的行为，该案例研究展示了 GPT-4 解释医学推理、向学生提供个性化解释的能力，并围绕医疗案例交互式地设计新的反事实场景。讨论了这些发现对 GPT-4 在医学教育、评估和临床实践中的潜在用途的影响，并适当关注准确性和安全性方面的挑战。

### 2 综述类文章

#### 1.生物医学领域的预训练语言模型：系统调查

- 论文地址：https://arxiv.org/abs/2110.05006
- 预训练语言模型 (PLM) 已成为大多数自然语言处理 (NLP) 任务的实际范例。 这也有利于生物医学领域：来自信息学、医学和计算机科学 (CS) 社区的研究人员提出了在生物医学数据集上训练的各种 PLM，例如，用于各种生物医学任务的生物医学文本、电子健康记录、蛋白质和 DNA 序列。 然而，生物医学PLM的跨学科特性阻碍了其在社区间的传播； 一些现有的作品相互孤立，没有进行全面的比较和讨论。 它期望一项调查不仅能系统地回顾生物医学 PLM 及其应用的最新进展，还能使术语和基准标准化。 在本文中，我们总结了预训练语言模型在生物医学领域的最新进展及其在生物医学下游任务中的应用。 特别是，我们讨论了动机并提出了现有生物医学 PLM 的分类法。 详尽讨论了它们在生物医学下游任务中的应用。 最后，我们阐述了各种局限性和未来趋势，希望能为研究界的未来研究提供启发。

#### 2.医疗保健深度学习指南

-  [论文地址 ](https://www.nature.com/articles/s41591-018-0316-z)   nature medicine发表的综述  
- 摘要翻译：在这里，我们介绍了用于医疗保健的深度学习技术，重点讨论了计算机视觉、自然语言处理、强化学习和通用方法中的深度学习。 我们描述了这些计算技术如何影响医学的几个关键领域，并探索如何构建端到端系统。 我们对计算机视觉的讨论主要集中在医学成像上，我们描述了自然语言处理在电子健康记录数据等领域的应用。 同样，在机器人辅助手术的背景下讨论了强化学习，并回顾了用于基因组学的广义深度学习方法。









### 3. 2021前仓库论文总结存档

#### 3.1 电子病历相关文章

**Transfer Learning from Medical Literature for Section Prediction in Electronic Health Records**

[论文地址](https://www.aclweb.org/anthology/D19-1492/)

论文概要：发表于EMNLP2019。基于少量in-domain数据和大量out-of-domain数据进行EHR相关的迁移学习。

论文摘要：sections such as Assessment and Plan, So- cial History, and Medications. These sec- tions help physicians find information easily and can be used by an information retrieval system to return specific information sought by a user. However, it is common that the exact format of sections in a particular EHR does not adhere to known patterns. There- fore, being able to predict sections and headers in EHRs automatically is beneficial to physi- cians. Prior approaches in EHR section pre- diction have only used text data from EHRs and have required significant manual annota- tion. We propose using sections from med- ical literature (e.g., textbooks, journals, web content) that contain content similar to that found in EHR sections. Our approach uses data from a different kind of source where la- bels are provided without the need of a time- consuming annotation effort. We use this data to train two models: an RNN and a BERT- based model. We apply the learned models along with source data via transfer learning to predict sections in EHRs. Our results show that medical literature can provide helpful su- pervision signal for this classification task.

**MUFASA: Multimodal Fusion Architecture Search for Electronic Health Records**

[论文地址](http://arxiv-download.xixiaoyao.cn/pdf/2102.02340.pdf)

论文概要:发表于AAAI2021。

论文摘要:One important challenge of applying deep learning to electronic health records (EHR) is the complexity of their multimodal structure. EHR usually contains a mixture of structured (codes) and unstructured (free-text) data with sparse and irregular longitudinal features – all of which doctors utilize when making decisions. In the deep learning regime, determining how different modality representations should be fused together is a difficult problem, which is often addressed by handcrafted modeling and intuition. In this work, we extend state-of-the-art neural architecture search (NAS) methods and propose MUltimodal Fusion Architecture SeArch (MUFASA) to simultaneously search across multimodal fusion strategies and modality-specific architectures for the first time. We demonstrate empirically that our MUFASA method outperforms established unimodal NAS on public EHR data with comparable computation costs. In addition, MUFASA produces architectures that outperform Transformer and Evolved Transformer. Compared with these baselines on CCS diagnosis code prediction, our discovered models improve top-5 recall from 0.88 to 0.91 and demonstrate the ability to generalize to other EHR tasks. Studying our top architecture in depth, we provide empirical evidence that MUFASA’s improvements are derived from its ability to both customize modeling for each data modality and find effective fusion strategies.




#### 3.2 医学关系抽取

**Leveraging Dependency Forest for Neural Medical Relation Extraction**

[论文地址](https://www.aclweb.org/anthology/D19-1020/)

论文概要：发表于EMNLP 2019. 基于dependency forest方法，提升对医学语句中依存关系的召回率，同时引进了一部分噪声，基于图循环网络进行特征提取，提供了在医疗关系抽取中使用依存关系，同时减少误差传递的一种思路。

论文摘要：Medical relation extraction discovers relations between entity mentions in text, such as research articles. For this task, dependency syntax has been recognized as a crucial source of features. Yet in the medical domain, 1-best parse trees suffer from relatively low accuracies, diminishing their usefulness. We investigate a method to alleviate this problem by utilizing dependency forests. Forests contain more than one possible decisions and therefore have higher recall but more noise compared with 1-best outputs. A graph neural network is used to represent the forests, automatically distinguishing the useful syntactic information from parsing noise. Results on two benchmarks show that our method outperforms the standard tree-based methods, giving the state-of-the-art results in the literature.

#### 3.3 医学知识图谱

**Learning a Health Knowledge Graph from Electronic Medical Records**

[论文地址](https://www.nature.com/articles/s41598-017-05778-z)

论文概要：发表于nature scientificreports（2017）. 基于27万余份电子病历构建的疾病-症状知识图谱。

论文摘要：Demand for clinical decision support systems in medicine and self-diagnostic symptom checkers has substantially increased in recent years. Existing platforms rely on knowledge bases manually compiled through a labor-intensive process or automatically derived using simple pairwise statistics. This study explored an automated process to learn high quality knowledge bases linking diseases and symptoms directly from electronic medical records. Medical concepts were extracted from 273,174 de-identified patient records and maximum likelihood estimation of three probabilistic models was used to automatically construct knowledge graphs: logistic regression, naive Bayes classifier and a Bayesian network using noisy OR gates. A graph of disease-symptom relationships was elicited from the learned parameters and the constructed knowledge graphs were evaluated and validated, with permission, against Google’s manually-constructed knowledge graph and against expert physician opinions. Our study shows that direct and automated construction of high quality health knowledge graphs from medical records using rudimentary concept extraction is feasible. The noisy OR model produces a high quality knowledge graph reaching precision of 0.85 for a recall of 0.6 in the clinical evaluation. Noisy OR significantly outperforms all tested models across evaluation frameworks (p < 0.01).

#### 3.4 辅助诊断

**Evaluation and accurate diagnoses of pediatric diseases using artificial intelligence**

[论文地址](https://www.nature.com/articles/s41591-018-0335-9)

论文概要：该文章由广州市妇女儿童医疗中心与依图医疗等企业和科研机构共同完成，基于机器学习的自然语言处理（NLP）技术实现不输人类医生的强大诊断能力，并具备多场景的应用能力。据介绍，这是全球首次在顶级医学杂志发表有关自然语言处理（NLP）技术基于电子健康记录（EHR）做临床智能诊断的研究成果，也是利用人工智能技术诊断儿科疾病的重磅科研成果。

论文摘要：Artificial intelligence (AI)-based methods have emerged as powerful tools to transform medical care. Although machine learning classifiers (MLCs) have already demonstrated strong performance in image-based diagnoses, analysis of diverse and massive electronic health record (EHR) data remains challenging. Here, we show that MLCs can query EHRs in a manner similar to the hypothetico-deductive reasoning used by physicians and unearth associations that previous statistical methods have not found. Our model applies an automated natural language processing system using deep learning techniques to extract clinically relevant information from EHRs. In total, 101.6 million data points from 1,362,559 pediatric patient visits presenting to a major referral center were analyzed to train and validate the framework. Our model demonstrates high diagnostic accuracy across multiple organ systems and is comparable to experienced pediatricians in diagnosing common childhood diseases. Our study provides a proof of concept for implementing an AI-based system as a means to aid physicians in tackling large amounts of data, augmenting diagnostic evaluations, and to provide clinical decision support in cases of diagnostic uncertainty or complexity. Although this impact may be most evident in areas where healthcare providers are in relative shortage, the benefits of such an AI system are likely to be universal.

#### 3.5 ACL2020医学领域相关论文列表

**A Generate-and-Rank Framework with Semantic Type Regularization for Biomedical Concept Normalization**

[论文地址](https://www.aclweb.org/anthology/2020.acl-main.748/)

**Biomedical Entity Representations with Synonym Marginalization**

[论文地址](https://www.aclweb.org/anthology/2020.acl-main.335/)

**Document Translation vs. Query Translation for Cross-Lingual Information Retrieval in the Medical Domain**

[论文地址](https://www.aclweb.org/anthology/2020.acl-main.613/)

**MIE: A Medical Information Extractor towards Medical Dialogues**

[论文地址](https://www.aclweb.org/anthology/2020.acl-main.576/)

**Rationalizing Medical Relation Prediction from Corpus-level Statistics**

[论文地址](https://www.aclweb.org/anthology/2020.acl-main.719/)

#### 3.6 医疗实体Linking（标准化）

**Medical Entity Linking using Triplet Network**

[论文地址](https://www.aclweb.org/anthology/W19-1912/)

论文概要： 发表于ACL2019,论文内容为疾病实体Linking研究。使用三元组数据，（mention，正例，负例），目标使distance(mention,负例)-distance(mention,正例)>alpha（人脸识别的经典方案）,具体损失函数参看论文。论文主要包括两部分内容1）候选数据集生成,对给定mention，与标准疾病集合数据（标准词及同义词）计算余弦相似度及Jaccard overlap分数,取topK作为候选样例。 2）网络结构基于Triplet Network。详见论文。

**A Generate-and-Rank Framework with Semantic Type Regularization for Biomedical Concept Normalization**

[论文地址](https://www.aclweb.org/anthology/2020.acl-main.748.pdf)

论文概要: 发表于ACL2020。基于list-wise排序学习方法。主要分为两部分：后续数据集生成 和  基于BERT的list-wise排序。较新颖的思路：1）在样本生成过程中，对标准词进行了基于同义词的扩展。2）在loss中引入了语义类型正则化。详见论文。

**Deep Neural Models for Medical Concept Normalization in User-Generated Texts**

[论文地址](https://www.aclweb.org/anthology/P19-2055.pdf)


#### 3.7 AAAI2020 医学NLP相关论文列表

**On the Generation of Medical Question-Answer Pairs**

[论文地址](https://arxiv.org/pdf/1811.00681.pdf)

**LATTE: Latent Type Modeling for Biomedical Entity Linking**

[论文地址](https://arxiv.org/pdf/1911.09787.pdf)

**Learning Conceptual-Contextual Embeddings for Medical Text**

[论文地址](https://arxiv.org/pdf/1908.06203.pdf)

**Understanding Medical Conversations with Scattered Keyword Attention and Weak Supervision from Responses**

[论文地址](http://ir.hit.edu.cn/~car/papers/AAAI2020-Shi-medconv.pdf)

**Simultaneously Linking Entities and Extracting Relations from Biomedical Text without Mention-level Supervision**

[论文地址](https://arxiv.org/pdf/1912.01070.pdf)

**Can Embeddings Adequately Represent Medical Terminology? New Large-Scale Medical Term Similarity Datasets Have the Answer!**

[论文地址](https://arxiv.org/pdf/2003.11082.pdf)

#### 3.8 EMNLP2020 医学NLP相关论文列表

**Towards Medical Machine Reading Comprehension with Structural Knowledge and Plain Text**

[论文地址](https://www.aclweb.org/anthology/2020.emnlp-main.111.pdf)

**MedDialog: Large-scale Medical Dialogue Datasets**

[论文地址](https://www.aclweb.org/anthology/2020.emnlp-main.743.pdf)

**COMETA: A Corpus for Medical Entity Linking in the Social Media**

[论文地址](https://www.aclweb.org/anthology/2020.emnlp-main.253.pdf)

**Biomedical Event Extraction as Sequence Labeling**

[论文地址](https://www.aclweb.org/anthology/2020.emnlp-main.431.pdf)

**FedED: Federated Learning via Ensemble Distillation for Medical Relation Extraction**

[论文地址](https://www.aclweb.org/anthology/2020.emnlp-main.165.pdf)

[论文解析:FedED:用于医学关系提取的联邦学习(基于融合蒸馏)](https://blog.csdn.net/lrs1353281004/article/details/111877017)

**Infusing Disease Knowledge into BERT for Health Question Answering, Medical Inference and Disease Name Recognition**

[论文地址](https://arxiv.org/pdf/2010.03746.pdf)

**A Knowledge-driven Generative Model for Multi-implication Chinese Medical Procedure Entity Normalization**

[论文地址](https://www.aclweb.org/anthology/2020.emnlp-main.116.pdf)

**BioMegatron: Larger Biomedical Domain Language Model**

[论文地址](https://www.aclweb.org/anthology/2020.emnlp-main.379.pdf)

**Querying Across Genres for Medical Claims in News**

[论文地址](https://www.aclweb.org/anthology/2020.emnlp-main.139.pdf)





## 6. 开源工具包

### 1. 分词工具：PKUSEG

- [项目地址](https://github.com/lancopku/pkuseg-python)
- 项目说明： 北京大学推出的多领域中文分词工具，支持选择医学领域。





## 7. 工业级产品解决方案

### 1. [灵医智慧](https://01.baidu.com/index.html)

### 2. [左手医生](https://open.zuoshouyisheng.com/)

### 3. [医渡云研究院-医学自然语言处理](https://www.yiducloud.com.cn/academy.html)

### 4. [百度-医学文本结构化](https://ai.baidu.com/solution/mtp)

### 5. [阿里云-医学自然语言处理](https://help.aliyun.com/document_detail/179395.html)





## 8. blog分享

### 1. 后ChatGPT时代 可能有帮助的博客(持续更新)

#### 1.1 [Alpaca：一个强大的开源指令跟随模型](https://crfm.stanford.edu/2023/03/13/alpaca.html)



### 2. 2021前仓库blog分享存档

#### 2.1 [医疗领域构建自然语言处理系统的经验教训](http://www.oreilly.com.cn/radar/?p=2083)

#### 2.2 [大数据时代的医学公共数据库与数据挖掘技术简介](https://mp.weixin.qq.com/s/tA44U4bJUttnROfrzpNYcQ)

#### 2.3 [从ACL 2021中看NLP在医疗领域应用的发展，附资源下载](https://mp.weixin.qq.com/s/RhcHvRWHRnYUg6u9vXoIGA)





## 9. 友情链接

### 1. [awesome_Chinese_medical_NLP](https://github.com/GanjinZero/awesome_Chinese_medical_NLP)

### 2. [中文NLP数据集搜索](https://www.cluebenchmarks.com/dataSet_search.html)

### 3. [medical-data(海量医疗相关数据)](https://github.com/beamandrew/medical-data)

### 4. [天池数据集(其中包含多个医疗NLP数据集)](https://tianchi.aliyun.com/dataset)

