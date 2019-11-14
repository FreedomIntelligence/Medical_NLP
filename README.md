# Chinese_medical_NLP
医疗NLP领域（主要关注中文）   评测数据集 与 论文列表

## 评测数据集

### 1. Yidu-S4K：医渡云结构化4K数据集
数据集描述：
> Yidu-S4K 数据集源自CCKS 2019 评测任务一，即“面向中文电子病历的命名实体识别”的数据集，包括两个子任务：
1）医疗命名实体识别：由于国内没有公开可获得的面向中文电子病历医疗实体识别数据集，本年度保留了医疗命名实体识别任务，对2017年度数据集做了修订，并随任务一同发布。本子任务的数据集包括训练集和测试集。
2）医疗实体及属性抽取（跨院迁移）：在医疗实体识别的基础上，对预定义实体属性进行抽取。本任务为迁移学习任务，即在只提供目标场景少量标注数据的情况下，通过其他场景的标注数据及非标注数据进行目标场景的识别任务。本子任务的数据集包括训练集（非目标场景和目标场景的标注数据、各个场景的非标注数据）和测试集（目标场景的标注数据

[数据集地址](http://openkg.cn/dataset/yidu-s4k)

度盘下载地址：待添加

提取码：待添加

### 2.瑞金医院糖尿病数据集
数据集描述：
>此数据集旨在通过糖尿病相关的教科书、研究论文来做糖尿病文献挖掘并构建糖尿病知识图谱。参赛选手需要设计高准确率，高效的算法来挑战这一科学难题。第一赛季课题为“基于糖尿病临床指南和研究论文的实体标注构建”，第二赛季课题为“基于糖尿病临床指南和研究论文的实体间关系构建”。

官方提供的数据只包含训练集，真正用于最终排名的测试集没有给出。

[数据集地址](https://tianchi.aliyun.com/competition/entrance/231687/information)

度盘下载地址：待添加

提取码：待添加

## 相关论文

### 1.医疗领域预训练embedding
注：目前没有收集到中文医疗领域的开源预训练模型，以下列出英文论文供参考。

#### Bio-bert
[论文地址](https://academic.oup.com/bioinformatics/advance-article/doi/10.1093/bioinformatics/btz682/5566506)

[项目地址](https://github.com/dmis-lab/biobert)

论文概要：以通用领域预训练bert为初始权重，基于Pubmed上大量医疗领域英文论文训练。在多个医疗相关下游任务中超越SOTA模型的表现。

论文摘要：
> **Motivation**: Biomedical text mining is becoming increasingly important as the number of biomedical documents rapidly grows. With the progress in natural language processing (NLP), extracting valuable information from bio- medical literature has gained popularity among researchers, and deep learning has boosted the development of ef- fective biomedical text mining models. However, directly applying the advancements in NLP to biomedical text min- ing often yields unsatisfactory results due to a word distribution shift from general domain corpora to biomedical corpora. In this article, we investigate how the recently introduced pre-trained language model BERT can be adapted for biomedical corpora. 
**Results**: We introduce BioBERT (Bidirectional Encoder Representations from Transformers for Biomedical Text Mining), which is a domain-specific language representation model pre-trained on large-scale biomedical corpora. With almost the same architecture across tasks, BioBERT largely outperforms BERT and previous state-of-the-art models in a variety of biomedical text mining tasks when pre-trained on biomedical corpora. While BERT obtains performance comparable to that of previous state-of-the-art models, BioBERT significantly outperforms them on the following three representative biomedical text mining tasks: biomedical named entity recognition (0.62% F1 score improvement), biomedical relation extraction (2.80% F1 score improvement) and biomedical question answering (12.24% MRR improvement). Our analysis results show that pre-training BERT on biomedical corpora helps it to understand complex biomedical texts. 
**Availability and implementation**: We make the pre-trained weights of BioBERT freely available at https://github.com/naver/biobert-pretrained, and the source code for fine-tuning BioBERT available at https://github.com/dmis-lab/biobert.
