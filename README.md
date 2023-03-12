# Chinese_medical_NLP


>由于[Cris Lee](https://github.com/lrs1353281004)2021年离开医疗NLP领域，此repo现由[Xidong Wang](https://github.com/wangxidong06)继续维护。

医疗NLP领域  评测/比赛，数据集，论文和预训练模型资源汇总。

   * [Chinese_medical_NLP](#chinese_medical_nlp)
      * [一. 评测/比赛](#一-评测比赛)
         * [1. 正在进行的评测/比赛：](#1-正在进行的评测比赛)
            * [1.1 中文：影像学NLP —— 医学影像诊断报告生成](#11-中文影像学nlp--医学影像诊断报告生成)
            * [1.2 英文：BioNLP Workshop 2023 共享任务：](#12-英文bionlp-workshop-2023-共享任务)
            * [1.3 英文：MedVidQA 2023](#13-英文medvidqa-2023)
            * [1.4 中文 (长期有效)：医疗信息处理挑战榜CBLUE数据集](#14-中文-长期有效医疗信息处理挑战榜cblue数据集)
         * [2. 已结束的评测/比赛(从2021开始)：](#2-已结束的评测比赛从2021开始)
            * [2.1 中文：非标准化疾病诉求的简单分诊挑战赛2.0](#21-中文非标准化疾病诉求的简单分诊挑战赛20)
            * [2.2 中文：第八届中国健康信息处理大会(CHIP2022)测评任务](#22-中文第八届中国健康信息处理大会chip2022测评任务)
            * [2.3 中文：科大讯飞-医疗实体及关系识别挑战赛](#23-中文科大讯飞-医疗实体及关系识别挑战赛)
            * [2.4 中文：第一届智能对话诊疗评测比赛（CCL 2021）](#24-中文第一届智能对话诊疗评测比赛ccl-2021)
            * [2.5 英文：MEDIQA-2021](#25-英文mediqa-2021)
            * [2.6 英文： ICLR-2021-医疗对话生成与自动诊断国际竞赛](#26-英文-iclr-2021-医疗对话生成与自动诊断国际竞赛)
      * [二. 数据集](#二-数据集)
         * [1. 中文数据集](#1-中文数据集)
            * [1.1 中文医患问答对话数据 (1.1M)](#11-中文医患问答对话数据-11m)
            * [1.2 中文医疗对话数据集（792K）](#12-中文医疗对话数据集792k)
            * [1.3 CPubMed-KG (4.4M三元组)](#13-cpubmed-kg-44m三元组)
            * [1.4 CBLUE测评](#14-cblue测评)
            * [1.5 中文医学知识图谱 CMeKG (1M三元组)](#15-中文医学知识图谱-cmekg-1m三元组)
            * [1.6 cMedQA2 (108K)](#16-cmedqa2-108k)
            * [1.7 xywy-KG(294K三元组)](#17-xywy-kg294k三元组)
            * [1.8 39Health-KG (210K三元组)](#18-39health-kg-210k三元组)
            * [1.9 CHIP历年测评 (官方测评)](#19-chip历年测评-官方测评)
            * [1.10 瑞金医院糖尿病数据集 (糖尿病)](#110-瑞金医院糖尿病数据集-糖尿病)
            * [1.11 天池新冠肺炎问句匹配比赛 (新冠)](#111-天池新冠肺炎问句匹配比赛-新冠)
            * [2. 中国临床医生常用知识信息源](#2-中国临床医生常用知识信息源)
               * [2.1 pubMed](#21-pubmed)
               * [2.2 Up-to-date](#22-up-to-date)
               * [2.3 临床指南](#23-临床指南)
               * [2.4 用药助手](#24-用药助手)
               * [2.5 丁香园](#25-丁香园)
               * [2.6 丁香医生](#26-丁香医生)
         * [3. 英文数据集](#3-英文数据集)
            * [3.1 PubMedQA](#31-pubmedqa)
            * [3.2 COMETA](#32-cometa)
            * [3.3 MedMentions](#33-medmentions)
      * [三. 开源预训练模型](#三-开源预训练模型)
         * [1. 现有Medical NLP大型模型](#1-现有medical-nlp大型模型)
            * [1.1 BioMedLM (2.7B)](#11-biomedlm-27b)
            * [1.2 BioGPT  (1.5B)](#12-biogpt--15b)
            * [1.3 Medical-chatgpt](#13-medical-chatgpt)
            * [1.4 BioBERT](#14-biobert)
            * [1.5 PubMedBERT](#15-pubmedbert)
         * [2. 其他可供在医疗领域微调的中文大模型](#2-其他可供在医疗领域微调的中文大模型)
            * [2.1 Awesome List:](#21-awesome-list)
            * [2.2 0B-5B:](#22-0b-5b)
            * [2.3 5B-10B:](#23-5b-10b)
            * [2.4 10B-100B:](#24-10b-100b)
            * [2.5 100B--:](#25-100b--)
      * [四. 相关论文](#四-相关论文)
         * [1. 后ChatGPT时代 可能有帮助的论文(持续更新)](#1-后chatgpt时代-可能有帮助的论文持续更新)
         * [2. 2021前仓库论文总结存档](#2-2021前仓库论文总结存档)
            * [2.1 综述类文章](#21-综述类文章)
            * [2.2 电子病历相关文章](#22-电子病历相关文章)
            * [2.3 医学关系抽取](#23-医学关系抽取)
            * [2.4 医学知识图谱](#24-医学知识图谱)
            * [2.5 辅助诊断](#25-辅助诊断)
            * [2.6 ACL2020医学领域相关论文列表](#26-acl2020医学领域相关论文列表)
            * [2.7 医疗实体Linking（标准化）](#27-医疗实体linking标准化)
            * [2.8 AAAI2020 医学NLP相关论文列表](#28-aaai2020-医学nlp相关论文列表)
            * [2.9 EMNLP2020 医学NLP相关论文列表](#29-emnlp2020-医学nlp相关论文列表)
      * [五. 开源工具包](#五-开源工具包)
         * [5.1 分词工具：PKUSEG](#51-分词工具pkuseg)
      * [六. 工业级产品解决方案](#六-工业级产品解决方案)
         * [6.1 <a href="https://01.baidu.com/index.html" rel="nofollow">灵医智慧</a>](#61-灵医智慧)
         * [6.2 <a href="https://open.zuoshouyisheng.com/" rel="nofollow">左手医生</a>](#62-左手医生)
         * [6.3 <a href="https://www.yiducloud.com.cn/academy.html" rel="nofollow">医渡云研究院-医学自然语言处理</a>](#63-医渡云研究院-医学自然语言处理)
         * [6.4 <a href="https://ai.baidu.com/solution/mtp" rel="nofollow">百度-医学文本结构化</a>](#64-百度-医学文本结构化)
         * [6.5 <a href="https://help.aliyun.com/document_detail/179395.html" rel="nofollow">阿里云-医学自然语言处理</a>](#65-阿里云-医学自然语言处理)
      * [七. blog分享](#七-blog分享)
         * [7.1 <a href="http://www.oreilly.com.cn/radar/?p=2083" rel="nofollow">医疗领域构建自然语言处理系统的经验教训</a>](#71-医疗领域构建自然语言处理系统的经验教训)
         * [7.2 <a href="https://mp.weixin.qq.com/s/tA44U4bJUttnROfrzpNYcQ" rel="nofollow">大数据时代的医学公共数据库与数据挖掘技术简介</a>](#72-大数据时代的医学公共数据库与数据挖掘技术简介)
         * [7.3 <a href="https://mp.weixin.qq.com/s/RhcHvRWHRnYUg6u9vXoIGA" rel="nofollow">从ACL 2021中看NLP在医疗领域应用的发展，附资源下载</a>](#73-从acl-2021中看nlp在医疗领域应用的发展附资源下载)
      * [八. 友情链接](#八-友情链接)
         * [8.1 <a href="https://github.com/GanjinZero/awesome_Chinese_medical_NLP">awesome_Chinese_medical_NLP</a>](#81-awesome_chinese_medical_nlp)
         * [8.2 <a href="https://www.cluebenchmarks.com/dataSet_search.html" rel="nofollow">中文NLP数据集搜索</a>](#82-中文nlp数据集搜索)
         * [8.3 <a href="https://github.com/beamandrew/medical-data">medical-data(海量医疗相关数据)</a>](#83-medical-data海量医疗相关数据)
         * [8.4 <a href="https://tianchi.aliyun.com/dataset" rel="nofollow">天池数据集(其中包含多个医疗NLP数据集)</a>](#84-天池数据集其中包含多个医疗nlp数据集)

## 一. 评测/比赛

### 1. 正在进行的评测/比赛：

##### 1.1 中文：影像学NLP —— 医学影像诊断报告生成

- 来源：2023全球人工智能技术创新大赛 赛道一
- 介绍：本赛道任务要求参赛队伍根据医生对CT的影像描述文本数据（即对医学影像特征的描述），生成诊断报告文本。与传统文本生成任务不同的是，医学影像诊断报告内容具有专业性、明确性和离散性，因此也需要针对性的算法与模型设计。报告生成结果按照指定评价指标进行评测和排名，得分最优者获胜。
- [官方地址](https://gaiic.caai.cn/ai2023/) 

##### 1.2 英文：BioNLP Workshop 2023 共享任务：

[官方地址](https://aclweb.org/aclwiki/BioNLP_Workshop#SHARED_TASKS_2023)

- 1A：问题列表总结
  - 介绍：从电子健康记录中的日常护理笔记中自动总结患者的主要问题，有助于减轻临床医生的信息和认知超载，并通过床边的计算机化诊断决策支持提供增强智能。Problem List Summarization 的任务旨在使用住院期间提供者的进度记录输入生成患者日常护理计划中的诊断和问题列表。
  - [详细信息](https://physionet.org/content/bionlp-workshop-2023-task-1a/1.0.0/)
- 1B：放射学报告摘要
  - 介绍：放射学报告摘要的研究领域目前面临一个重要的局限性：大多数研究是在胸部X光片上进行的。为了减轻这些限制，我们提出了两个数据集：一个共享摘要任务，包括六种不同的模式和解剖结构，总共 79,779 个样本，基于 MIMIC-III 数据库。一项关于胸部 X 光放射学报告的共享摘要任务，其中包含斯坦福大学的图像和全新的域外测试集。
  - [详细信息](https://vilmedic.app/misc/bionlp23/sharedtask)
- 2：生物医学研究文章的外行摘要
  - 介绍：生物医学出版物包含与健康相关的突出主题的最新研究，从常见疾病到全球流行病。这通常会导致他们的内容引起广泛的受众兴趣，包括研究人员、医疗专业人员、记者，甚至公众。然而，此类文章中使用的高度技术性和专业性语言通常会使非专业观众难以理解其内容。因此，这些模型在经过训练以生成更具可读性、包含更多背景信息和更少技术术语（即“外行摘要”）的摘要时，有可能帮助扩大对高技术文档的访问。这项共同任务围绕生物医学研究文章的抽象总结，强调可控性和迎合非专家观众。
  - [详细信息](https://biolaysumm.org/)

##### 1.3 英文：MedVidQA 2023

- 来源：美国国立卫生研究院
- 介绍：在线视频可用性的激增改变了获取信息和知识的方式。以类似的方式，医疗教学视频更适合和有益于通过视觉和口头交流向消费者需要指导的医疗保健问题传递关键信息。本任务由两个主要任务组成：视频语料库视觉答案定位 (VCVAL) 和医学教学问题生成 (MIQG)。
- [官方地址](https://medvidqa.github.io/index.html)

##### 1.4 中文 (长期有效)：医疗信息处理挑战榜CBLUE数据集

- CBLUE 1.0：
  - 来源：中国中文信息学会医疗健康与生物信息处理专业委员会在合法开放共享的理念下发起，由阿里云天池平台承办，并由医渡云（北京）技术有限公司、平安医疗科技、北京大学、郑州大学、鹏城实验室、哈尔滨工业大学(深圳）、同济大学、夸克、阿里巴巴达摩院等开展智慧医疗研究的单位共同协办，旨在推动中文医学NLP技术和社区的发展。**由CHIP会议往届的学术评测比赛和阿里夸克医疗搜索业务的数据集组成。**
  - 介绍：涵盖了医学文本信息抽取（实体识别、关系抽取）、医学术语归一化、医学文本分类、医学句子语义相关性判定4大类常见的医疗信息处理任务，共包含8个子任务。
- CBLUE 2.0：
  - 来源：相比1.0 新增 复旦大学、腾讯天衍实验室和中山大学。
  - 介绍：涵盖了医学文本信息抽取（实体识别、关系抽取）、医学术语归一化、医学文本分类、医学句子语义相关性判定、医疗对话理解和生成5大类常见的医疗信息处理任务，共包含15个子任务。
    - 详细对比请参考 https://zhuanlan.zhihu.com/p/469465499 

- [CBLUE评测官方地址](https://tianchi.aliyun.com/dataset/dataDetail?dataId=95414)
- [论文地址](https://arxiv.org/abs/2106.08087)
- [Github项目地址](https://github.com/CBLUEbenchmark/CBLUE)

### 2. 已结束的评测/比赛(从2021开始)：

> 此部分包含从2021.2.20开始的测评/比赛 按照比赛出现时间倒序整理

##### 2.1 中文：非标准化疾病诉求的简单分诊挑战赛2.0

- 来源：科大讯飞
- 介绍：进行简单分诊需要一定的数据和经验知识进行支撑。本次比赛提供了部分好大夫在线的真实问诊数据，经过严格脱敏，提供给参赛者进行单分类任务。具体为：通过处理文字诉求，给出20个常见的就诊方向之一和61个疾病方向之一。
- [官方地址](http://challenge.xfyun.cn/topic/info?type=disease-claims-2022&ch=ds22-dw-sq03)

##### 2.2 中文：第八届中国健康信息处理大会(CHIP2022)测评任务

[官方地址](http://cips-chip.org.cn/) 

1. 测评一：面向“基因-疾病”的关联语义挖掘任务
   - 介绍：在海量科学文献中，“基因-疾病”的关联机理通过突变、基因等系列分子对象及其触发词获得描述，自然语言处理为自动挖掘这一隐性知识条目提供了可能，亦为健康医学信息的自动化处理提供解决方案。任务包括三个子任务：1、触发词实体识别；2、语义角色标注，3、“基因，调控类型，疾病”三元组抽取。所有数据取自AGAC语料库。
   - [任务网址](http://cips-chip.org.cn/2022/eval1)
2. 测评二：医疗因果实体关系抽取任务
   - 介绍：现代医疗很强调解释性，互联网上存在大量的医疗的问答和知识类的文本中存在大量的因果关系解释。任务为构建医疗因果知识图谱。
   - [任务网址](http://cips-chip.org.cn/2022/eval2)
3. 测评三：从医疗文本中抽取诊疗决策树
   - 介绍：探索如何从诊疗决策知识源（临床诊疗指南、医学教科书）中自动抽取诊疗决策树。
   - [任务网址](http://cips-chip.org.cn/2022/eval3)
4. 测评四：医疗纸质文档电子档(ePaper)OCR识别
   - 介绍：利用OCR及NLP技术将纸质材料上的信息进行电子化、结构化很有必要。  任务数据集中包括：出院小结、门诊发票、购药发票、住院发票这四类病历材料。主要针对需求：生活场景图片，提取数据，并生成电子结构化数据。
   - [任务网址](http://cips-chip.org.cn/2022/eval4)
5. 测评五：临床诊断编码任务
   - 介绍：疾病分类与手术操作分类编码是对患者疾病诊断和治疗信息的加工过程，是病案信息管理的重要环节。中国推出了疾病分类与代码国家临床版2.0和手术操作分类代码国家临床版2.0，在部分医院中得到了应用。本次评测任务主要目标是针对中文电子病历中进行诊断编码。给定一次就诊的相关诊断信息（包括入院诊断、术前诊断、术后诊断、出院诊断），以及手术名称、药品名称、医嘱名称，要求给出其对应的国家临床版2.0标准词。所有就诊数据均来自于真实医疗数据，并以《疾病分类与代码国家临床版2.0》词表为标准进行了标注。
   - [任务网址](http://cips-chip.org.cn/2022/eval5)

##### 2.3 中文：科大讯飞-医疗实体及关系识别挑战赛

- 来源：科大讯飞

- 介绍：针对医技报告单(一种半结构化的数据，不同医生的表述风格不一致，文本形式缺乏统一的规范)的命名实体识别和实体关系抽取。
- [评测官网](https://challenge.xfyun.cn/topic/info?type=medical-entity&ch=dc-web-35)

##### 2.4 中文：第一届智能对话诊疗评测比赛（CCL 2021）

- 来源：中国计算语言学大会2021（CCL 2021）：中山医院姚璐老师对数据标注框架设计提供专业指导建议。陈伟，钟宗烨，王静致远， 葛羽，王亚丽，温惠梅，司若琰等同学参与数据标注过程。

- 介绍: 发布5项技术评测任务，其中包含“智能医疗对话诊疗”任务。 本次智能对话诊疗评测设置医患对话理解(命名实体识别、症状识别)、医疗报告自动生成和智能化医疗诊断3个赛道共四个任务。
- [任务网址](http://www.fudan-disc.com/sharedtask/imcs21/index.html)

##### 2.5 英文：MEDIQA-2021

- 来源： NAACL-BioNLP 2021 workshop.
- 介绍：解决医疗领域的三项摘要任务：消费者健康问题摘要、多答案摘要和放射报告摘要，并探索使用不同的评估指标进行总结。
- [MEDIQA评测地址](https://sites.google.com/view/mediqa2021)

##### 2.6 英文： ICLR-2021-医疗对话生成与自动诊断国际竞赛

- 来源：ICLR 2021 workshop


- 介绍：本次竞赛以自动医疗诊断对话系统的开发为主题，目前设置了两大赛道：医疗对话生成赛道和自动医疗诊断赛道。
- [竞赛官方地址](https://mlpcp21.github.io/pages/challenge) 





## 二. 数据集

> 此部分包含大型的或者具有特色的中英文数据集，基本按数据集大小(问题数量)降序排序。

### 1. 中文数据集

##### 1.1 中文医患问答对话数据 (1.1M)

- 介绍: 来自haodf.com 的中文医患对话数据。

- [项目地址](https://github.com/UCSD-AI4H/Medical-Dialogue-System)

- 度盘下载地址: https://pan.baidu.com/s/1ZwzNgvAAMQk4klerTspsoA   提取码: lbo4



##### 1.2 中文医疗对话数据集（792K）

- 介绍：包含六个科室的医学问答数据，github开源数据 ，来源不明。

- [项目地址](https://github.com/Toyhom/Chinese-medical-dialogue-data)



##### 1.3 CPubMed-KG (4.4M三元组)

- 来源：中国中文信息学会医疗健康与生物信息处理专业委员会、语言与知识计算专委会医疗知识图谱专业组、深圳计算机学会人工智能专委会、哈尔滨工业大学（深圳）联合国内高水平医疗机构、中华医学会。
- 介绍：中华医学会高质量全文期刊数据所构建的大规模中文开放医学知识图谱及开放式医学知识在线协同构建平台，旨在通过完全开放、协作的机制来打破中文医学知识的瓶颈，支撑智慧医疗技术的发展。
- [项目地址](https://cpubmed.openi.org.cn/graph/wiki)



##### 1.4 CBLUE测评 

- CBLUE 1.0：
  - 来源：中国中文信息学会医疗健康与生物信息处理专业委员会在合法开放共享的理念下发起，由阿里云天池平台承办，并由医渡云（北京）技术有限公司、平安医疗科技、北京大学、郑州大学、鹏城实验室、哈尔滨工业大学(深圳）、同济大学、夸克、阿里巴巴达摩院等开展智慧医疗研究的单位共同协办，旨在推动中文医学NLP技术和社区的发展。**由CHIP会议往届的学术评测比赛和阿里夸克医疗搜索业务的数据集组成。**
  - 介绍：涵盖了医学文本信息抽取（实体识别、关系抽取）、医学术语归一化、医学文本分类、医学句子语义相关性判定4大类常见的医疗信息处理任务，共包含8个子任务。
- CBLUE 2.0：
  - 来源：相比1.0 新增 复旦大学、腾讯天衍实验室和中山大学。
  - 介绍：涵盖了医学文本信息抽取（实体识别、关系抽取）、医学术语归一化、医学文本分类、医学句子语义相关性判定、医疗对话理解和生成5大类常见的医疗信息处理任务，共包含15个子任务。
    - 详细对比请参考 https://zhuanlan.zhihu.com/p/469465499 

- [CBLUE评测官方地址](https://tianchi.aliyun.com/dataset/dataDetail?dataId=95414)
- [论文地址](https://arxiv.org/abs/2106.08087)
- [Github项目地址](https://github.com/CBLUEbenchmark/CBLUE)





##### 1.5 中文医学知识图谱 CMeKG (1M三元组)

- 介绍：CMeKG（Chinese Medical Knowledge Graph）是利用自然语言处理与文本挖掘技术，基于大规模医学文本数据，以人机结合的方式研发的中文医学知识图谱。CMeKG的构建参考了ICD、ATC、SNOMED、MeSH等权威的国际医学标准以及规模庞大、多源异构的临床指南、行业标准、诊疗规范与医学百科等医学文本信息。CMeKG 1.0包括：6310种疾病、19853种药物（西药、中成药、中草药）、1237种诊疗技术及设备的结构化知识描述，涵盖疾病的临床症状、发病部位、药物治疗、手术治疗、鉴别诊断、影像学检查、高危因素、传播途径、多发群体、就诊科室等以及药物的成分、适应症、用法用量、有效期、禁忌证等30余种常见关系类型，CMeKG描述的概念关系实例及属性三元组达100余万。

- [项目地址](http://cmekg.pcl.ac.cn/)



#####  1.6 cMedQA2 (108K)

- 介绍：中文医药方面的问答数据集，超过10万条。

  - questions.csv：所有的问题及其内容。answers.csv ：所有问题的答案。

  - train_candidates.txt， dev_candidates.txt， test_candidates.txt ：将上述两个文件进行了拆分。

- [数据集地址](https://www.kesci.com/home/dataset/5d313070cf76a60036e4b023/document)

- [数据集github地址](https://github.com/zhangsheng93/cMedQA2)



##### 1.7 xywy-KG(294K三元组)

- 来源：寻医问药网
- 介绍：44.1K实体  294.1K 三元组
- [项目地址](https://github.com/baiyang2464/chatbot-base-on-Knowledge-Graph)



##### 1.8 39Health-KG (210K三元组)

- 来源：39健康网。
- 介绍：包括15项信息，其中7类实体，约3.7万实体，21万实体关系。
- [项目地址](https://github.com/zhihao-chen/QASystemOnMedicalGraph)



##### 1.9 CHIP历年测评 (官方测评)

1. CHIP2022:  http://cips-chip.org.cn/2022/callforeval
2. CHIP2021: http://www.cips-chip.org.cn/2021/
3. CHIP2020: http://cips-chip.org.cn/2020/



##### 1.10 瑞金医院糖尿病数据集 (糖尿病)

- 介绍：数据集来自天池大赛。此数据集旨在通过糖尿病相关的教科书、研究论文来做糖尿病文献挖掘并构建糖尿病知识图谱。参赛选手需要设计高准确率，高效的算法来挑战这一科学难题。第一赛季课题为“基于糖尿病临床指南和研究论文的实体标注构建”，第二赛季课题为“基于糖尿病临床指南和研究论文的实体间关系构建”。
  - 官方提供的数据只包含训练集，真正用于最终排名的测试集没有给出。

- [数据集地址](https://tianchi.aliyun.com/competition/entrance/231687/information)

- 度盘下载地址：https://pan.baidu.com/s/1CWKblBNBqR-vs2h0xiXSdQ   提取码：0c54



##### 1.11 天池新冠肺炎问句匹配比赛 (新冠)

- 介绍：本次大赛数据包括：脱敏之后的医疗问题数据对和标注数据。医疗问题涉及“肺炎”、“支原体肺炎”、“支气管炎”、“上呼吸道感染”、“肺结核”、“哮喘”、“胸膜炎”、“肺气肿”、“感冒”、“咳血”等10个病种。

- [数据集地址(需注册)](https://tianchi.aliyun.com/competition/entrance/231776/information)

- [线上第四名解决方案及代码](https://github.com/Makaixin/similar-sentence-pairs-in-epidemic)

- [线上第一名解决方案及代码](https://github.com/zzy99/epidemic-sentence-pair) 





#### 2. 中国临床医生常用知识信息源

##### 2.1 pubMed

 https://pubmed.ncbi.nlm.nih.gov/ 

##### 2.2 Up-to-date

https://www.wolterskluwer.com/en/expert-insights/health

##### 2.3 临床指南

 https://guide.medlive.cn/

##### 2.4 用药助手

 https://drugs.dxy.cn/

##### 2.5 丁香园

 https://www.dxy.cn/

##### 2.6 丁香医生

 https://dxy.com/










### 3. 英文数据集

##### 3.1 PubMedQA

- 介绍： 基于Pubmed提取的医学问答数据集。PubMedQA has 1k expert-annotated, 61.2k unlabeled and 211.3k artificially gen- erated QA instances. 
- [论文地址](https://arxiv.org/abs/1909.06146)

##### 3.2 COMETA

- 介绍： 社交媒体中的医疗实体链接数据。发表于EMNLP2020。


- 数据获取方式： https://www.siphs.org/      https://github.com/cambridgeltl/cometa


- [论文地址](https://arxiv.org/pdf/2010.03295.pdf)

##### 3.3 MedMentions

- 介绍： 基于Pubmed摘要的生物医学实体链接数据集。发表于AKBC 2019。


- [数据集地址](https://github.com/chanzuckerberg/MedMentions)

- [论文地址](https://arxiv.org/abs/1902.09476)





## 三. 开源预训练模型

该部分介绍医疗NLP领域的大型语言模型，为从业人员提供初始化参数参考和训练方法参考。 基本按照模型大小降序排序。

#### 1. 现有Medical NLP大型模型

##### 1.1 BioMedLM (2.7B)

- 来源：Stanford  Chris Manning and Percy Liang Group
- 介绍：引入了一种新的 2.7B 参数语言模型，该模型在生物医学文献上进行了训练，为医学问答提供了改进的技术水平。（注意：应持有“PubMed”商标的 NIH 的要求，该模型已重命名为 BioMedLM。未来的更新将参考 BioMedLM）

- [项目地址](https://github.com/stanford-crfm/BioMedLM)

- [解读文章](https://crfm.stanford.edu/2022/12/15/pubmedgpt.html)

- [模型](https://huggingface.co/stanford-crfm/pubmedgpt/tree/main)



##### 1.2 BioGPT  (1.5B)

- 来源：Microsoft  Tie-Yan Liu Group
- 介绍：BioGPT是一种在大规模生物医学文献上预训练的特定领域生成式 Transformer 语言模型，在 PubMedQA上的准确率为 78.2%，创造了新的记录

- [项目地址](https://github.com/microsoft/BioGPT)



##### 1.3 Medical-chatgpt 

- 来源：Google Research and Deep AI
- 介绍：针对初级医学健康领域量身定制的ChatGPT的实施，但，奖励能够以彻底有效的方式收集患者病史并提出合理的鉴别诊断
- [项目地址](https://github.com/lucidrains/medical-chatgpt)
- [论文地址](https://arxiv.org/pdf/2212.13138.pdf)



##### 1.4 BioBERT

- 来源：Department of Computer Science and Engineering, Korea University，Interdisciplinary Graduate Program in Bioinformatics, Korea University, 
- 介绍： BioBERT（用于生物医学文本挖掘的 Transformers 的双向编码器表示）是一个在大规模生物医学语料库上预训练的特定领域语言表示模型。
- [项目地址](https://github.com/dmis-lab/biobert)
- [论文地址](https://arxiv.org/ftp/arxiv/papers/1901/1901.08746.pdf)



##### 1.5 PubMedBERT

- 来源：National Center for Biotechnology Information National Library of Medicine, National Institutes of Health Bethesda, MD, USA
- 介绍：PubMedBERT使用PubMed 的摘要从头开始预训练。
- [论文地址](https://arxiv.org/pdf/2007.15779.pdf)
- [模型地址](https://huggingface.co/microsoft/BiomedNLP-PubMedBERT-base-uncased-abstract)



#### 2. 其他可供在医疗领域微调的中文大模型

##### 2.1 Awesome List: 

https://github.com/lonePatient/awesome-pretrained-chinese-nlp-models#GPT

##### 2.2 0B-5B:

- 孟子(1B):  https://github.com/Langboat/Mengzi
- CPM-1(2.6B): https://github.com/TsinghuaAI/CPM-1-Generate
- gpt2-ml(1.5B): https://github.com/imcaspar/gpt2-ml
- Pangu-Alpha(2.6B): https://openi.pcl.ac.cn/PCL-Platform.Intelligence/PanGu-Alpha
- Chinese-Transformer-XL(2.9B): https://github.com/THUDM/Chinese-Transformer-XL

##### 2.3 5B-10B:

- GLM-10B： https://github.com/THUDM/glm
- ERNIE3.0(10B): https://github.com/PaddlePaddle/ERNIE

##### 2.4 10B-100B:

- Pangu-Alpha(13B): https://openi.pcl.ac.cn/PCL-Platform.Intelligence/PanGu-Alpha
- CPM-2(11B): https://github.com/TsinghuaAI/CPM-2-Finetune

##### 2.5 100B--:

- GLM-130B:https://github.com/THUDM/GLM-130B
- CPM-2-MoE(198B): https://openi.pcl.ac.cn/BAAI/WuDao-Model/src/branch/master/CPM
- Pangu-Alpha(200B):  https://openi.pcl.ac.cn/PCL-Platform.Intelligence/PanGu-Alpha
- 源1.0(245B): https://github.com/Shawn-Inspur/Yuan-1.0





## 四. 相关论文

此部分 更加侧重于收集 后ChatGPT时代的相关论文，大致以论文发表时间为序。

### 1. 后ChatGPT时代 可能有帮助的论文(持续更新)

1.  **ChatGPT在USMLE上的表现**：使用大型语言模型进行 AI 辅助医学教育的潜力
   - 论文地址：https://journals.plos.org/digitalhealth/article?id=10.1371/journal.pdig.0000198
   - 摘要翻译：我们评估了名为 ChatGPT 的大型语言模型在美国医学执照考试 (USMLE) 上的表现，该考试由三门考试组成：Step1、Step2CK 和 Step3。 ChatGPT 在所有三项考试中的表现均达到或接近通过门槛，无需任何专门培训或强化。 此外，ChatGPT 在其解释中表现出高度的一致性和洞察力。 这些结果表明，大型语言模型可能有助于医学教育，并可能有助于临床决策。
2. 对 **ChatGPT 的医疗建议进行（图灵）测试**
   - 论文地址：https://arxiv.org/abs/2301.10035
   - 摘要翻译：目标：评估使用 ChatGPT 或类似的基于 AI 的聊天机器人进行患者与提供者沟通的可行性。 参与者：美国代表性样本 430 名年龄在 18 岁及以上的研究参与者。53.2% 的受访者为女性； 他们的平均年龄是47.1岁。 曝光：从 EHR 中提取了 10 个具有代表性的非管理性患者-提供者交互。 患者的问题被放置在 ChatGPT 中，要求聊天机器人使用与人类提供者的回答大致相同的字数来回答。 在调查中，每个患者的问题之后都会有提供者或 ChatGPT 生成的回复。 参与者被告知有五个响应是由提供者生成的，五个是由聊天机器人生成的。 参与者被要求并在经济上受到激励，以正确识别响应源。 参与者还被问及他们对聊天机器人在患者与提供者沟通中的功能的信任，使用李克特量表 1-5。 结果：不同问题的回答正确分类在49.0%到85.7%之间。 平均而言，聊天机器人响应在 65.5% 的时间内被正确识别，供应商响应在 65.1% 的时间内被正确识别。 平均而言，患者对聊天机器人功能的信任度反应较弱（李克特平均得分：3.4），随着问题任务的健康相关复杂性增加，信任度降低。 结论：ChatGPT 对患者问题的回答与提供者的回答难以区分。 外行似乎相信使用聊天机器人来回答风险较低的健康问题。
3. **Toolformer**：语言模型可以自学使用工具
   - 论文地址：https://arxiv.org/abs/2302.04761
   - 摘要翻译：语言模型 (LM) 表现出非凡的能力，可以仅通过几个示例或文本指令来解决新任务，尤其是在规模上。 矛盾的是，它们还在基本功能上苦苦挣扎，例如算术或事实查找，而在这些功能中，更简单、更小的模型更胜一筹。 在本文中，我们展示了 LM 可以通过简单的 API 自学使用外部工具并实现两全其美。 我们介绍了 Toolformer，这是一个经过训练的模型，可以决定调用哪些 API、何时调用它们、传递哪些参数，以及如何最好地将结果纳入未来的代币预测。 这是以自我监督的方式完成的，只需要对每个 API 进行少量演示。 我们整合了一系列工具，包括计算器、问答系统、两个不同的搜索引擎、翻译系统和日历。 Toolformer 在各种下游任务中实现了显着改进的零样本性能，通常与更大的模型竞争，而不会牺牲其核心语言建模能力。
4. 检查你的事实并再试一次：**利用外部知识和自动反馈改进大型语言模型**
   - 论文地址：https://arxiv.org/abs/2302.12813
   - 摘要翻译：大型语言模型 (LLM)，例如 ChatGPT，能够为许多下游任务生成类似人类的流畅响应，例如面向任务的对话和问答。 然而，将 LLM 应用于现实世界的关键任务应用程序仍然具有挑战性，主要是因为它们倾向于产生幻觉并且无法使用外部知识。 本文提出了一个 LLM-Augmenter 系统，它使用一组即插即用模块来增强黑盒 LLM。 我们的系统使 LLM 生成基于外部知识的响应，例如存储在任务特定的数据库中。 它还迭代地修改 LLM 提示，以使用实用函数生成的反馈改进模型响应，例如LLM 生成的响应的真实性分数。 LLM-Augmenter 的有效性在两种类型的场景中得到了实证验证，即面向任务的对话和开放域问答。 LLM-Augmenter 在不牺牲其响应的流畅性和信息量的情况下显着减少了 ChatGPT 的幻觉。 我们公开提供源代码和模型。







### 2. 2021前仓库论文总结存档

#### 2.1 综述类文章

**nature medicine发表的综述**

论文题目：A guide to deep learning in healthcare

[论文地址](https://www.nature.com/articles/s41591-018-0316-z)

论文概要：发表于nature medicine，包含医学领域下CV,NLP,强化学习等方面的应用综述。

论文摘要：Here we present deep-learning techniques for healthcare, centering our discussion on deep learning in computer vision, natural language processing, reinforcement learning, and generalized methods. We describe how these computational techniques can impact a few key areas of medicine and explore how to build end-to-end systems. Our discussion of computer vision focuses largely on medical imaging, and we describe the application of natural language processing to domains such as electronic health record data. Similarly, reinforcement learning is discussed in the context of robotic-assisted surgery, and generalized deep- learning methods for genomics are reviewed.

#### 2.2 电子病历相关文章

**Transfer Learning from Medical Literature for Section Prediction in Electronic Health Records**

[论文地址](https://www.aclweb.org/anthology/D19-1492/)

论文概要：发表于EMNLP2019。基于少量in-domain数据和大量out-of-domain数据进行EHR相关的迁移学习。

论文摘要：sections such as Assessment and Plan, So- cial History, and Medications. These sec- tions help physicians find information easily and can be used by an information retrieval system to return specific information sought by a user. However, it is common that the exact format of sections in a particular EHR does not adhere to known patterns. There- fore, being able to predict sections and headers in EHRs automatically is beneficial to physi- cians. Prior approaches in EHR section pre- diction have only used text data from EHRs and have required significant manual annota- tion. We propose using sections from med- ical literature (e.g., textbooks, journals, web content) that contain content similar to that found in EHR sections. Our approach uses data from a different kind of source where la- bels are provided without the need of a time- consuming annotation effort. We use this data to train two models: an RNN and a BERT- based model. We apply the learned models along with source data via transfer learning to predict sections in EHRs. Our results show that medical literature can provide helpful su- pervision signal for this classification task.

**MUFASA: Multimodal Fusion Architecture Search for Electronic Health Records**

[论文地址](http://arxiv-download.xixiaoyao.cn/pdf/2102.02340.pdf)

论文概要:发表于AAAI2021。

论文摘要:One important challenge of applying deep learning to electronic health records (EHR) is the complexity of their multimodal structure. EHR usually contains a mixture of structured (codes) and unstructured (free-text) data with sparse and irregular longitudinal features – all of which doctors utilize when making decisions. In the deep learning regime, determining how different modality representations should be fused together is a difficult problem, which is often addressed by handcrafted modeling and intuition. In this work, we extend state-of-the-art neural architecture search (NAS) methods and propose MUltimodal Fusion Architecture SeArch (MUFASA) to simultaneously search across multimodal fusion strategies and modality-specific architectures for the first time. We demonstrate empirically that our MUFASA method outperforms established unimodal NAS on public EHR data with comparable computation costs. In addition, MUFASA produces architectures that outperform Transformer and Evolved Transformer. Compared with these baselines on CCS diagnosis code prediction, our discovered models improve top-5 recall from 0.88 to 0.91 and demonstrate the ability to generalize to other EHR tasks. Studying our top architecture in depth, we provide empirical evidence that MUFASA’s improvements are derived from its ability to both customize modeling for each data modality and find effective fusion strategies.


#### 2.3 医学关系抽取

**Leveraging Dependency Forest for Neural Medical Relation Extraction**

[论文地址](https://www.aclweb.org/anthology/D19-1020/)

论文概要：发表于EMNLP 2019. 基于dependency forest方法，提升对医学语句中依存关系的召回率，同时引进了一部分噪声，基于图循环网络进行特征提取，提供了在医疗关系抽取中使用依存关系，同时减少误差传递的一种思路。

论文摘要：Medical relation extraction discovers relations between entity mentions in text, such as research articles. For this task, dependency syntax has been recognized as a crucial source of features. Yet in the medical domain, 1-best parse trees suffer from relatively low accuracies, diminishing their usefulness. We investigate a method to alleviate this problem by utilizing dependency forests. Forests contain more than one possible decisions and therefore have higher recall but more noise compared with 1-best outputs. A graph neural network is used to represent the forests, automatically distinguishing the useful syntactic information from parsing noise. Results on two benchmarks show that our method outperforms the standard tree-based methods, giving the state-of-the-art results in the literature.

#### 2.4 医学知识图谱

**Learning a Health Knowledge Graph from Electronic Medical Records**

[论文地址](https://www.nature.com/articles/s41598-017-05778-z)

论文概要：发表于nature scientificreports（2017）. 基于27万余份电子病历构建的疾病-症状知识图谱。

论文摘要：Demand for clinical decision support systems in medicine and self-diagnostic symptom checkers has substantially increased in recent years. Existing platforms rely on knowledge bases manually compiled through a labor-intensive process or automatically derived using simple pairwise statistics. This study explored an automated process to learn high quality knowledge bases linking diseases and symptoms directly from electronic medical records. Medical concepts were extracted from 273,174 de-identified patient records and maximum likelihood estimation of three probabilistic models was used to automatically construct knowledge graphs: logistic regression, naive Bayes classifier and a Bayesian network using noisy OR gates. A graph of disease-symptom relationships was elicited from the learned parameters and the constructed knowledge graphs were evaluated and validated, with permission, against Google’s manually-constructed knowledge graph and against expert physician opinions. Our study shows that direct and automated construction of high quality health knowledge graphs from medical records using rudimentary concept extraction is feasible. The noisy OR model produces a high quality knowledge graph reaching precision of 0.85 for a recall of 0.6 in the clinical evaluation. Noisy OR significantly outperforms all tested models across evaluation frameworks (p < 0.01).

#### 2.5 辅助诊断

**Evaluation and accurate diagnoses of pediatric diseases using artificial intelligence**

[论文地址](https://www.nature.com/articles/s41591-018-0335-9)

论文概要：该文章由广州市妇女儿童医疗中心与依图医疗等企业和科研机构共同完成，基于机器学习的自然语言处理（NLP）技术实现不输人类医生的强大诊断能力，并具备多场景的应用能力。据介绍，这是全球首次在顶级医学杂志发表有关自然语言处理（NLP）技术基于电子健康记录（EHR）做临床智能诊断的研究成果，也是利用人工智能技术诊断儿科疾病的重磅科研成果。

论文摘要：Artificial intelligence (AI)-based methods have emerged as powerful tools to transform medical care. Although machine learning classifiers (MLCs) have already demonstrated strong performance in image-based diagnoses, analysis of diverse and massive electronic health record (EHR) data remains challenging. Here, we show that MLCs can query EHRs in a manner similar to the hypothetico-deductive reasoning used by physicians and unearth associations that previous statistical methods have not found. Our model applies an automated natural language processing system using deep learning techniques to extract clinically relevant information from EHRs. In total, 101.6 million data points from 1,362,559 pediatric patient visits presenting to a major referral center were analyzed to train and validate the framework. Our model demonstrates high diagnostic accuracy across multiple organ systems and is comparable to experienced pediatricians in diagnosing common childhood diseases. Our study provides a proof of concept for implementing an AI-based system as a means to aid physicians in tackling large amounts of data, augmenting diagnostic evaluations, and to provide clinical decision support in cases of diagnostic uncertainty or complexity. Although this impact may be most evident in areas where healthcare providers are in relative shortage, the benefits of such an AI system are likely to be universal.

#### 2.6 ACL2020医学领域相关论文列表

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

#### 2.7 医疗实体Linking（标准化）

**Medical Entity Linking using Triplet Network**

[论文地址](https://www.aclweb.org/anthology/W19-1912/)

论文概要： 发表于ACL2019,论文内容为疾病实体Linking研究。使用三元组数据，（mention，正例，负例），目标使distance(mention,负例)-distance(mention,正例)>alpha（人脸识别的经典方案）,具体损失函数参看论文。论文主要包括两部分内容1）候选数据集生成,对给定mention，与标准疾病集合数据（标准词及同义词）计算余弦相似度及Jaccard overlap分数,取topK作为候选样例。 2）网络结构基于Triplet Network。详见论文。

**A Generate-and-Rank Framework with Semantic Type Regularization for Biomedical Concept Normalization**

[论文地址](https://www.aclweb.org/anthology/2020.acl-main.748.pdf)

论文概要: 发表于ACL2020。基于list-wise排序学习方法。主要分为两部分：后续数据集生成 和  基于BERT的list-wise排序。较新颖的思路：1）在样本生成过程中，对标准词进行了基于同义词的扩展。2）在loss中引入了语义类型正则化。详见论文。

**Deep Neural Models for Medical Concept Normalization in User-Generated Texts**

[论文地址](https://www.aclweb.org/anthology/P19-2055.pdf)


#### 2.8 AAAI2020 医学NLP相关论文列表

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

#### 2.9 EMNLP2020 医学NLP相关论文列表

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





## 五. 开源工具包

#### 5.1 分词工具：PKUSEG

- [项目地址](https://github.com/lancopku/pkuseg-python)
- 项目说明： 北京大学推出的多领域中文分词工具，支持选择医学领域。





## 六. 工业级产品解决方案

#### 6.1 [灵医智慧](https://01.baidu.com/index.html)

#### 6.2 [左手医生](https://open.zuoshouyisheng.com/)

#### 6.3 [医渡云研究院-医学自然语言处理](https://www.yiducloud.com.cn/academy.html)

#### 6.4 [百度-医学文本结构化](https://ai.baidu.com/solution/mtp)

#### 6.5 [阿里云-医学自然语言处理](https://help.aliyun.com/document_detail/179395.html)





## 七. blog分享

#### 7.1 [医疗领域构建自然语言处理系统的经验教训](http://www.oreilly.com.cn/radar/?p=2083)

#### 7.2 [大数据时代的医学公共数据库与数据挖掘技术简介](https://mp.weixin.qq.com/s/tA44U4bJUttnROfrzpNYcQ)

#### 7.3 [从ACL 2021中看NLP在医疗领域应用的发展，附资源下载](https://mp.weixin.qq.com/s/RhcHvRWHRnYUg6u9vXoIGA)





## 八. 友情链接

#### 8.1 [awesome_Chinese_medical_NLP](https://github.com/GanjinZero/awesome_Chinese_medical_NLP)

#### 8.2 [中文NLP数据集搜索](https://www.cluebenchmarks.com/dataSet_search.html)

#### 8.3 [medical-data(海量医疗相关数据)](https://github.com/beamandrew/medical-data)

#### 8.4 [天池数据集(其中包含多个医疗NLP数据集)](https://tianchi.aliyun.com/dataset)

