# Chinese_medical_NLP
医疗NLP领域（主要关注中文）   评测数据集 与 论文列表

## 评测数据集

### 1. Yidu-S4K：医渡云结构化4K数据集
数据集描述：
> Yidu-S4K 数据集源自CCKS 2019 评测任务一，即“面向中文电子病历的命名实体识别”的数据集，包括两个子任务：
1）医疗命名实体识别：由于国内没有公开可获得的面向中文电子病历医疗实体识别数据集，本年度保留了医疗命名实体识别任务，对2017年度数据集做了修订，并随任务一同发布。本子任务的数据集包括训练集和测试集。
2）医疗实体及属性抽取（跨院迁移）：在医疗实体识别的基础上，对预定义实体属性进行抽取。本任务为迁移学习任务，即在只提供目标场景少量标注数据的情况下，通过其他场景的标注数据及非标注数据进行目标场景的识别任务。本子任务的数据集包括训练集（非目标场景和目标场景的标注数据、各个场景的非标注数据）和测试集（目标场景的标注数据

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

## 相关论文

### 1.医疗领域预训练embedding
注：目前没有收集到中文医疗领域的开源预训练模型，以下列出英文论文供参考。

#### Bio-bert
论文题目：BioBERT: a pre-trained biomedical language representation model for biomedical text mining

