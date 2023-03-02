# Chinese_medical_NLP

>🚀🚀🚀欢迎大家参与共建：
>
>由于本人2021年离开医疗NLP领域，这个repo已经较长时间没有更新，如果有从事相关领域的同学想要继续维护此repo，可以联系我把你添加为共建者（或其他方式）。
>
>🤝🤝🤝
>
>wx: 18810877926  备注： github 医疗




医疗NLP领域（主要关注中文）   评测数据集 与 论文等相关资源。

   * [Chinese_medical_NLP](#chinese_medical_nlp)
     * [评测/比赛更新](#评测及比赛更新)
       * [1. MEDIQA 2021](#mediqa-2021)
       * [2. ICLR 2021 医疗对话生成与自动诊断国际竞赛](#iclr-2021-医疗对话生成与自动诊断国际竞赛)
       * [3. 中文医疗信息处理挑战榜CBLUE数据集](#中文医疗信息处理挑战榜CBLUE数据集)
       * [4. 中国计算语言学大会CCL 2021智能医疗对话诊疗评测任务](#中国计算语言学大会CCL-2021智能医疗对话诊疗评测任务)
       * [5. 科大讯飞 医疗实体及关系识别挑战赛](#科大讯飞-医疗实体及关系识别挑战赛)
     * [中文数据集](#中文数据集)
       * [1. Yidu-S4K：医渡云结构化4K数据集](#1-yidu-s4k医渡云结构化4k数据集)
       * [2.瑞金医院糖尿病数据集](#2瑞金医院糖尿病数据集)
       * [3.Yidu-N7K：医渡云标准化7K数据集](#3yidu-n7k医渡云标准化7k数据集)
       * [4.中文医学问答数据集](#4中文医学问答数据集)
       * [5.平安医疗科技疾病问答迁移学习比赛](#5平安医疗科技疾病问答迁移学习比赛)
       * [6.天池新冠肺炎问句匹配比赛](#6天池新冠肺炎问句匹配比赛)
       * [7.中文医患问答对话数据](#7中文医患问答对话数据)
       * [8.中文医学问答数据](#8中文医学问答数据)
       * [9.CHIP2020各项评测已开放](#9chip2020各项评测已开放)
       * [10.医学数据挖掘与算法评测大赛](#10医学数据挖掘与算法评测大赛)
       * [11.中文医疗对话数据集](#11中文医疗对话数据集)
       * [12.阿里发布的中文医疗标准数据集合](#12阿里发布的中文医疗标准数据集合)
     * [中文医学知识图谱](#中文医学知识图谱)
       * [CMeKG](#cmekg)
     * [英文数据集](#英文数据集)
       * [PubMedQA: A Dataset for Biomedical Research Question Answering](#pubmedqa-a-dataset-for-biomedical-research-question-answering)
       * [COMETA: A Corpus for Medical Entity Linking in the Social Media](#cometa-a-corpus-for-medical-entity-linking-in-the-social-media)
       * [MedMentions](#medmentions)
     * [相关论文](#相关论文)
       * [1.医疗领域预训练embedding](#1医疗领域预训练embedding)
       * [2.综述类文章](#2综述类文章)
       * [3.电子病历相关文章](#3电子病历相关文章)
       * [4.医学关系抽取](#4医学关系抽取)
       * [5.医学知识图谱](#5医学知识图谱)
       * [6.辅助诊断](#6辅助诊断)
       * [7.ACL2020医学领域相关论文列表](#7acl2020医学领域相关论文列表)
       * [8.医疗实体Linking（标准化）](#8医疗实体linking标准化)
       * [9. AAAI2020 医学NLP相关论文列表](#9-aaai2020-医学nlp相关论文列表)
       * [10. EMNLP2020 医学NLP相关论文列表](#10-emnlp2020-医学nlp相关论文列表)
     * [中文医疗领域语料](#中文医疗领域语料)
       * [医学教材 培训考试](#医学教材培训考试)
       * [哈工大《大词林》开放75万核心实体词及相关概念、关系列表（包含中药/医院/生物 类别）](#哈工大大词林开放75万核心实体词及相关概念关系列表包含中药医院生物-类别)
     * [医学embedding及预训练模型](#医学embedding及预训练模型)
       * [开源英文医学embedding](#开源英文医学embedding)
       * [MC-BERT中文医疗预训练模型](#MC-BERT中文医疗预训练模型)
     * [开源工具包](#开源工具包)
       * [分词工具](#分词工具)
         * [PKUSEG](#pkuseg)
     * [工业级产品解决方案](#工业级产品解决方案)
     * [blog分享](#blog分享)
     * [友情链接](#友情链接)

## 评测及比赛更新

说明: 这部分从2021.2.20开始更新。添加当时还未截止的中英文医疗相关的NLP评测或比赛。

### MEDIQA-2021

来源： NAACL 2021 workshop

Introduction

MEDIQA 2021 tackles three summarization tasks in the medical domain: consumer health question summarization, multi-answer summarization, and radiology report summarization. In this shared task, we will also explore the use of different evaluation metrics for summarization.

MEDIQA 2021 will be organized at the NAACL-BioNLP 2021 workshop.

[BioNLP Workshop](https://aclweb.org/aclwiki/BioNLP_Workshop)

[MEDIQA评测地址](https://sites.google.com/view/mediqa2021)

### ICLR-2021-医疗对话生成与自动诊断国际竞赛

来源: ICLR 2021 workshop

本次竞赛以自动医疗诊断对话系统的开发为主题，目前设置了两大赛道：医疗对话生成赛道和自动医疗诊断赛道。

[竞赛官方地址](https://mlpcp21.github.io/pages/challenge)

### 中文医疗信息处理挑战榜CBLUE数据集

评测介绍:

中文医疗信息处理挑战榜CBLUE(Chinese Biomedical Language Understanding Evaluation)是中国中文信息学会医疗健康与生物信息处理专业委员会在合法开放共享的理念下发起，由阿里云天池平台承办，并由医渡云（北京）技术有限公司、平安医疗科技、北京大学、郑州大学、鹏城实验室、哈尔滨工业大学(深圳）、同济大学、夸克、阿里巴巴达摩院等开展智慧医疗研究的单位共同协办，旨在推动中文医学NLP技术和社区的发展。评测长期开放。

CBLUE 1.0是由CHIP会议往届的学术评测比赛和阿里夸克医疗搜索业务的数据集组成，包括医学文本信息抽取（实体识别、关系抽取）、医学术语归一化、医学文本分类、医学句子关系判定和医学QA共5大类任务8个子任务。

[CBLUE评测官方地址](https://tianchi.aliyun.com/dataset/dataDetail?dataId=95414)

[论文地址](https://arxiv.org/abs/2106.08087)

[Github项目地址](https://github.com/CBLUEbenchmark/CBLUE)


### 中国计算语言学大会CCL-2021智能医疗对话诊疗评测任务

中国计算语言学大会（CCL 2021）发布5项技术评测任务，其中包含“智能医疗对话诊疗”任务。

任务介绍:

本次智能对话诊疗评测设置3个赛道。

赛道一：医患对话理解
医患对话理解旨在对问诊文本信息进行信息抽取，主要包括两个任务，分别是命名实体识别和症状检查识别。

任务1：命名实体识别。从医患对话文本中识别出五类重要的医疗相关实体。
任务2：症状识别。根据医患对话文本，识别出病人具有的症状信息。
本赛道数据集包括超过3000组医患对话案例样本，覆盖6种儿科疾病，10万余句对话，样本平均对话次数为40次， 平均每个样本的对话字数为523个。

赛道二：医疗报告自动生成
医疗报告自动生成旨在对问诊过程中进行信息的总结，任务要求参赛团队能依据病人自述和医患对话， 输出具有规定格式的医疗报告。报告需要包含6个部分：主诉、现病史、辅助检查、既往史、诊断和建议。

任务1：医疗报告生成。依据病人自述和医患对话，输出具有规定格式的医疗报告。
本赛道数据集包括超过3000组医患对话案例样本，覆盖6种儿科疾病，10万余句对话，样本平均对话次数为40次， 平均每个样本的对话字数为523个。

赛道三：智能化医疗诊断
就诊过程是一个带有目的的序列化医生-患者交互的过程。智能化医疗诊断是任务型对话系统的重点研究方向。

任务1：面向自动诊疗的对话系统。要求参赛系统根据给出的显性信息 （病人自诉中提及的症状、检查），与病人模拟器进行互动以获取更多病人的症状、已做的医疗检查， 依据交互内容判断疾病，并给出相应的检查建议。
本赛道的数据集超过2000个样本，每个样本包含疾病类别、病人自诉文本、直接信息 （病人自诉中明确提及的实体信息，包括症状和检查）、隐藏信息（结合整段医患对话得到的实体及标签，表示患者是否已经有该症状、是否已经做过该检查）。

[任务网址](http://www.fudan-disc.com/sharedtask/imcs21/index.html)

附：

[CCL2021评测官网](http://cips-cl.org/static/CCL2021/cclEval/taskEvaluation/index.html)

### 科大讯飞-医疗实体及关系识别挑战赛

评测介绍：电子病历是医疗机构对门诊、住院患者进行临床治疗和指导干预的数字化医疗服务工作记录，包含了大量的患者医学信息。医技报告单是电子病历十分重要组成部分，其中包含了患者详细的检查检验信息，如超声、CT和磁共振等。但是，医技报告单是一种半结构化的数据，不同医生的表述风格不一致，文本形式缺乏统一的规范，因此将其中非结构化的部分转换为结构化的信息是非常重要的，可以有效的提高医生工作效率，优化医疗机构流程。医技领域的命名实体和实体关系识别是目前的研究热点之一，同时也是电子病历信息抽取的重要研究内容。评测任务包含医学实体识别+医学关系抽取。

[评测官网](https://challenge.xfyun.cn/topic/info?type=medical-entity&ch=dc-web-35)
## 中文数据集

### 1. Yidu-S4K：医渡云结构化4K数据集

数据集描述：

> Yidu-S4K 数据集源自CCKS 2019 评测任务一，即“面向中文电子病历的命名实体识别”的数据集，包括两个子任务：
> 1）医疗命名实体识别：由于国内没有公开可获得的面向中文电子病历医疗实体识别数据集，本年度保留了医疗命名实体识别任务，对2017年度数据集做了修订，并随任务一同发布。本子任务的数据集包括训练集和测试集。
> 2）医疗实体及属性抽取（跨院迁移）：在医疗实体识别的基础上，对预定义实体属性进行抽取。本任务为迁移学习任务，即在只提供目标场景少量标注数据的情况下，通过其他场景的标注数据及非标注数据进行目标场景的识别任务。本子任务的数据集包括训练集（非目标场景和目标场景的标注数据、各个场景的非标注数据）和测试集（目标场景的标注数据

[数据集地址](http://openkg.cn/dataset/yidu-s4k)

度盘下载地址：https://pan.baidu.com/s/1QqYtqDwhc_S51F3SYMChBQ

提取码：flql

### 2.瑞金医院糖尿病数据集

数据集描述：

>数据集来自天池大赛。此数据集旨在通过糖尿病相关的教科书、研究论文来做糖尿病文献挖掘并构建糖尿病知识图谱。参赛选手需要设计高准确率，高效的算法来挑战这一科学难题。第一赛季课题为“基于糖尿病临床指南和研究论文的实体标注构建”，第二赛季课题为“基于糖尿病临床指南和研究论文的实体间关系构建”。

官方提供的数据只包含训练集，真正用于最终排名的测试集没有给出。

[数据集地址](https://tianchi.aliyun.com/competition/entrance/231687/information)

度盘下载地址：https://pan.baidu.com/s/1CWKblBNBqR-vs2h0xiXSdQ

提取码：0c54

### 3.Yidu-N7K：医渡云标准化7K数据集

数据集描述：

>Yidu-N4K 数据集源自CHIP 2019 评测任务一，即“临床术语标准化任务”的数据集。
>临床术语标准化任务是医学统计中不可或缺的一项任务。临床上，关于同一种诊断、手术、药品、检查、化验、症状等往往会有成百上千种不同的写法。标准化（归一）要解决的问题就是为临床上各种不同说法找到对应的标准说法。有了术语标准化的基础，研究人员才可对电子病历进行后续的统计分析。本质上，临床术语标准化任务也是语义相似度匹配任务的一种。但是由于原词表述方式过于多样，单一的匹配模型很难获得很好的效果。

[数据集地址](http://openkg.cn/dataset/yidu-n7k)

### 4.中文医学问答数据集

数据集描述：

>中文医药方面的问答数据集，超过10万条。

数据说明:

>questions.csv：所有的问题及其内容。answers.csv ：所有问题的答案。
>train_candidates.txt， dev_candidates.txt， test_candidates.txt ：将上述两个文件进行了拆分。

[数据集地址](https://www.kesci.com/home/dataset/5d313070cf76a60036e4b023/document)

[数据集github地址](https://github.com/zhangsheng93/cMedQA2)

### 5.平安医疗科技疾病问答迁移学习比赛

数据集描述：

>本次比赛是chip2019中的评测任务二，由平安医疗科技主办。chip2019会议详情见链接：http://cips-chip.org.cn/evaluation
>迁移学习是自然语言处理中的重要一环，其主要目的是通过从已学习的相关任务中转移知识来改进新任务的学习效果，从而提高模型的泛化能力。
>本次评测任务的主要目标是针对中文的疾病问答数据，进行病种间的迁移学习。具体而言，给定来自5个不同病种的问句对，要求判定两个句子语义是否相同或者相近。所有语料来自互联网上患者真实的问题，并经过了筛选和人工的意图匹配标注。

[数据集地址(需注册)](https://www.biendata.com/competition/chip2019/)

### 6.天池新冠肺炎问句匹配比赛

数据集描述：

>本次大赛数据包括：脱敏之后的医疗问题数据对和标注数据。医疗问题涉及“肺炎”、“支原体肺炎”、“支气管炎”、“上呼吸道感染”、“肺结核”、“哮喘”、“胸膜炎”、“肺气肿”、“感冒”、“咳血”等10个病种。
>数据共包含train.csv、dev.csv、test.csv三个文件，其中给参赛选手的文件包含训练集train.csv和验证集dev.csv，测试集test.csv 对参赛选手不可见。
>每一条数据由 Category，Query1，Query2，Label构成，分别表示问题类别、问句1、问句2、标签。Label表示问句之间的语义是否相同，若相同，标为1，若不相同，标为0。其中，训练集Label已知，验证集和测试集Label未知。
>示例
>类别：肺炎
>问句1：肺部发炎是什么原因引起的？
>问句2：肺部发炎是什么引起的
>标签:1
>类别：肺炎
>问句1：肺部发炎是什么原因引起的？
>问句2：肺部炎症有什么症状
>标签:0

[数据集地址(需注册)](https://tianchi.aliyun.com/competition/entrance/231776/information)

[线上第四名解决方案及代码](https://github.com/Makaixin/similar-sentence-pairs-in-epidemic)

[线上第一名解决方案及代码](https://github.com/zzy99/epidemic-sentence-pair)

### 7.中文医患问答对话数据

数据说明: 来自某在线求医产品的中文医患对话数据。

原始描述:The MedDialog dataset contains conversations (in Chinese) between doctors and patients. It has 1.1 million dialogues and 4 million utterances. The data is continuously growing and more dialogues will be added. The raw dialogues are from haodf.com. All copyrights of the data belong to haodf.com.

[项目地址](https://github.com/UCSD-AI4H/Medical-Dialogue-System)

度盘下载地址: https://pan.baidu.com/s/1ZwzNgvAAMQk4klerTspsoA

提取码: lbo4

### 8.中文医学问答数据

数据说明: 包含六个科室的医学问答数据，来源不明。

[项目地址](https://github.com/Toyhom/Chinese-medical-dialogue-data)

### 9.CHIP2020各项评测已开放

CHIP2020各项评测已开放，包括医学领域的实体识别，关系抽取，文本生成，术语标准化等任务，可以前往官网查阅。

[CHIP2020官方网址](http://cips-chip.org.cn/2020/)

### 10.医学数据挖掘与算法评测大赛

新鲜出炉，详情参看paperweekly公众号。[文章链接](https://mp.weixin.qq.com/s/3hiJy8m0VohYfEH5ISta5w)

### 11.中文医疗对话数据集

github开源数据

[项目地址](https://github.com/Toyhom/Chinese-medical-dialogue-data)

### 12.阿里发布的中文医疗标准数据集合

阿里团队发布的中文医疗NLP相关评测数据集合Chinese_BLUE,发表于WSDM2020。另外:项目中说此项目非阿里的官方产品，所以仅供参考。

[项目地址](https://github.com/alibaba-research/ChineseBLUE)

[论文地址](https://arxiv.org/pdf/2008.10813.pdf)

## 中文医学知识图谱

### CMeKG

[地址](http://cmekg.pcl.ac.cn/)

简介：CMeKG（Chinese Medical Knowledge Graph）是利用自然语言处理与文本挖掘技术，基于大规模医学文本数据，以人机结合的方式研发的中文医学知识图谱。CMeKG的构建参考了ICD、ATC、SNOMED、MeSH等权威的国际医学标准以及规模庞大、多源异构的临床指南、行业标准、诊疗规范与医学百科等医学文本信息。CMeKG 1.0包括：6310种疾病、19853种药物（西药、中成药、中草药）、1237种诊疗技术及设备的结构化知识描述，涵盖疾病的临床症状、发病部位、药物治疗、手术治疗、鉴别诊断、影像学检查、高危因素、传播途径、多发群体、就诊科室等以及药物的成分、适应症、用法用量、有效期、禁忌证等30余种常见关系类型，CMeKG描述的概念关系实例及属性三元组达100余万。

## 英文数据集

### PubMedQA: A Dataset for Biomedical Research Question Answering

数据集描述： 基于Pubmed提取的医学问答数据集。PubMedQA has 1k expert-annotated, 61.2k unlabeled and 211.3k artificially gen- erated QA instances. 

[论文地址](https://arxiv.org/abs/1909.06146)

### COMETA: A Corpus for Medical Entity Linking in the Social Media

数据集描述： 社交媒体中的医疗实体链接数据。发表于EMNLP2020。

数据获取方式:
COMETA is available by contacting the last author via e-mail or following the instructions on https://www.siphs.org/. We release the
pre-trained embeddings and the code to replicate our baselines online at https://github.com/cambridgeltl/cometa.

[论文地址](https://arxiv.org/pdf/2010.03295.pdf)

### MedMentions

数据集描述： 基于Pubmed摘要的生物医学实体链接数据集。发表于AKBC 2019。

[数据集地址](https://github.com/chanzuckerberg/MedMentions)

[论文地址](https://arxiv.org/abs/1902.09476)

## 相关论文

### 1.医疗领域预训练embedding

注：目前没有收集到中文医疗领域的开源预训练模型，以下列出英文论文供参考。

**Bio-bert**

论文题目：BioBERT: a pre-trained biomedical language representation model for biomedical text mining

[论文地址](https://academic.oup.com/bioinformatics/advance-article/doi/10.1093/bioinformatics/btz682/5566506)

[项目地址](https://github.com/dmis-lab/biobert)

论文概要：以通用领域预训练bert为初始权重，基于Pubmed上大量医疗领域英文论文训练。在多个医疗相关下游任务中超越SOTA模型的表现。

论文摘要：

> **Motivation**: Biomedical text mining is becoming increasingly important as the number of biomedical documents rapidly grows. With the progress in natural language processing (NLP), extracting valuable information from bio- medical literature has gained popularity among researchers, and deep learning has boosted the development of ef- fective biomedical text mining models. However, directly applying the advancements in NLP to biomedical text min- ing often yields unsatisfactory results due to a word distribution shift from general domain corpora to biomedical corpora. In this article, we investigate how the recently introduced pre-trained language model BERT can be adapted for biomedical corpora. 
> **Results**: We introduce BioBERT (Bidirectional Encoder Representations from Transformers for Biomedical Text Mining), which is a domain-specific language representation model pre-trained on large-scale biomedical corpora. With almost the same architecture across tasks, BioBERT largely outperforms BERT and previous state-of-the-art models in a variety of biomedical text mining tasks when pre-trained on biomedical corpora. While BERT obtains performance comparable to that of previous state-of-the-art models, BioBERT significantly outperforms them on the following three representative biomedical text mining tasks: biomedical named entity recognition (0.62% F1 score improvement), biomedical relation extraction (2.80% F1 score improvement) and biomedical question answering (12.24% MRR improvement). Our analysis results show that pre-training BERT on biomedical corpora helps it to understand complex biomedical texts. 
> **Availability and implementation**: We make the pre-trained weights of BioBERT freely available at https://github.com/naver/biobert-pretrained, and the source code for fine-tuning BioBERT available at https://github.com/dmis-lab/biobert.

**sci-bert**

论文题目：SCIBERT: A Pretrained Language Model for Scientific Text

[论文地址](https://arxiv.org/abs/1903.10676)

[项目地址](https://github.com/allenai/scibert/)

论文概要：AllenAI 团队出品.基于Semantic Scholar 上 110万+ 文章训练的 科学领域bert.

论文摘要：Obtaining large-scale annotated data for NLP tasks in the scientific domain is challeng- ing and expensive. We release SCIBERT, a pretrained language model based on BERT (Devlin et al., 2019) to address the lack of high-quality, large-scale labeled scientific data. SCIBERT leverages unsupervised pretraining on a large multi-domain corpus of scientific publications to improve perfor- mance on downstream scientific NLP tasks. We evaluate on a suite of tasks including sequence tagging, sentence classification and dependency parsing, with datasets from a variety of scientific domains. We demon- strate statistically significant improvements over BERT and achieve new state-of-the- art results on several of these tasks. The code and pretrained models are available at https://github.com/allenai/scibert/.

**clinical-bert**

论文题目：Publicly Available Clinical BERT Embeddings

[论文地址](https://www.aclweb.org/anthology/W19-1909/)

[项目地址](https://github.com/EmilyAlsentzer/clinicalBERT)

论文概要：出自NAACL Clinical NLP Workshop 2019.基于MIMIC-III数据库中的200万份医疗记录训练的临床领域bert.

论文摘要：Contextual word embedding models such as ELMo and BERT have dramatically improved performance for many natural language processing (NLP) tasks in recent months. However, these models have been minimally explored on specialty corpora, such as clinical text; moreover, in the clinical domain, no publicly-available pre-trained BERT models yet exist. In this work, we address this need by exploring and releasing BERT models for clinical text: one for generic clinical text and another for discharge summaries specifically. We demonstrate that using a domain-specific model yields performance improvements on 3/5 clinical NLP tasks, establishing a new state-of-the-art on the MedNLI dataset. We find that these domain-specific models are not as performant on 2 clinical de-identification tasks, and argue that this is a natural consequence of the differences between de-identified source text and synthetically non de-identified task text.

**clinical-bert(另一团队的版本)**

论文题目：ClinicalBert: Modeling Clinical Notes and Predicting Hospital Readmission

[论文地址](https://arxiv.org/abs/1904.05342)

[项目地址](https://github.com/kexinhuang12345/clinicalBERT)

论文概要：同样基于MIMIC-III数据库,但只随机选取了10万份医疗记录训练的临床领域bert.

论文摘要：Clinical notes contain information about patients that goes beyond structured data like lab values and medications. However, clinical notes have been underused relative to structured data, because notes are high-dimensional and sparse. This work develops and evaluates representations of clinical notes using bidirectional transformers (ClinicalBert). Clini- calBert uncovers high-quality relationships between medical concepts as judged by hu- mans. ClinicalBert outperforms baselines on 30-day hospital readmission prediction using both discharge summaries and the first few days of notes in the intensive care unit. Code and model parameters are available.

**BEHRT**

论文题目：BEHRT: TRANSFORMER FOR ELECTRONIC HEALTH RECORDS

[论文地址](https://arxiv.org/abs/1907.09538)

项目地址: 暂未开源

论文概要：这篇论文中embedding是基于医学实体训练，而不是基于单词。

论文摘要：Today, despite decades of developments in medicine and the growing interest in precision healthcare, vast majority of diagnoses happen once patients begin to show noticeable signs of illness. Early indication and detection of diseases, however, can provide patients and carers with the chance of early intervention, better disease management, and efficient allocation of healthcare resources. The latest developments in machine learning (more specifically, deep learning) provides a great opportunity to address this unmet need. In this study, we introduce BEHRT: A deep neural sequence transduction model for EHR (electronic health records), capable of multitask prediction and disease trajectory mapping. When trained and evaluated on the data from nearly 1.6 million individuals, BEHRT shows a striking absolute improvement of 8.0-10.8%, in terms of Average Precision Score, compared to the existing state-of-the-art deep EHR models (in terms of average precision, when predicting for the onset of 301 conditions). In addition to its superior prediction power, BEHRT provides a personalised view of disease trajectories through its attention mechanism; its flexible architecture enables it to incorporate multiple heterogeneous concepts (e.g., diagnosis, medication, measurements, and more) to improve the accuracy of its predictions; and its (pre-)training results in disease and patient representations that can help us get a step closer to interpretable predictions.

### 2.综述类文章

**nature medicine发表的综述**

论文题目：A guide to deep learning in healthcare

[论文地址](https://www.nature.com/articles/s41591-018-0316-z)

论文概要：发表于nature medicine，包含医学领域下CV,NLP,强化学习等方面的应用综述。

论文摘要：Here we present deep-learning techniques for healthcare, centering our discussion on deep learning in computer vision, natural language processing, reinforcement learning, and generalized methods. We describe how these computational techniques can impact a few key areas of medicine and explore how to build end-to-end systems. Our discussion of computer vision focuses largely on medical imaging, and we describe the application of natural language processing to domains such as electronic health record data. Similarly, reinforcement learning is discussed in the context of robotic-assisted surgery, and generalized deep- learning methods for genomics are reviewed.

### 3.电子病历相关文章

**Transfer Learning from Medical Literature for Section Prediction in Electronic Health Records**

[论文地址](https://www.aclweb.org/anthology/D19-1492/)

论文概要：发表于EMNLP2019。基于少量in-domain数据和大量out-of-domain数据进行EHR相关的迁移学习。

论文摘要：sections such as Assessment and Plan, So- cial History, and Medications. These sec- tions help physicians find information easily and can be used by an information retrieval system to return specific information sought by a user. However, it is common that the exact format of sections in a particular EHR does not adhere to known patterns. There- fore, being able to predict sections and headers in EHRs automatically is beneficial to physi- cians. Prior approaches in EHR section pre- diction have only used text data from EHRs and have required significant manual annota- tion. We propose using sections from med- ical literature (e.g., textbooks, journals, web content) that contain content similar to that found in EHR sections. Our approach uses data from a different kind of source where la- bels are provided without the need of a time- consuming annotation effort. We use this data to train two models: an RNN and a BERT- based model. We apply the learned models along with source data via transfer learning to predict sections in EHRs. Our results show that medical literature can provide helpful su- pervision signal for this classification task.

**MUFASA: Multimodal Fusion Architecture Search for Electronic Health Records**

[论文地址](http://arxiv-download.xixiaoyao.cn/pdf/2102.02340.pdf)

论文概要:发表于AAAI2021。

论文摘要:One important challenge of applying deep learning to electronic health records (EHR) is the complexity of their multimodal structure. EHR usually contains a mixture of structured (codes) and unstructured (free-text) data with sparse and irregular longitudinal features – all of which doctors utilize when making decisions. In the deep learning regime, determining how different modality representations should be fused together is a difficult problem, which is often addressed by handcrafted modeling and intuition. In this work, we extend state-of-the-art neural architecture search (NAS) methods and propose MUltimodal Fusion Architecture SeArch (MUFASA) to simultaneously search across multimodal fusion strategies and modality-specific architectures for the first time. We demonstrate empirically that our MUFASA method outperforms established unimodal NAS on public EHR data with comparable computation costs. In addition, MUFASA produces architectures that outperform Transformer and Evolved Transformer. Compared with these baselines on CCS diagnosis code prediction, our discovered models improve top-5 recall from 0.88 to 0.91 and demonstrate the ability to generalize to other EHR tasks. Studying our top architecture in depth, we provide empirical evidence that MUFASA’s improvements are derived from its ability to both customize modeling for each data modality and find effective fusion strategies.


### 4.医学关系抽取

**Leveraging Dependency Forest for Neural Medical Relation Extraction**

[论文地址](https://www.aclweb.org/anthology/D19-1020/)

论文概要：发表于EMNLP 2019. 基于dependency forest方法，提升对医学语句中依存关系的召回率，同时引进了一部分噪声，基于图循环网络进行特征提取，提供了在医疗关系抽取中使用依存关系，同时减少误差传递的一种思路。

论文摘要：Medical relation extraction discovers relations between entity mentions in text, such as research articles. For this task, dependency syntax has been recognized as a crucial source of features. Yet in the medical domain, 1-best parse trees suffer from relatively low accuracies, diminishing their usefulness. We investigate a method to alleviate this problem by utilizing dependency forests. Forests contain more than one possible decisions and therefore have higher recall but more noise compared with 1-best outputs. A graph neural network is used to represent the forests, automatically distinguishing the useful syntactic information from parsing noise. Results on two benchmarks show that our method outperforms the standard tree-based methods, giving the state-of-the-art results in the literature.

### 5.医学知识图谱

**Learning a Health Knowledge Graph from Electronic Medical Records**

[论文地址](https://www.nature.com/articles/s41598-017-05778-z)

论文概要：发表于nature scientificreports（2017）. 基于27万余份电子病历构建的疾病-症状知识图谱。

论文摘要：Demand for clinical decision support systems in medicine and self-diagnostic symptom checkers has substantially increased in recent years. Existing platforms rely on knowledge bases manually compiled through a labor-intensive process or automatically derived using simple pairwise statistics. This study explored an automated process to learn high quality knowledge bases linking diseases and symptoms directly from electronic medical records. Medical concepts were extracted from 273,174 de-identified patient records and maximum likelihood estimation of three probabilistic models was used to automatically construct knowledge graphs: logistic regression, naive Bayes classifier and a Bayesian network using noisy OR gates. A graph of disease-symptom relationships was elicited from the learned parameters and the constructed knowledge graphs were evaluated and validated, with permission, against Google’s manually-constructed knowledge graph and against expert physician opinions. Our study shows that direct and automated construction of high quality health knowledge graphs from medical records using rudimentary concept extraction is feasible. The noisy OR model produces a high quality knowledge graph reaching precision of 0.85 for a recall of 0.6 in the clinical evaluation. Noisy OR significantly outperforms all tested models across evaluation frameworks (p < 0.01).

### 6.辅助诊断

**Evaluation and accurate diagnoses of pediatric diseases using artificial intelligence**

[论文地址](https://www.nature.com/articles/s41591-018-0335-9)

论文概要：该文章由广州市妇女儿童医疗中心与依图医疗等企业和科研机构共同完成，基于机器学习的自然语言处理（NLP）技术实现不输人类医生的强大诊断能力，并具备多场景的应用能力。据介绍，这是全球首次在顶级医学杂志发表有关自然语言处理（NLP）技术基于电子健康记录（EHR）做临床智能诊断的研究成果，也是利用人工智能技术诊断儿科疾病的重磅科研成果。

论文摘要：Artificial intelligence (AI)-based methods have emerged as powerful tools to transform medical care. Although machine learning classifiers (MLCs) have already demonstrated strong performance in image-based diagnoses, analysis of diverse and massive electronic health record (EHR) data remains challenging. Here, we show that MLCs can query EHRs in a manner similar to the hypothetico-deductive reasoning used by physicians and unearth associations that previous statistical methods have not found. Our model applies an automated natural language processing system using deep learning techniques to extract clinically relevant information from EHRs. In total, 101.6 million data points from 1,362,559 pediatric patient visits presenting to a major referral center were analyzed to train and validate the framework. Our model demonstrates high diagnostic accuracy across multiple organ systems and is comparable to experienced pediatricians in diagnosing common childhood diseases. Our study provides a proof of concept for implementing an AI-based system as a means to aid physicians in tackling large amounts of data, augmenting diagnostic evaluations, and to provide clinical decision support in cases of diagnostic uncertainty or complexity. Although this impact may be most evident in areas where healthcare providers are in relative shortage, the benefits of such an AI system are likely to be universal.

### 7.ACL2020医学领域相关论文列表

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

### 8.医疗实体Linking（标准化）

**Medical Entity Linking using Triplet Network**

[论文地址](https://www.aclweb.org/anthology/W19-1912/)

论文概要： 发表于ACL2019,论文内容为疾病实体Linking研究。使用三元组数据，（mention，正例，负例），目标使distance(mention,负例)-distance(mention,正例)>alpha（人脸识别的经典方案）,具体损失函数参看论文。论文主要包括两部分内容1）候选数据集生成,对给定mention，与标准疾病集合数据（标准词及同义词）计算余弦相似度及Jaccard overlap分数,取topK作为候选样例。 2）网络结构基于Triplet Network。详见论文。

**A Generate-and-Rank Framework with Semantic Type Regularization for Biomedical Concept Normalization**

[论文地址](https://www.aclweb.org/anthology/2020.acl-main.748.pdf)

论文概要: 发表于ACL2020。基于list-wise排序学习方法。主要分为两部分：后续数据集生成 和  基于BERT的list-wise排序。较新颖的思路：1）在样本生成过程中，对标准词进行了基于同义词的扩展。2）在loss中引入了语义类型正则化。详见论文。

**Deep Neural Models for Medical Concept Normalization in User-Generated Texts**

[论文地址](https://www.aclweb.org/anthology/P19-2055.pdf)


### 9. AAAI2020 医学NLP相关论文列表

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

### 10. EMNLP2020 医学NLP相关论文列表

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


## 中文医疗领域语料

### 医学教材+培训考试 

说明:由于版权原因，现在无法提供度盘下载链接了，请大家前往原豆瓣链接下载吧。

语料说明：根据此[豆瓣链接](https://www.douban.com/note/692003915/)整理。

数据预览：

![image](https://github.com/lrs1353281004/Chinese_medical_NLP/blob/master/images/pretrain_overview.png)

### 哈工大《大词林》开放75万核心实体词及相关概念、关系列表（包含中药/医院/生物 类别）

语料说明:哈工大开源了《大词林》中的75万的核心实体词，以及这些核心实体词对应的细粒度概念词（共1.8万概念词，300万实体-概念元组），还有相关的关系三元组（共300万）。这75万核心实体列表涵盖了常见的人名、地名、物品名等术语。概念词列表则包含了细粒度的实体概念信息。借助于细粒度的上位概念层次结构和丰富的实体间关系，本次开源的数据能够为人机对话、智能推荐、等应用技术提供数据支持。

[语料官方下载地址](http://101.200.120.155/browser/)

说明: 通过网上查询，这部分资源应该是被一些公司付费使用了，可能有版权问题，所以现在下载链接都失效了。后续如果再有开源的信息再进行更新。

## 医学embedding及预训练模型

### 开源英文医学embedding

项目说明：发表于AMIA 2016. 开源医学相关概念embedding. 

[项目地址](https://github.com/clinicalml/embeddings)

### MC-BERT中文医疗预训练模型

论文名称：Conceptualized Representation Learning for Chinese Biomedical Text Mining

[项目地址](https://github.com/alibaba-research/ChineseBLUE)

[解读文章](https://zhuanlan.zhihu.com/p/208721884)

## 开源工具包

### 分词工具

#### PKUSEG

[项目地址](https://github.com/lancopku/pkuseg-python)

项目说明： 北京大学推出的多领域中文分词工具，支持选择医学领域。

## 工业级产品解决方案

[灵医智慧](https://01.baidu.com/index.html)

[左手医生](https://open.zuoshouyisheng.com/)

[医渡云研究院-医学自然语言处理](https://www.yiducloud.com.cn/academy.html)

[百度-医学文本结构化](https://ai.baidu.com/solution/mtp)

[阿里云-医学自然语言处理](https://help.aliyun.com/document_detail/179395.html)

## blog分享

[医疗领域构建自然语言处理系统的经验教训](http://www.oreilly.com.cn/radar/?p=2083)

[大数据时代的医学公共数据库与数据挖掘技术简介](https://mp.weixin.qq.com/s/tA44U4bJUttnROfrzpNYcQ)

[从ACL 2021中看NLP在医疗领域应用的发展，附资源下载](https://mp.weixin.qq.com/s/RhcHvRWHRnYUg6u9vXoIGA)

## 友情链接

[awesome_Chinese_medical_NLP](https://github.com/GanjinZero/awesome_Chinese_medical_NLP)

[中文NLP数据集搜索](https://www.cluebenchmarks.com/dataSet_search.html)

[medical-data(海量医疗相关数据)](https://github.com/beamandrew/medical-data)

[天池数据集(其中包含多个医疗NLP数据集)](https://tianchi.aliyun.com/dataset)

