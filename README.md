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
      * [5.1 OpenAI](#51-openai)
      * [5.2 后ChatGPT时代 可能有帮助的论文(持续更新)](#52-后chatgpt时代-可能有帮助的论文持续更新)
      * [5.3 综述类文章](#53-综述类文章)
      * [5.4 特定任务文章](#54-特定任务文章)
      * [5.4 会议索引](#54-会议索引)
   * [6. 开源工具包](#6-开源工具包)
   * [7. 工业级产品解决方案](#7-工业级产品解决方案)
   * [8. blog分享](#8-blog分享)
   * [9. 友情链接](#9-友情链接) 



## 1. 评测

### 1.1  中文医疗基准测评：CMB / CMExam / PromptCBLUE 

| 名称        | 来源                                                         | github地址                                  |
| ----------- | ------------------------------------------------------------ | ------------------------------------------- |
| CMB         | 各个临床医学工种各阶段考试；临床复杂病例问诊                 | https://github.com/FreedomIntelligence/CMB  |
| CMExam      | 执业医师资格考试往年题                                       | https://github.com/williamliujl/CMExam      |
| PromptCBLUE | CBLUE                                                        | https://github.com/michael-wzhu/PromptCBLUE |
| CBLUE       | CHIP会议往届的学术评测比赛和阿里夸克医疗搜索业务的数据集组成 | https://github.com/CBLUEbenchmark/CBLUE     |

### 1.2  英文医疗基准测评: 

| 名称          | 来源   | 介绍                     | github地址 | 官方测评网站地址 |
| ------------- | ------ | ------------------------ | ---------- | ---------------- |
| MultiMedBench | Google | 是一种大型多模态生成模型 |            |                  |



## 2. 比赛-

### 2.1 正在进行的比赛

暂无 欢迎补充~

### 2.2 已经结束的比赛

**英文**

| 名称                                     | 来源                        | 地址                                                         |
| ---------------------------------------- | --------------------------- | ------------------------------------------------------------ |
| BioNLP Workshop 2023 共享任务            | BioNLP Workshop             | https://aclweb.org/aclwiki/BioNLP_Workshop#SHARED_TASKS_2023 |
| MedVidQA 2023                            | 美国国立卫生研究院          | https://medvidqa.github.io/index.html                        |
| MEDIQA-2021                              | NAACL-BioNLP 2021 workshop. | https://sites.google.com/view/mediqa2021                     |
| ICLR-2021-医疗对话生成与自动诊断国际竞赛 | ICLR 2021 workshop          | https://mlpcp21.github.io/pages/challenge                    |

**中文**

| 名称                                         | 来源                                | 地址                                                         |
| -------------------------------------------- | ----------------------------------- | ------------------------------------------------------------ |
| 影像学NLP —— 医学影像诊断报告生成            | 2023全球人工智能技术创新大赛 赛道一 | https://gaiic.caai.cn/ai2023/                                |
| 非标准化疾病诉求的简单分诊挑战赛2.0          | 科大讯飞                            | http://challenge.xfyun.cn/topic/info?type=disease-claims-2022&ch=ds22-dw-sq03 |
| 第八届中国健康信息处理大会(CHIP2022)测评任务 | CHIP2022                            | http://cips-chip.org.cn/)                                    |
| 科大讯飞-医疗实体及关系识别挑战赛            | 科大讯飞                            | http://www.fudan-disc.com/sharedtask/imcs21/index.html       |



## 3. 数据集

### 3.1 中文

| 名称                              | 介绍                                                         | 地址                                                         |
| --------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Huatuo-26M                        | Huatuo-26M 是迄今为止最大的中医问答数据集。                  | https://github.com/FreedomIntelligence/Huatuo-26M            |
| Yidu-S4K                          | 命名实体识别,实体及属性抽取                                  | http://openkg.cn/dataset/yidu-s4k                            |
| Yidu-N7K                          | 临床语标准化                                                 | http://openkg.cn/dataset/yidu-n7k                            |
| 中文医药方面的问答数据集          | 医疗问答                                                     | https://github.com/zhangsheng93/cMedQA2                      |
| 中文医患问答对话数据              | 医疗问答                                                     | https://github.com/UCSD-AI4H/Medical-Dialogue-System         |
| 中文医疗对话数据集                | 包含六个科室的医学问答数据                                   | https://github.com/Toyhom/Chinese-medical-dialogue-data      |
| CPubMed-KG (4.4M三元组)           | 中华医学会高质量全文期刊数据                                 | https://cpubmed.openi.org.cn/graph/wiki                      |
| CBLUE                             | 涵盖了医学文本信息抽取（实体识别、关系抽取）                 | https://github.com/CBLUEbenchmark/CBLUE                      |
| 中文医学知识图谱 CMeKG (1M三元组) | CMeKG（Chinese Medical Knowledge  Graph）                    | http://cmekg.pcl.ac.cn/                                      |
| cMedQA2 (108K)                    | 中文医药方面的问答数据集，超过10万条。                       | https://github.com/zhangsheng93/cMedQA2                      |
| xywy-KG(294K三元组)               | 44.1K实体 294.1K 三元组                                      | https://github.com/baiyang2464/chatbot-base-on-Knowledge-Graph |
| 39Health-KG (210K三元组)          | 包括15项信息，其中7类实体，约3.7万实体，21万实体关系。       | https://github.com/zhihao-chen/QASystemOnMedicalGraph        |
| CHIP历年测评 (官方测评)           | CHIP历年测评 (官方测评)                                      | http://cips-chip.org.cn/2022/callforeval ;  http://www.cips-chip.org.cn/2021/ ;   http://cips-chip.org.cn/2020/ |
| 瑞金医院糖尿病数据集 (糖尿病)     | 通过糖尿病相关的教科书、研究论文来做糖尿病文献挖掘并构建糖尿病知识图谱 | https://tianchi.aliyun.com/competition/entrance/231687/information |
| 天池新冠肺炎问句匹配比赛 (新冠)   | 本次大赛数据包括：脱敏之后的医疗问题数据对和标注数据。       | https://tianchi.aliyun.com/competition/entrance/231776/information |

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

### 5.1 OpenAI

**openai RLHF+NLP之前 出现在RLHF领域的工作**

- 从轨迹偏好查询中学习政策的贝叶斯方法(NIPS 2012)  论文地址：https://papers.nips.cc/paper/2012/hash/16c222aa19898e5058938167c8ab6c57-Abstract.html
- 通过人类反馈训练机器人：案例研究(ICSR 2013) 论文地址：https://link.springer.com/chapter/10.1007/978-3-319-02675-6_46
- APRIL：基于主动偏好学习的强化学习(2012) 论文地址：https://arxiv.org/abs/1208.0984
- 通过反馈编程(2014)  论文地址：https://hal.inria.fr/hal-00980839

- 在 Atari 中从人类偏好和示范中进行奖励学习(2018) 论文地址：https://arxiv.org/abs/1811.06521

**openai RLHF思维链路**

1. 高效反馈(2015) Start from this [blog](https://ai-alignment.com/efficient-feedback-a347748b1557#.exjnsupts)！  地址：https://ai-alignment.com/efficient-feedback-a347748b1557#.exjnsupts
2.  [使用损坏的奖励渠道进行强化学习](https://openai.com/research/faulty-reward-functions)(2017.3 openai) openai对RL Policy安全性的考虑 4/5的尝试 论文地址：https://arxiv.org/abs/1705.08417   Blog: https://openai.com/research/faulty-reward-functions
3. [从人类偏好中深度强化学习](https://openai.com/research/learning-from-human-preferences)(2017.6 openai) RLHF in RL 初探  论文地址：https://arxiv.org/abs/1706.03741
4. [通过辩论提升人工智能安全](https://openai.com/research/debate) (2018.5 openai)  通过辩论 实现RL安全 解决2 论文地址：https://arxiv.org/abs/1805.00899

5. [通过放大弱专家来监督强学习者](https://openai.com/research/learning-complex-goals-with-iterated-amplification) (2018.10 openai)   迭代放大的 RL 安全技术 解决2 论文地址：https://arxiv.org/abs/1810.08575
6. [根据人类偏好微调语言模型]( https://openai.com/research/fine-tuning-gpt-2)(根据人类偏好微调 GPT-2) (2019 openai) First NLP+RLHF!  论文地址：https://arxiv.org/abs/1909.08593
7. [RLHF in 摘要生成](https://openai.com/research/learning-to-summarize-with-human-feedback)(openai 2020)  Second try NLP+RLHF! 论文地址：https://arxiv.org/abs/2009.01325
8. [TruthfulQA](https://openai.com/research/truthfulqa)：衡量模型如何模仿人类的谎言 (2021.8.9)  摘要最后一句话：最大的模型通常是最不真实的，我们建议单独扩大模型在提高真实性方面不如使用训练目标进行微调而不是模仿网络文本。   directly lead to 9  论文地址：https://arxiv.org/abs/2109.07958
9. [instruct GPT]( https://openai.com/research/instruction-following)(2022.1 openai)  0.0.2.6/7中探索的技术终于和GPT-3进行了对齐！  重点：尽管参数少了 100 多倍，但我们的标签制作者更喜欢1.3B InstructGPT模型的输出，而不是175BGPT-3模型的输出。 论文地址：https://arxiv.org/abs/2203.02155

**GPT-x 及其变体的迭代过程**

硬件资源和调度的迭代

1. [kubernetes](https://kubernetes.io/)
2. [将 Kubernetes 扩展到 2,500 个节点](https://openai.com/research/scaling-kubernetes-to-2500-nodes)  Blog地址：https://openai.com/research/scaling-kubernetes-to-2500-nodes
3. 将 [Kubernetes 扩展到 7,500 个节点](https://openai.com/research/scaling-kubernetes-to-7500-nodes) 为大型模型提供了可扩展的基础设施。同时也为神经语言模型的缩放定律等快速小规模迭代研究提供了基础设施。 Blog地址：https://openai.com/research/scaling-kubernetes-to-7500-nodes

模型的迭代

1. [GPT](https://openai.com/research/language-unsupervised)(2018.6.11 openai) 论文地址：https://cdn.openai.com/research-covers/language-unsupervised/language_understanding_paper.pdf
2. [GPT-2](https://openai.com/research/better-language-models)(2019.2.14 openai) 论文地址：https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf
3. [GPT-3: 语言模型是小样本学习者](https://openai.com/research/language-models-are-few-shot-learners) (2020.3.28 openai) 论文地址：https://arxiv.org/abs/2005.14165
4. [CLIP](https://openai.com/research/clip) 从自然语言监督中学习可迁移视觉模型(2021.1.5openai)  论文地址：https://arxiv.org/abs/2103.00020
5. [CodeX](https://openai.com/blog/openai-codex) 评估在代码上训练的大型语言模型 (2021.6.7 openai) 论文地址：https://arxiv.org/abs/2107.03374
6. [instruct GPT]( https://openai.com/research/instruction-following)(2022.6.27 openai)   论文地址：https://arxiv.org/abs/2203.02155
7. [GPT-4](https://openai.com/research/gpt-4) (openai 2023.3.14)  论文地址：https://cdn.openai.com/papers/gpt-4.pdf



### 5.2 后ChatGPT时代 可能有帮助的论文(持续更新)

1. 大型语言模型编码临床知识  论文地址：https://arxiv.org/abs/2212.13138

2. ChatGPT在USMLE上的表现：使用大型语言模型进行 AI 辅助医学教育的潜力  论文地址：https://journals.plos.org/digitalhealth/article?id=10.1371/journal.pdig.0000198

3. 对 ChatGPT 的医疗建议进行（图灵）测试  论文地址：https://arxiv.org/abs/2301.10035

4. Toolformer：语言模型可以自学使用工具  论文地址：https://arxiv.org/abs/2302.04761

5. 检查你的事实并再试一次：利用外部知识和自动反馈改进大型语言模型  论文地址：https://arxiv.org/abs/2302.12813

6. GPT-4 在医学挑战问题上的能力  论文地址：https://arxiv.org/abs/2303.13375

   

### 5.3 综述类文章

1. 生物医学领域的预训练语言模型：系统调查   论文地址：https://arxiv.org/abs/2110.05006
2. 医疗保健深度学习指南  [论文地址 ](https://www.nature.com/articles/s41591-018-0316-z)   nature medicine发表的综述  



### 5.4 特定任务文章

**电子病历相关文章**

1. Transfer Learning from Medical Literature for Section Prediction in Electronic Health Records   [论文地址](https://www.aclweb.org/anthology/D19-1492/)
2. MUFASA: Multimodal Fusion Architecture Search for Electronic Health Records [论文地址](http://arxiv-download.xixiaoyao.cn/pdf/2102.02340.pdf) 

**医学关系抽取**

1. Leveraging Dependency Forest for Neural Medical Relation Extraction [论文地址](https://www.aclweb.org/anthology/D19-1020/) 

**医学知识图谱**

1. Learning a Health Knowledge Graph from Electronic Medical Records [论文地址](https://www.nature.com/articles/s41598-017-05778-z)

**辅助诊断**

1. Evaluation and accurate diagnoses of pediatric diseases using artificial intelligence [论文地址](https://www.nature.com/articles/s41591-018-0335-9) 

**医疗实体Linking（标准化）**

1. Medical Entity Linking using Triplet Network  [论文地址](https://www.aclweb.org/anthology/W19-1912/)
2. A Generate-and-Rank Framework with Semantic Type Regularization for Biomedical Concept Normalization   [论文地址](https://www.aclweb.org/anthology/2020.acl-main.748.pdf)
3. Deep Neural Models for Medical Concept Normalization in User-Generated Texts  [论文地址](https://www.aclweb.org/anthology/P19-2055.pdf)



### 5.4 会议索引

**ACL2020医学领域相关论文列表**

1. A Generate-and-Rank Framework with Semantic Type Regularization for Biomedical Concept Normalization [论文地址](https://www.aclweb.org/anthology/2020.acl-main.748/)
2. Biomedical Entity Representations with Synonym Marginalization [论文地址](https://www.aclweb.org/anthology/2020.acl-main.335/)
3. Document Translation vs. Query Translation for Cross-Lingual Information Retrieval in the Medical Domain [论文地址](https://www.aclweb.org/anthology/2020.acl-main.613/)
4. MIE: A Medical Information Extractor towards Medical Dialogues [论文地址](https://www.aclweb.org/anthology/2020.acl-main.576/)
5. Rationalizing Medical Relation Prediction from Corpus-level Statistics  [论文地址](https://www.aclweb.org/anthology/2020.acl-main.719/) 

**AAAI2020 医学NLP相关论文列表**

1. On the Generation of Medical Question-Answer Pairs [论文地址](https://arxiv.org/pdf/1811.00681.pdf)
2. LATTE: Latent Type Modeling for Biomedical Entity Linking  [论文地址](https://arxiv.org/pdf/1911.09787.pdf)
3. Learning Conceptual-Contextual Embeddings for Medical Text [论文地址](https://arxiv.org/pdf/1908.06203.pdf)
4. Understanding Medical Conversations with Scattered Keyword Attention and Weak Supervision from Responses [论文地址](http://ir.hit.edu.cn/~car/papers/AAAI2020-Shi-medconv.pdf)
5. Simultaneously Linking Entities and Extracting Relations from Biomedical Text without Mention-level Supervision [论文地址](https://arxiv.org/pdf/1912.01070.pdf)
6. Can Embeddings Adequately Represent Medical Terminology? New Large-Scale Medical Term Similarity Datasets Have the Answer!   [论文地址](https://arxiv.org/pdf/2003.11082.pdf)

**EMNLP2020 医学NLP相关论文列表**

1. Towards Medical Machine Reading Comprehension with Structural Knowledge and Plain Text [论文地址](https://www.aclweb.org/anthology/2020.emnlp-main.111.pdf)
2. MedDialog: Large-scale Medical Dialogue Datasets [论文地址](https://www.aclweb.org/anthology/2020.emnlp-main.743.pdf)
3. COMETA: A Corpus for Medical Entity Linking in the Social Media  [论文地址](https://www.aclweb.org/anthology/2020.emnlp-main.253.pdf)
4. Biomedical Event Extraction as Sequence Labeling [论文地址](https://www.aclweb.org/anthology/2020.emnlp-main.431.pdf)
5. FedED: Federated Learning via Ensemble Distillation for Medical Relation Extraction [论文地址](https://www.aclweb.org/anthology/2020.emnlp-main.165.pdf)  [论文解析:FedED:用于医学关系提取的联邦学习(基于融合蒸馏)](https://blog.csdn.net/lrs1353281004/article/details/111877017)
6. Infusing Disease Knowledge into BERT for Health Question Answering, Medical Inference and Disease Name Recognition [论文地址](https://arxiv.org/pdf/2010.03746.pdf)
7. A Knowledge-driven Generative Model for Multi-implication Chinese Medical Procedure Entity Normalization [论文地址](https://www.aclweb.org/anthology/2020.emnlp-main.116.pdf)
8. BioMegatron: Larger Biomedical Domain Language Model [论文地址](https://www.aclweb.org/anthology/2020.emnlp-main.379.pdf)
9. Querying Across Genres for Medical Claims in News  [论文地址](https://www.aclweb.org/anthology/2020.emnlp-main.139.pdf)





## 6. 开源工具包

1. 分词工具：PKUSEG [项目地址](https://github.com/lancopku/pkuseg-python)   项目说明： 北京大学推出的多领域中文分词工具，支持选择医学领域。





## 7. 工业级产品解决方案

1. [灵医智慧](https://01.baidu.com/index.html)

2. [左手医生](https://open.zuoshouyisheng.com/)

3. [医渡云研究院-医学自然语言处理](https://www.yiducloud.com.cn/academy.html)

4. [百度-医学文本结构化](https://ai.baidu.com/solution/mtp)

5. [阿里云-医学自然语言处理](https://help.aliyun.com/document_detail/179395.html)

   

## 8. blog分享

1. [Alpaca：一个强大的开源指令跟随模型](https://crfm.stanford.edu/2023/03/13/alpaca.html) 
2. [医疗领域构建自然语言处理系统的经验教训](http://www.oreilly.com.cn/radar/?p=2083)
3. [大数据时代的医学公共数据库与数据挖掘技术简介](https://mp.weixin.qq.com/s/tA44U4bJUttnROfrzpNYcQ)
4. [从ACL 2021中看NLP在医疗领域应用的发展，附资源下载](https://mp.weixin.qq.com/s/RhcHvRWHRnYUg6u9vXoIGA)





## 9. 友情链接

1.  [awesome_Chinese_medical_NLP](https://github.com/GanjinZero/awesome_Chinese_medical_NLP)
2.  [中文NLP数据集搜索](https://www.cluebenchmarks.com/dataSet_search.html)
3. [medical-data(海量医疗相关数据)](https://github.com/beamandrew/medical-data)
4. [天池数据集(其中包含多个医疗NLP数据集)](https://tianchi.aliyun.com/dataset)


## 10. reference


```bibtex
@misc{medical_NLP_github,
  author = {Xidong Wang},
  title = {Medical NLP},
  year = {2023},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/FreedomIntelligence/Medical_NLP}}
}
```