[论文地址](https://academic.oup.com/bioinformatics/advance-article/doi/10.1093/bioinformatics/btz682/5566506)

[项目地址](https://github.com/dmis-lab/biobert)

论文概要：以通用领域预训练bert为初始权重，基于Pubmed上大量医疗领域英文论文训练。在多个医疗相关下游任务中超越SOTA模型的表现。

论文摘要：
> **Motivation**: Biomedical text mining is becoming increasingly important as the number of biomedical documents rapidly grows. With the progress in natural language processing (NLP), extracting valuable information from bio- medical literature has gained popularity among researchers, and deep learning has boosted the development of ef- fective biomedical text mining models. However, directly applying the advancements in NLP to biomedical text min- ing often yields unsatisfactory results due to a word distribution shift from general domain corpora to biomedical corpora. In this article, we investigate how the recently introduced pre-trained language model BERT can be adapted for biomedical corpora. 
**Results**: We introduce BioBERT (Bidirectional Encoder Representations from Transformers for Biomedical Text Mining), which is a domain-specific language representation model pre-trained on large-scale biomedical corpora. With almost the same architecture across tasks, BioBERT largely outperforms BERT and previous state-of-the-art models in a variety of biomedical text mining tasks when pre-trained on biomedical corpora. While BERT obtains performance comparable to that of previous state-of-the-art models, BioBERT significantly outperforms them on the following three representative biomedical text mining tasks: biomedical named entity recognition (0.62% F1 score improvement), biomedical relation extraction (2.80% F1 score improvement) and biomedical question answering (12.24% MRR improvement). Our analysis results show that pre-training BERT on biomedical corpora helps it to understand complex biomedical texts. 
**Availability and implementation**: We make the pre-trained weights of BioBERT freely available at https://github.com/naver/biobert-pretrained, and the source code for fine-tuning BioBERT available at https://github.com/dmis-lab/biobert.

#### sci-bert
论文题目：SCIBERT: A Pretrained Language Model for Scientific Text

[论文地址](https://arxiv.org/abs/1903.10676)

[项目地址](https://github.com/allenai/scibert/)

论文概要：AllenAI 团队出品.基于Semantic Scholar 上 110万+ 文章训练的 科学领域bert.

论文摘要：Obtaining large-scale annotated data for NLP tasks in the scientific domain is challeng- ing and expensive. We release SCIBERT, a pretrained language model based on BERT (Devlin et al., 2019) to address the lack of high-quality, large-scale labeled scientific data. SCIBERT leverages unsupervised pretraining on a large multi-domain corpus of scientific publications to improve perfor- mance on downstream scientific NLP tasks. We evaluate on a suite of tasks including sequence tagging, sentence classification and dependency parsing, with datasets from a variety of scientific domains. We demon- strate statistically significant improvements over BERT and achieve new state-of-the- art results on several of these tasks. The code and pretrained models are available at https://github.com/allenai/scibert/.

#### clinical-bert
论文题目：Publicly Available Clinical BERT Embeddings

[论文地址](https://www.aclweb.org/anthology/W19-1909/)

[项目地址](https://github.com/EmilyAlsentzer/clinicalBERT)

论文概要：出自NAACL Clinical NLP Workshop 2019.基于MIMIC-III数据库中的200万份医疗记录训练的临床领域bert.

论文摘要：Contextual word embedding models such as ELMo and BERT have dramatically improved performance for many natural language processing (NLP) tasks in recent months. However, these models have been minimally explored on specialty corpora, such as clinical text; moreover, in the clinical domain, no publicly-available pre-trained BERT models yet exist. In this work, we address this need by exploring and releasing BERT models for clinical text: one for generic clinical text and another for discharge summaries specifically. We demonstrate that using a domain-specific model yields performance improvements on 3/5 clinical NLP tasks, establishing a new state-of-the-art on the MedNLI dataset. We find that these domain-specific models are not as performant on 2 clinical de-identification tasks, and argue that this is a natural consequence of the differences between de-identified source text and synthetically non de-identified task text.

#### clinical-bert(另一团队的版本)
论文题目：ClinicalBert: Modeling Clinical Notes and Predicting Hospital Readmission

[论文地址](https://arxiv.org/abs/1904.05342)

[项目地址](https://github.com/kexinhuang12345/clinicalBERT)

论文概要：同样基于MIMIC-III数据库,但只随机选取了10万份医疗记录训练的临床领域bert.

论文摘要：Clinical notes contain information about patients that goes beyond structured data like lab values and medications. However, clinical notes have been underused relative to structured data, because notes are high-dimensional and sparse. This work develops and evaluates representations of clinical notes using bidirectional transformers (ClinicalBert). Clini- calBert uncovers high-quality relationships between medical concepts as judged by hu- mans. ClinicalBert outperforms baselines on 30-day hospital readmission prediction using both discharge summaries and the first few days of notes in the intensive care unit. Code and model parameters are available.

#### BEHRT
论文题目：BEHRT: TRANSFORMER FOR ELECTRONIC HEALTH RECORDS

[论文地址](https://arxiv.org/abs/1907.09538)

项目地址: 暂未开源

论文概要：这篇论文中embedding是基于医学实体训练，而不是基于单词。

论文摘要：Today, despite decades of developments in medicine and the growing interest in precision healthcare, vast majority of diagnoses happen once patients begin to show noticeable signs of illness. Early indication and detection of diseases, however, can provide patients and carers with the chance of early intervention, better disease management, and efficient allocation of healthcare resources. The latest developments in machine learning (more specifically, deep learning) provides a great opportunity to address this unmet need. In this study, we introduce BEHRT: A deep neural sequence transduction model for EHR (electronic health records), capable of multitask prediction and disease trajectory mapping. When trained and evaluated on the data from nearly 1.6 million individuals, BEHRT shows a striking absolute improvement of 8.0-10.8%, in terms of Average Precision Score, compared to the existing state-of-the-art deep EHR models (in terms of average precision, when predicting for the onset of 301 conditions). In addition to its superior prediction power, BEHRT provides a personalised view of disease trajectories through its attention mechanism; its flexible architecture enables it to incorporate multiple heterogeneous concepts (e.g., diagnosis, medication, measurements, and more) to improve the accuracy of its predictions; and its (pre-)training results in disease and patient representations that can help us get a step closer to interpretable predictions.

### 2.综述类文章

#### nature medicine发表的综述
论文题目：A guide to deep learning in healthcare

[论文地址](https://www.nature.com/articles/s41591-018-0316-z)

论文概要：发表于nature medicine，包含医学领域下CV,NLP,强化学习等方面的应用综述。

论文摘要：Here we present deep-learning techniques for healthcare, centering our discussion on deep learning in computer vision, natural language processing, reinforcement learning, and generalized methods. We describe how these computational techniques can impact a few key areas of medicine and explore how to build end-to-end systems. Our discussion of computer vision focuses largely on medical imaging, and we describe the application of natural language processing to domains such as electronic health record data. Similarly, reinforcement learning is discussed in the context of robotic-assisted surgery, and generalized deep- learning methods for genomics are reviewed.

### 3.电子病历相关文章

#### Transfer Learning from Medical Literature for Section Prediction in Electronic Health Records

[论文地址](https://www.aclweb.org/anthology/D19-1492/)

论文概要：发表于EMNLP2019。基于少量in-domain数据和大量out-of-domain数据进行EHR相关的迁移学习。

论文摘要：sections such as Assessment and Plan, So- cial History, and Medications. These sec- tions help physicians find information easily and can be used by an information retrieval system to return specific information sought by a user. However, it is common that the exact format of sections in a particular EHR does not adhere to known patterns. There- fore, being able to predict sections and headers in EHRs automatically is beneficial to physi- cians. Prior approaches in EHR section pre- diction have only used text data from EHRs and have required significant manual annota- tion. We propose using sections from med- ical literature (e.g., textbooks, journals, web content) that contain content similar to that found in EHR sections. Our approach uses data from a different kind of source where la- bels are provided without the need of a time- consuming annotation effort. We use this data to train two models: an RNN and a BERT- based model. We apply the learned models along with source data via transfer learning to predict sections in EHRs. Our results show that medical literature can provide helpful su- pervision signal for this classification task.




## 中文医疗领域语料

### 医学教材+培训考试 （共57G）

语料说明：根据此[豆瓣链接](https://www.douban.com/note/692003915/)整理。整合到一个文件夹内，便于保存。去掉了其中视频部分。

数据预览：

![image](https://github.com/lrs1353281004/Chinese_medical_NLP/blob/master/images/pretrain_overview.png)



度盘下载地址：https://pan.baidu.com/s/1P2WHX7hNTqErZ3j1vhkr_Q

提取码：xd0c
