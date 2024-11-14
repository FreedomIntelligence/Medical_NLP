# Medical_NLP

医疗NLP领域  评测/比赛，数据集，论文和预训练模型资源汇总。

Summary of medical NLP evaluations/competitions, datasets, papers and pre-trained models.

<p>
  <a href="https://github.com/FreedomIntelligence/Medical_NLP"><img src=https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg ></a>
  <a href="https://github.com/FreedomIntelligence/Medical_NLP"><img src=https://img.shields.io/github/forks/FreedomIntelligence/Medical_NLP.svg?style=social ></a>
  <a href="https://github.com/FreedomIntelligence/Medical_NLP"><img src=https://img.shields.io/github/stars/FreedomIntelligence/Medical_NLP.svg?style=social ></a>
  <a href="https://github.com/FreedomIntelligence/Medical_NLP"><img src=https://img.shields.io/github/watchers/FreedomIntelligence/Medical_NLP.svg?style=social ></a>
</p>

<!--
[中文版本](https://github.com/FreedomIntelligence/Chinese_medical_NLP)  [English_version](https://github.com/FreedomIntelligence/Chinese_medical_NLP/blob/master/English_vision.md)
-->

#### News

- 🟡*2024/11/14* 新增 [`4. VLM数据集`](#4-VLM数据集)、[`5.3 医疗VLM`](#53-医疗VLM)，**后续将重点维护 Medical VLM 方向相关资源汇总**，repo由[Rongsheng Wang](https://github.com/WangRongsheng)维护。
- 🟡*2024/11/14之前* 由于[Cris Lee](https://github.com/lrs1353281004)2021年离开医疗NLP领域，此repo现由[Xidong Wang](https://github.com/wangxidong06), [Ziyue Lin](https://github.com/RobinLin2002), [Jing Tang](https://github.com/vaew)继续维护。

#### Contents

[Medical_NLP](#medical_nlp)

* [1. 评测](#1-评测)
  * [1.1  中文医疗基准测评：CMB / CMExam / PromptCBLUE](#11--中文医疗基准测评cmb--cmexam--promptcblue)
  * [1.2  英文医疗基准测评:](#12--英文医疗基准测评)
* [2. 比赛](#2-比赛)
  * [2.1 正在进行的比赛](#21-正在进行的比赛)
  * [2.2 已经结束的比赛](#22-已经结束的比赛)
* [3. LLM 数据集](#3-LLM数据集)
  * [3.1 中文](#31-中文)
  * [3.2 英文](#32-英文)
* [4. VLM 数据集](#4-VLM数据集)
  * [4.1 中文](#41-中文)
  * [4.2 英文](#42-英文)
* [5. 开源预训练模型](#5-开源预训练模型)
  * [5.1 医疗PLM](#51-医疗PLM)
  * [5.2 医疗LLM](#52-医疗LLM)
  * [5.3 医疗VLM](#53-医疗VLM)
* [6. 相关论文](#6-相关论文)
  * [6.1 后ChatGPT时代 可能有帮助的论文](#61-后chatgpt时代-可能有帮助的论文)
  * [6.2 综述类文章](#62-综述类文章)
  * [6.3 特定任务文章](#63-特定任务文章)
  * [6.4 会议索引](#64-会议索引)
* [7. 开源工具包](#7-开源工具包)
* [8. 工业级产品解决方案](#8-工业级产品解决方案)
* [9. blog分享](#9-blog分享)
* [10. 友情链接](#10-友情链接) 



## 1. 评测

### 1.1  中文医疗基准测评：CMB / CMExam / PromptCBLUE 

* CMB

  * 地址：https://github.com/FreedomIntelligence/CMB
    ![](https://img.shields.io/github/stars/FreedomIntelligence/CMB)
  * 来源：各个临床医学工种各阶段考试；临床复杂病例问诊
* CMExam

  * 地址：https://github.com/williamliujl/CMExam
    ![](https://img.shields.io/github/stars/williamliujl/CMExam)
  * 来源：执业医师资格考试往年题
* PromptCBLUE
  * 地址：https://github.com/michael-wzhu/PromptCBLUE
    ![](https://img.shields.io/github/stars/michael-wzhu/PromptCBLUE)
  * 来源：CBLUE
* PromptCBLUE
  * 地址：https://github.com/CBLUEbenchmark/CBLUE
    ![](https://img.shields.io/github/stars/CBLUEbenchmark/CBLUE)
  * 来源：CHIP会议往届的学术评测比赛和阿里夸克医疗搜索业务的数据集组成
* MedBench
  * 地址：https://arxiv.org/abs/2312.12806
  * 来源：包含来自执医考试和报告的40,041个问题，覆盖各个专科。

### 1.2  英文医疗基准测评: 

* MultiMedBench

  * 简介：是一种源自Google的大型多模态生成模型


<div align="right">
    <b><a href="#Contents">↥ back to top</a></b>
</div>


## 2. 比赛

### 2.1 正在进行的比赛

* 医学搜索Query相关性判断
  
  * 地址：https://tianchi.aliyun.com/competition/entrance/532001/introduction
  * 来源：阿里天池


### 2.2 已经结束的比赛

#### 2.2.1 英文比赛

* BioNLP Workshop 2023 共享任务

  * 地址：https://aclweb.org/aclwiki/BioNLP_Workshop#SHARED_TASKS_2023
  * 来源：BioNLP Workshop
* MedVidQA 2023

  * 地址：https://medvidqa.github.io/index.html
  * 来源：美国国立卫生研究院
* MEDIQA-2021

  * 地址：https://sites.google.com/view/mediqa2021
  * 来源：NAACL-BioNLP 2021 workshop
* ICLR-2021-医疗对话生成与自动诊断国际竞赛

  * 地址：https://mlpcp21.github.io/pages/challenge
  * 来源：ICLR 2021 workshop

#### 2.2.2 中文比赛

* 影像学NLP —— 医学影像诊断报告生成

  * 地址：https://gaiic.caai.cn/ai2023/
  * 来源：2023全球人工智能技术创新大赛 赛道一
* 非标准化疾病诉求的简单分诊挑战赛2.0

  * 地址：http://challenge.xfyun.cn/topic/info?type=disease-claims-2022&ch=ds22-dw-sq03
  * 来源：科大讯飞
* 第八届中国健康信息处理大会(CHIP2022)测评任务

  * 地址：http://cips-chip.org.cn/
  * 来源：CHIP2022
* 科大讯飞-医疗实体及关系识别挑战赛

  * 地址：http://www.fudan-disc.com/sharedtask/imcs21/index.html
  * 来源：科大讯飞
    
* “肝”柔相济，大模型开创肝病医患交互服务新格局

  * 地址：http://www.fudan-disc.com/sharedtask/imcs21/index.html](https://www.dcic-china.com/competitions/10090
  * 来源：数字中国建设峰会组委会







## 3. LLM数据集

### 3.1 中文

* Huatuo-26M

  * 地址：https://github.com/FreedomIntelligence/Huatuo-26M
    ![](https://img.shields.io/github/stars/FreedomIntelligence/Huatuo-26M)
  * 简介：Huatuo-26M 是迄今为止最大的中医问答数据集。
* 中文医疗对话数据集

  * 地址：https://github.com/Toyhom/Chinese-medical-dialogue-data
    ![](https://img.shields.io/github/stars/Toyhom/Chinese-medical-dialogue-data)
  * 简介：包含六个科室的医学问答数据
* CBLUE

  * 地址：https://github.com/CBLUEbenchmark/CBLUE
    ![](https://img.shields.io/github/stars/CBLUEbenchmark/CBLUE)
  * 简介：涵盖了医学文本信息抽取（实体识别、关系抽取）
* cMedQA2 (108K)

  * 地址：https://github.com/zhangsheng93/cMedQA2
    ![](https://img.shields.io/github/stars/zhangsheng93/cMedQA2)
  * 简介：中文医药方面的问答数据集，超过10万条
* xywy-KG(294K三元组)

  * 地址：https://github.com/baiyang2464/chatbot-base-on-Knowledge-Graph
    ![](https://img.shields.io/github/stars/baiyang2464/chatbot-base-on-Knowledge-Graph)
  * 简介：44.1K实体 294.1K 三元组
* 39Health-KG (210K三元组)
  * 地址：https://github.com/zhihao-chen/QASystemOnMedicalGraph
    ![](https://img.shields.io/github/stars/zhihao-chen/QASystemOnMedicalGraph)
  * 简介：包括15项信息，其中7类实体，约3.7万实体，21万实体关系。
* Medical-Dialogue-System
  * 地址：https://github.com/UCSD-AI4H/Medical-Dialogue-System
    ![](https://img.shields.io/github/stars/UCSD-AI4H/Medical-Dialogue-System)
  * MedDialog 数据集（中文）包含医生和病人之间的对话（中文）。该数据集有 110 万条对话和 400 万条语句。数据还在不断增长，未来有更多的对话将被添加进来。
* Chinese medical dialogue data
  * 地址：https://github.com/Toyhom/Chinese-medical-dialogue-data
    ![](https://img.shields.io/github/stars/Toyhom/Chinese-medical-dialogue-data)
  * 该数据集含有包括男科，儿科，妇产科，内科，外科，肿瘤科在内的六个不同科室总计792099条数据。

* Yidu-S4K

  * 地址：http://openkg.cn/dataset/yidu-s4k
  * 简介：命名实体识别, 实体及属性抽取
* Yidu-N7K

  * 地址：http://openkg.cn/dataset/yidu-n7k
  * 简介：临床语标准化
* 中文医药方面的问答数据集

  * 地址：https://github.com/zhangsheng93/cMedQA2
  * 简介：医疗问答
* 中文医患问答对话数据

  * 地址：https://github.com/UCSD-AI4H/Medical-Dialogue-System
  * 简介：医疗问答
* CPubMed-KG (4.4M三元组)

  * 地址：https://cpubmed.openi.org.cn/graph/wiki
  * 简介：中华医学会高质量全文期刊数据
* 中文医学知识图谱 CMeKG (1M三元组)

  * 地址：http://cmekg.pcl.ac.cn/
  * 简介：CMeKG（Chinese Medical Knowledge  Graph）
* CHIP历年测评 (官方测评)
  * 地址：http://cips-chip.org.cn/2022/callforeval ;  http://www.cips-chip.org.cn/2021/ ;   http://cips-chip.org.cn/2020/
  * 简介：CHIP历年测评 (官方测评)
* 瑞金医院糖尿病数据集 (糖尿病)
  * 地址：https://tianchi.aliyun.com/competition/entrance/231687/information
  * 简介：瑞金医院糖尿病数据集 (糖尿病)
* 天池新冠肺炎问句匹配比赛 (新冠)
  * 地址：https://tianchi.aliyun.com/competition/entrance/231776/information
  * 简介：本次大赛数据包括：脱敏之后的医疗问题数据对和标注数据。

### 3.2 英文

- MedMentions

  * 地址：https://github.com/chanzuckerberg/MedMentions
    ![](https://img.shields.io/github/stars/chanzuckerberg/MedMentions)
  * 简介：基于Pubmed摘要的生物医学实体链接数据集
- webMedQA
  - 地址：https://github.com/hejunqing/webMedQA
    ![](https://img.shields.io/github/stars/hejunqing/webMedQA)
  - 简介：医疗问答
- COMETA

  * 地址：https://www.siphs.org/
  * 简介：社交媒体中的医疗实体链接数据。发表于EMNLP2020
- PubMedQA

  * 地址：https://arxiv.org/abs/1909.06146
  * 简介：基于Pubmed提取的医学问答数据集
- MediQA
  - 地址：https://sites.google.com/view/mediqa2021
  - 简介：文本概括
- ChatDoctor Dataset-1
  - 地址：https://drive.google.com/file/d/1lyfqIwlLSClhgrCutWuEe_IACNq6XNUt/view?usp=sharing
  - 简介：来自 HealthCareMagic.com 的 10 万条病人与医生之间的真实对话
- ChatDoctor Dataset-2
  - 地址：https://drive.google.com/file/d/1ZKbqgYqWc7DJHs3N9TQYQVPdDQmZaClA/view?usp=sharing
  - 简介：来自 icliniq.com 的 10k 条病人与医生之间的真实对话
- BioInstruct
  - 地址：https://github.com/bio-nlp/BioInstruct
  - 简介： 超过25,000条为生物医学任务量身定制的指令，包括但不限于问答（QA）、信息提取（IE）和文本生成
- Visual Med-Alpaca Data
  - 地址：https://github.com/cambridgeltl/visual-med-alpaca/tree/main/data
  - 简介：用于Visual Med-Alpaca训练的数据，源自 [BigBio](https://huggingface.co/bigbio), [ROCO](https://github.com/razorx89/roco-dataset) and [GPT-3.5-Turbo](https://chat.openai.com/chat)
- CheXpert Plus
  - 地址：https://github.com/Stanford-AIMI/chexpert-plus
  - 简介： 放射学领域公开发布的最大文本数据集，共有 3600 万个文本tokens，均配有 DICOM 格式的高质量图像，以及涵盖各种临床和社会群体的大量图像和患者元数据，以及许多病理标签和 RadGraph注释
  


## 4. VLM数据集


## 5. 开源预训练模型

### 5.1 医疗PLM

- BioBERT：

  * 地址：https://github.com/naver/biobert-pretrained 
    ![](https://img.shields.io/github/stars/naver/biobert-pretrained )
  * 简介：BioBERT是一种生物医学领域的语言表示模型，专门用于生物医学文本挖掘任务，如生物医学命名实体识别、关系提取、问答等。

* BlueBERT：

  * 地址：https://github.com/ncbi-nlp/BLUE_Benchmark
    ![](https://img.shields.io/github/stars/ncbi-nlp/BLUE_Benchmark)
  * 简介：BLUE基准包括5个不同的生物医学文本挖掘任务和10个语料库。BLUE基准依赖于预先存在的数据集，因为它们已被BioNLP社区广泛用作共享任务。这些任务涵盖了各种文本类型(生物医学文献和临床笔记)、数据集大小和难度，更重要的是，突出了常见的生物医学文本挖掘挑战。

* BioFLAIR：

  * 地址：https://github.com/flairNLP/flair
    ![](https://img.shields.io/github/stars/flairNLP/flair)
  * 简介：Flair是一个强大的NLP库，能将最先进的自然语言处理(NLP)模型应用于文本，例如命名实体识别(NER)，情感分析，词性标记(PoS)，对[生物医学数据](https://github.com/flairNLP/flair/blob/master/resources/docs/HUNFLAIR.md)的特殊支持，语义消歧和分类，支持快速增长的语言数量。Flair 还是一个文本嵌入库，一个基于PyTorch的自然语言处理框架。

* COVID-Twitter-BERT：

  * 地址：https://github.com/digitalepidemiologylab/covid-twitter-bert
    ![](https://img.shields.io/github/stars/digitalepidemiologylab/covid-twitter-bert)
  * 简介：COVID-Twitter-BERT（简称CT-BERT）是一种基于Transformer的模型，它在关于COVID-19主题的大量推特消息上进行了预训练。v2模型是在9700万条推文（12亿训练样本）上训练的。

* bio-lm (Biomedical and Clinical Language Models)

  * 地址：https://github.com/facebookresearch/bio-lm
    ![](https://img.shields.io/github/stars/facebookresearch/bio-lm)
  * 简介：这项工作评估了用于生物医学和临床自然语言处理任务的许多模型，并训练了一些性能更佳的新模型。

* BioALBERT

  * 地址：https://github.com/usmaann/BioALBERT
    ![](https://img.shields.io/github/stars/usmaann/BioALBERT)
  * 简介：这是一种针对大型领域特定(生物医学)语料库训练的生物医学语言表示模型，专为生物医学文本挖掘任务而设计。


### 5.2 医疗LLM 


#### 5.2.1 多语言医疗大模型

* ApolloMoE：
  * 地址：https://github.com/FreedomIntelligence/ApolloMoE
    ![](https://img.shields.io/github/stars/FreedomIntelligence/ApolloMoE)
  * 简介：通过语言家族专家的混合，有效地实现 50 种语言医学LLM的民主化
    
* Apollo：
  * 地址：https://github.com/FreedomIntelligence/Apollo
    ![](https://img.shields.io/github/stars/FreedomIntelligence/Apollo)
  * 简介：轻量级多语言医学LLM，将医疗人工智能普及到 60亿人群

* MMedLM：
  * 地址：https://github.com/MAGIC-AI4Med/MMedLM
    ![](https://img.shields.io/github/stars/MAGIC-AI4Med/MMedLM)
  * 简介：第一个开源的多语言医学语言模型

  
#### 5.2.2 中文医疗大语言模型

* BenTsao：
  * 地址：https://github.com/SCIR-HI/Huatuo-Llama-Med-Chinese
    ![](https://img.shields.io/github/stars/SCIR-HI/Huatuo-Llama-Med-Chinese)
  * 简介：BenTsao以LLaMA-7B为基础，经过中文医学指令精调/指令微调得到。研究人员通过医学知识图谱和GPT3.5 API构建了中文医学指令数据集，并在此基础上对LLaMA进行了指令微调，提高了LLaMA在医疗领域的问答效果。
* BianQue：
  * 地址：https://github.com/scutcyr/BianQue
    ![](https://img.shields.io/github/stars/scutcyr/BianQue)
  * 简介：一个经过指令与多轮问询对话联合微调的医疗对话大模型，以ClueAI/ChatYuan-large-v2作为底座，使用中文医疗问答指令与多轮问询对话混合数据集进行微调。
* SoulChat：
  * 地址：https://github.com/scutcyr/SoulChat
    ![](https://img.shields.io/github/stars/scutcyr/SoulChat)
  * 简介：灵心以ChatGLM-6B作为初始化模型，经过百万规模心理咨询领域中文长文本指令与多轮共情对话数据联合指令微调，提升模型的共情能力、引导用户倾诉能力以及提供合理建议的能力。
* DoctorGLM：
  * 地址：https://github.com/xionghonglin/DoctorGLM
    ![](https://img.shields.io/github/stars/xionghonglin/DoctorGLM)
  * 简介：一个基于 ChatGLM-6B的中文问诊大模型。该模型通过中文医疗对话数据集进行微调，实现了包括lora、p-tuningv2等微调及部署。
* HuatuoGPT：
  * 地址：https://github.com/FreedomIntelligence/HuatuoGPT
    ![](https://img.shields.io/github/stars/FreedomIntelligence/HuatuoGPT)
  * 简介：华佗GPT是一个经过中文医学指令精调/指令微调(Instruct-tuning)得到的一个GPT-like模型。该模型是专门为医疗咨询设计的中文LLM，它的训练数据包含了从ChatGPT处蒸馏得到的数据和来自医生的真实数据，在训练过程中加入了RLHF的反馈。
* HuatuoGPT-II：
  * 地址：https://github.com/FreedomIntelligence/HuatuoGPT-II
    ![](https://img.shields.io/github/stars/FreedomIntelligence/HuatuoGPT-II)
  * 简介：华佗GPT2采用了创新的领域适应方法，大大提高了其医学知识和对话能力。它在多个医疗基准测试中表现出了一流的性能，尤其是在专家评估和新医学执业资格考试中超越了 GPT-4。

#### 5.2.3 英文医疗大语言模型

* GatorTron：
  * 地址：https://github.com/uf-hobi-informatics-lab/GatorTron
    ![](https://img.shields.io/github/stars/uf-hobi-informatics-lab/GatorTron)
  * 简介：一个医疗健康领域的早期大模型，致力于研究使用非结构化的电子健康病例的系统是如何从有数十亿参数的医疗大模型中获益。
* Codex-Med：
  * 地址：https://github.com/vlievin/medical-reasoning
    ![](https://img.shields.io/github/stars/uf-hobi-informatics-lab/GatorTron)
  * 简介：致力于研究GPT-3.5模型回答和推理实际医疗问题的能力。使用了医疗测试数据集USMLE和MedMCQA， 医疗阅读理解数据集PubMedQA。
* Galactica：
  * 地址：https://galactica.org/
  * 简介：Galactica致力于解决科学领域的信息过载问题，储存合并了包括医疗医疗健康领域在内的科学知识。Galactica在大型论文语料库，参考文献的基础上训练而成，尝试发现不同领域研究之间的潜在关系。
* DeID-GPT：
  * 地址：https://github.com/yhydhx/ChatGPT-API
    ![](https://img.shields.io/github/stars/yhydhx/ChatGPT-API)
  * 简介：一个创新的的支持GPT4的去识别框架，可以自动识别和删除识别信息。
* ChatDoctor：
  * 地址：https://github.com/Kent0n-Li/ChatDoctor
    ![](https://img.shields.io/github/stars/Kent0n-Li/ChatDoctor)
  * 简介：一个利用医疗领域基础知识，基于LLaMA进行微调得到的医疗对话模型。
* MedAlpaca：
  * 地址：https://github.com/kbressem/medAlpaca
    ![](https://img.shields.io/github/stars/kbressem/medAlpaca)
  * 简介：MedAlpaca采用了一种开源策略，致力于解决医疗系统中的隐私问题。该模型基于70亿和130亿参数量的LLaMa构建。
* PMC-LLaMA：
  * 地址：https://github.com/chaoyi-wu/PMC-LLaMA
    ![](https://img.shields.io/github/stars/chaoyi-wu/PMC-LLaMA)
  * 简介： PMC-LLaMA是一个开源语言模型，通过对LLaMA-7B在总计480万篇生物医学学术论文上进行调质，进一步灌输医学知识，以增强其在医学领域的能力。
* Visual Med-Alpaca：
  * 地址：https://github.com/cambridgeltl/visual-med-alpaca
    ![](https://img.shields.io/github/stars/cambridgeltl/visual-med-alpaca)
  * 简介： Visual Med-Alpaca是一个开源的、参数高效的生物医学基础模型，可以与医学的“视觉专家”集成，用于多模式生物医学任务。该模型基于LLaMa-7B架构构建，使用由GPT-3.5-Turbo和人类专家共同策划的指令集进行训练。
* GatorTronGPT：
  * 地址：https://github.com/uf-hobi-informatics-lab/GatorTronGPT
    ![](https://img.shields.io/github/stars/uf-hobi-informatics-lab/GatorTronGPT)
  * 简介：GatorTronGPT 是一个医疗生成大语言模型。该模型基于GPT-3构建，含有50亿或200亿参数。该模型使用了含有2770亿单词的，由临床和英语文本组成的庞大语料库。
* MedAGI：
  * 地址：https://github.com/JoshuaChou2018/MedAGI
    ![](https://img.shields.io/github/stars/JoshuaChou2018/MedAGI)
  * 简介：MedAGI一个范例，以最低的成本将领域特定的医疗语言模型统一起来，为实现医疗通用人工智能提供了一条可能的途径。
* LLaVA-Med：
  * 地址：https://github.com/microsoft/LLaVA-Med
    ![](https://img.shields.io/github/stars/microsoft/LLaVA-Med)
  * 简介：LLaVA- med使用通用领域LLaVA进行初始化，然后以课程学习方式进行持续训练(首先是生物医学概念对齐，然后是全面的指令调整)。  
* Med-Flamingo：
  * 地址：https://github.com/snap-stanford/med-flamingo
    ![](https://img.shields.io/github/stars/snap-stanford/med-flamingo)
  * 简介：Med-Flamingo是一个视觉语言模型，专门设计用于处理包含图像和文本的交错多模态数据。以Flamingo为基础，Med-Flamingo通过对不同医学学科的多种多模式知识来源进行预训练，进一步增强了在这些医学领域的能力。

### 5.3 医疗VLM

## 6. 相关论文

### 6.1 后ChatGPT时代 可能有帮助的论文

1. 大型语言模型编码临床知识  论文地址：https://arxiv.org/abs/2212.13138

2. ChatGPT在USMLE上的表现：使用大型语言模型进行 AI 辅助医学教育的潜力  论文地址：https://journals.plos.org/digitalhealth/article?id=10.1371/journal.pdig.0000198

3. 对 ChatGPT 的医疗建议进行（图灵）测试  论文地址：https://arxiv.org/abs/2301.10035

4. Toolformer：语言模型可以自学使用工具  论文地址：https://arxiv.org/abs/2302.04761

5. 检查你的事实并再试一次：利用外部知识和自动反馈改进大型语言模型  论文地址：https://arxiv.org/abs/2302.12813

6. GPT-4 在医学挑战问题上的能力  论文地址：https://arxiv.org/abs/2303.13375


### 6.2 综述类文章

1. 生物医学领域的预训练语言模型：系统调查   [论文地址 ](https://arxiv.org/abs/2110.05006) 
2. 医疗保健深度学习指南  [论文地址 ](https://www.nature.com/articles/s41591-018-0316-z)   nature medicine发表的综述  
3. 医疗保健领域大语言模型综述    [论文地址 ](https://arxiv.org/abs/2310.05694) 

### 6.3 特定任务文章

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

### 6.4 会议索引

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





## 7. 开源工具包

1. 分词工具：PKUSEG [项目地址](https://github.com/lancopku/pkuseg-python)   项目说明： 北京大学推出的多领域中文分词工具，支持选择医学领域。





## 8. 工业级产品解决方案

1. [灵医智慧](https://01.baidu.com/index.html)

2. [左手医生](https://open.zuoshouyisheng.com/)

3. [医渡云研究院-医学自然语言处理](https://www.yiducloud.com.cn/academy.html)

4. [百度-医学文本结构化](https://ai.baidu.com/solution/mtp)

5. [阿里云-医学自然语言处理](https://help.aliyun.com/document_detail/179395.html)

   

## 9. blog分享

1. [Alpaca：一个强大的开源指令跟随模型](https://crfm.stanford.edu/2023/03/13/alpaca.html) 
2. [医疗领域构建自然语言处理系统的经验教训](http://www.oreilly.com.cn/radar/?p=2083)
3. [大数据时代的医学公共数据库与数据挖掘技术简介](https://mp.weixin.qq.com/s/tA44U4bJUttnROfrzpNYcQ)
4. [从ACL 2021中看NLP在医疗领域应用的发展，附资源下载](https://mp.weixin.qq.com/s/RhcHvRWHRnYUg6u9vXoIGA)



## 10. 友情链接

1.  [awesome_Chinese_medical_NLP](https://github.com/GanjinZero/awesome_Chinese_medical_NLP)
2.  [中文NLP数据集搜索](https://www.cluebenchmarks.com/dataSet_search.html)
3.  [medical-data(海量医疗相关数据)](https://github.com/beamandrew/medical-data)
4.  [天池数据集(其中包含多个医疗NLP数据集)](https://tianchi.aliyun.com/dataset)



## 11. reference


```bibtex
@misc{medical_NLP_github,
  author = {Xidong Wang, Ziyue Lin and Jing Tang},
  title = {Medical NLP},
  year = {2023},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/FreedomIntelligence/Medical_NLP}}
}
```
