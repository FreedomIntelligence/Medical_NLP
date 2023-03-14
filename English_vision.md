# Medical_NLP


>Since [Cris Lee](https://github.com/lrs1353281004) left the medical NLP field in 2021, this repo is now maintained by [Xidong Wang](https://github.com/wangxidong06).

Summary of medical NLP evaluations/competitions, datasets, papers and pre-trained models.

[中文版本](https://github.com/FreedomIntelligence/Chinese_medical_NLP) [English_version](https://github.com/FreedomIntelligence/Chinese_medical_NLP/blob/master/English_vision.md)

* [Medical_NLP](#medical_nlp)
   * [一. Evaluation/Competition](#一-evaluationcompetition)
      * [1. Ongoing Contests:](#1-ongoing-contests)
         * [1.1 Chinese: Imaging NLP ——Medical Imaging Diagnostic Report Generation](#11-chinese-imaging-nlp-medical-imaging-diagnostic-report-generation)
         * [1.2 English: BioNLP Workshop 2023 Shared tasks](#12-english-bionlp-workshop-2023-shared-tasks)
         * [1.3 English: MedVidQA 2023](#13-english-medvidqa-2023)
         * [1.4 Chinese (long-term effective): Medical information processing challenge list CBLUE dataset](#14-chinese-long-term-effective-medical-information-processing-challenge-list-cblue-dataset)
      * [2. Ended assessments/competitions (starting in 2021):](#2-ended-assessmentscompetitions-starting-in-2021)
         * [2.1 Chinese: Simple Triage Challenge for Non-Standardized Disease Claims 2.0](#21-chinese-simple-triage-challenge-for-non-standardized-disease-claims-20)
         * [2.2 Chinese: Evaluation tasks of the 8th China Health Information Processing Conference (CHIP2022)](#22-chinese-evaluation-tasks-of-the-8th-china-health-information-processing-conference-chip2022)
         * [2.3 Chinese: HKUST Xunfei-Medical Entity and Relationship Recognition Challenge](#23-chinese-hkust-xunfei-medical-entity-and-relationship-recognition-challenge)
         * [2.4 Chinese: The First Intelligent Dialogue Diagnosis and Treatment Evaluation Competition (CCL 2021)](#24-chinese-the-first-intelligent-dialogue-diagnosis-and-treatment-evaluation-competition-ccl-2021)
         * [2.5 English: MEDIQA-2021](#25-english-mediqa-2021)
         * [2.6 英文： ICLR-2021-医疗对话生成与自动诊断国际竞赛](#26-英文-iclr-2021-医疗对话生成与自动诊断国际竞赛)
   * [二. data set](#二-data-set)
      * [1. Chinese dataset](#1-chinese-dataset)
         * [1.1 Chinese doctor-patient Q&amp;A dialogue data (1.1M)](#11-chinese-doctor-patient-qa-dialogue-data-11m)
         * [1.2 Chinese Medical Dialogue Dataset (792K)](#12-chinese-medical-dialogue-dataset-792k)
         * [1.3 CPubMed-KG (4.4M triplets)](#13-cpubmed-kg-44m-triplets)
         * [1.4 CBLUE evaluation](#14-cblue-evaluation)
         * [1.5 Chinese Medical Knowledge Graph CMeKG (1M triples)](#15-chinese-medical-knowledge-graph-cmekg-1m-triples)
         * [1.6 cMedQA2 (108K)](#16-cmedqa2-108k)
         * [1.7 xywy-KG (294K triplets)](#17-xywy-kg-294k-triplets)
         * [1.8 39Health-KG (210K triplets)](#18-39health-kg-210k-triplets)
         * [1.9 Evaluation of CHIP over the years (official evaluation)](#19-evaluation-of-chip-over-the-years-official-evaluation)
         * [1.10 Ruijin Hospital Diabetes Dataset (Diabetes)](#110-ruijin-hospital-diabetes-dataset-diabetes)
         * [1.11 Tianchi COVID-19 Question Matching Competition (COVID-19)](#111-tianchi-covid-19-question-matching-competition-covid-19)
      * [2. Knowledge and information sources commonly used by Chinese clinicians](#2-knowledge-and-information-sources-commonly-used-by-chinese-clinicians)
         * [2.1 pubMed](#21-pubmed)
         * [2.2 Up-to-date](#22-up-to-date)
         * [2.3clinical guidelines](#23clinical-guidelines)
         * [2.4 medication assistant](#24-medication-assistant)
         * [2.5 Lilac Garden](#25-lilac-garden)
         * [2.6 Doctor Lilac](#26-doctor-lilac)
      * [3. English dataset](#3-english-dataset)
         * [3.1 PubMedQA](#31-pubmedqa)
         * [3.2 COMETA](#32-cometa)
         * [3.3 MedMentions](#33-medmentions)
   * [三. Open source pre-trained model](#三-open-source-pre-trained-model)
      * [1. Existing Medical NLP large model](#1-existing-medical-nlp-large-model)
         * [1.1 BioMedLM (2.7B)](#11-biomedlm-27b)
         * [1.2 BioGPT  (1.5B)](#12-biogpt--15b)
         * [1.3 Medical-chatgpt](#13-medical-chatgpt)
         * [1.4 BioBERT](#14-biobert)
         * [1.5 PubMedBERT](#15-pubmedbert)
      * [2.Other large models in Chinese that can be fine-tuned in the medical field](#2other-large-models-in-chinese-that-can-be-fine-tuned-in-the-medical-field)
         * [2.1 <a href="https://github.com/lonePatient/awesome-pretrained-chinese-nlp-models#GPT">Awesome List</a>](#21-awesome-list)
         * [2.2 Model parameter scale 0B-5B:](#22-model-parameter-scale-0b-5b)
            * [2.2.1 <a href="https://github.com/Langboat/Mengzi">Mencius (1B)</a>](#221-mencius-1b)
            * [2.2.2 <a href="https://github.com/THUDM/glm">GLM-2b</a>](#222-glm-2b)
            * [2.2.3 <a href="https://github.com/TsinghuaAI/CPM-1-Generate">CPM-1(2.6B)</a>](#223-cpm-126b)
            * [2.2.4 <a href="https://github.com/imcaspar/gpt2-ml">gpt2-ml(1.5B)</a>](#224-gpt2-ml15b)
            * [2.2.5 <a href="https://openi.pcl.ac.cn/PCL-Platform.Intelligence/PanGu-Alpha" rel="nofollow">Pangu-Alpha(2.6B)</a>](#225-pangu-alpha26b)
            * [2.2.6 <a href="https://github.com/THUDM/Chinese-Transformer-XL">Chinese-Transformer-XL(2.9B)</a>](#226-chinese-transformer-xl29b)
         * [2.3 Model parameter scale 5B-10B:](#23-model-parameter-scale-5b-10b)
            * [2.3.1 <a href="https://github.com/THUDM/ChatGLM-6B"><strong>ChatGLM-6B</strong></a>](#231-chatglm-6b)
            * [2.3.2 <a href="https://github.com/tatsu-lab/stanford_alpaca">Stanford Alpaca(7B)</a>](#232-stanford-alpaca7b)
            * [2.3.2 <a href="https://github.com/THUDM/glm">GLM-10B</a>](#232-glm-10b)
            * [2.3.3 <a href="https://github.com/PaddlePaddle/ERNIE">ERNIE3.0(10B)</a>](#233-ernie3010b)
         * [2.4 Model parameter scale 10B-100B:](#24-model-parameter-scale-10b-100b)
            * [2.4.1 <a href="https://openi.pcl.ac.cn/PCL-Platform.Intelligence/PanGu-Alpha" rel="nofollow">Pangu-Alpha(13B)</a>](#241-pangu-alpha13b)
            * [2.4.2 <a href="https://github.com/TsinghuaAI/CPM-2-Finetune">CPM-2(11B)</a>](#242-cpm-211b)
         * [2.5 Model parameter size 100B--:](#25-model-parameter-size-100b--)
            * [2.5.1 <a href="https://github.com/THUDM/GLM-130B"><strong>GLM-130B</strong></a> SHOW respects to those guys who firmly overcome difficulties and finally realize the project and selflessly share [detailed experience](https ://keg.cs.tsinghua.edu.cn/glm-130b/zh/posts/glm-130b)  !](#251-glm-130b-show-respects-to-those-guys-who-firmly-overcome-difficulties-and-finally-realize-the-project-and-selflessly-share-detailed-experiencehttps-kegcstsinghuaeducnglm-130bzhpostsglm-130b--)
            * [2.5.2 <a href="https://openi.pcl.ac.cn/BAAI/WuDao-Model/src/branch/master/CPM" rel="nofollow">CPM-2-MoE(198B)</a>](#252-cpm-2-moe198b)
            * [2.5.3 <a href="https://openi.pcl.ac.cn/PCL-Platform.Intelligence/PanGu-Alpha" rel="nofollow">Pangu-Alpha(200B)</a>](#253-pangu-alpha200b)
            * [2.5.4 <a href="https://github.com/Shawn-Inspur/Yuan-1.0">Source 1.0(245B)</a>](#254-source-10245b)
   * [四. Related Papers](#四-related-papers)
      * [1. Papers that may be helpful in the post-ChatGPT era (continuously updated)](#1-papers-that-may-be-helpful-in-the-post-chatgpt-era-continuously-updated)
         * [1.1 <strong>ChatGPT Performance on USMLE</strong>: The Potential of Using Large Language Models for AI-Assisted Medical Education](#11-chatgpt-performance-on-usmle-the-potential-of-using-large-language-models-for-ai-assisted-medical-education)
         * [1.2 Conducting a (Turing) Test on <strong>ChatGPT's Medical Advice</strong>](#12-conducting-a-turing-test-on-chatgpts-medical-advice)
         * [1.3 <strong>Toolformer</strong>: The language model can learn to use tools by itself](#13-toolformer-the-language-model-can-learn-to-use-tools-by-itself)
         * [1.4 Check your facts and try again: <strong>Leverage external knowledge and automatic feedback to improve large language models</strong>](#14-check-your-facts-and-try-again-leverage-external-knowledge-and-automatic-feedback-to-improve-large-language-models)
      * [2 Review articles](#2-review-articles)
         * [1. Pretrained Language Models in Biomedical Domains: A Systematic Survey](#1-pretrained-language-models-in-biomedical-domains-a-systematic-survey)
         * [2. A Guide to Deep Learning in Healthcare](#2-a-guide-to-deep-learning-in-healthcare)
      * [3. Summary and archive of papers in the warehouse before 2021](#3-summary-and-archive-of-papers-in-the-warehouse-before-2021)
         * [3.1 Electronic medical records related articles](#31-electronic-medical-records-related-articles)
         * [3.2 Medical relationship extraction](#32-medical-relationship-extraction)
         * [3.4 Auxiliary diagnosis](#34-auxiliary-diagnosis)
         * [3.5 ACL2020 list of related papers in the medical field](#35-acl2020-list-of-related-papers-in-the-medical-field)
         * [3.6 Medical entity Linking (standardization)](#36-medical-entity-linking-standardization)
         * [3.7 List of AAAI2020 medical NLP related papers](#37-list-of-aaai2020-medical-nlp-related-papers)
         * [3.8 EMNLP2020 Medical NLP related papers list](#38-emnlp2020-medical-nlp-related-papers-list)
   * [5. Open source toolkit](#5-open-source-toolkit)
      * [1. Word segmentation tool: PKUSEG](#1-word-segmentation-tool-pkuseg)
   * [6. Industrial-grade product solutions](#6-industrial-grade-product-solutions)
      * [1. <a href="https://01.baidu.com/index.html" rel="nofollow">Spiritual Doctor Wisdom</a>](#1-spiritual-doctor-wisdom)
      * [2. <a href="https://open.zuoshouyisheng.com/" rel="nofollow">Left-handed doctor</a>](#2-left-handed-doctor)
      * [3. <a href="https://www.yiducloud.com.cn/academy.html" rel="nofollow">Yidu Cloud Academy - Medical Natural Language Processing</a>](#3-yidu-cloud-academy---medical-natural-language-processing)
      * [4. <a href="https://ai.baidu.com/solution/mtp" rel="nofollow">Baidu-Medical Text Structured</a>](#4-baidu-medical-text-structured)
      * [5. <a href="https://help.aliyun.com/document_detail/179395.html" rel="nofollow">Alibaba Cloud - Medical Natural Language Processing</a>](#5-alibaba-cloud---medical-natural-language-processing)
   * [7. Blog sharing](#7-blog-sharing)
      * [1. Blogs that may be helpful in the post-ChatGPT era (continuously updated)](#1-blogs-that-may-be-helpful-in-the-post-chatgpt-era-continuously-updated)
         * [1.1 <a href="https://crfm.stanford.edu/2023/03/13/alpaca.html" rel="nofollow">Alpaca: A Powerful Open Source Instruction Following Model</a>](#11-alpaca-a-powerful-open-source-instruction-following-model)
      * [2. Warehouse blog sharing archive before 2021](#2-warehouse-blog-sharing-archive-before-2021)
         * [2.1 <a href="http://www.oreilly.com.cn/radar/?p=2083" rel="nofollow">Experiences and lessons of building natural language processing systems in the medical field</a>](#21-experiences-and-lessons-of-building-natural-language-processing-systems-in-the-medical-field)
         * [2.2 <a href="https://mp.weixin.qq.com/s/tA44U4bJUttnROfrzpNYcQ" rel="nofollow">Introduction to Medical Public Database and Data Mining Technology in the Big Data Era</a>](#22-introduction-to-medical-public-database-and-data-mining-technology-in-the-big-data-era)
         * [2.3 <a href="https://mp.weixin.qq.com/s/RhcHvRWHRnYUg6u9vXoIGA" rel="nofollow">See the development of NLP in the medical field from ACL 2021, with resource download attached</a>](#23-see-the-development-of-nlp-in-the-medical-field-from-acl-2021-with-resource-download-attached)
   * [8. Friendship Links](#8-friendship-links)
      * [1. <a href="https://github.com/GanjinZero/awesome_Chinese_medical_NLP">awesome_Chinese_medical_NLP</a>](#1-awesome_chinese_medical_nlp)
      * [2. <a href="https://www.cluebenchmarks.com/dataSet_search.html" rel="nofollow">Chinese NLP Dataset Search</a>](#2-chinese-nlp-dataset-search)
      * [3. <a href="https://github.com/beamandrew/medical-data">medical-data (massive medical-related data)</a>](#3-medical-data-massive-medical-related-data)
      * [4. <a href="https://tianchi.aliyun.com/dataset" rel="nofollow">Tianchi data set (which contains multiple medical NLP data sets)</a>](#4-tianchi-data-set-which-contains-multiple-medical-nlp-data-sets)


## 一. Evaluation/Competition

### 1. Ongoing Contests:

#### 1.1 Chinese: Imaging NLP ——Medical Imaging Diagnostic Report Generation

- Source: 2023 Global Artificial Intelligence Technology Innovation Competition Track 1
- Introduction: The task of this track requires the participating teams to generate a diagnosis report text based on the doctor's description text data of the CT image (that is, the description of the characteristics of the medical image). Different from traditional text generation tasks, the content of medical imaging diagnosis reports is professional, clear and discrete, so targeted algorithm and model design is also required. The report generation results are evaluated and ranked according to the specified evaluation indicators, and the one with the best score wins.
- [Official address](https://gaiic.caai.cn/ai2023/)

#### 1.2 English: BioNLP Workshop 2023 Shared tasks

[Official address](https://aclweb.org/aclwiki/BioNLP_Workshop#SHARED_TASKS_2023)

- 1A：Question List Summary
  - Introduction: Automatically summarizing patients' major concerns from daily care notes in electronic health records helps alleviate clinicians' information and cognitive overload and provides augmented intelligence through computerized diagnostic decision support at the bedside. The Problem List Summarization task is designed to generate a list of diagnoses and problems in a patient's day-to-day care plan using the provider's progress record input during the hospital stay.
  - [Details](https://physionet.org/content/bionlp-workshop-2023-task-1a/1.0.0/)
- 1B：Radiology Report Summary
  - Introduction: The field of research in abstracts of radiology reports currently faces an important limitation: most studies have been performed on chest radiographs. To alleviate these limitations, we propose two datasets: a shared summarization task, including six different patterns and anatomical structures, with a total of 79,779 samples, based on the MIMIC-III database. A shared summarization task on chest X-ray radiology reports with images from Stanford University and a new out-of-domain test set.
  - [Details](https://vilmedic.app/misc/bionlp23/sharedtask)
- 2：Layman's Summary of Biomedical Research Articles
  - Introduction: Biomedical publications contain the latest research on prominent topics related to health, from common diseases to global epidemics. This often results in their content being of interest to a broad audience, including researchers, medical professionals, journalists, and even the general public. However, the highly technical and technical language used in such articles often makes it difficult for a lay audience to understand the content. Thus, these models have the potential to help expand access to highly technical documents when they are trained to generate summaries that are more readable, contain more background information and less technical jargon (i.e., “layman summaries”). This common mission revolves around abstract summaries of biomedical research articles, emphasizing manageability and catering to non-specialist audiences.
  - [Details](https://biolaysumm.org/)

#### 1.3 English: MedVidQA 2023

- Source: National Institutes of Health
- Introduction: The explosion in the availability of online video has changed the way information and knowledge are acquired. In a similar manner, medical instructional videos are more suitable and beneficial for delivering key information through visual and verbal communication to consumers on healthcare issues that require guidance. This task consists of two main tasks: Video Corpus Visual Answer Localization (VCVAL) and Medical Instructional Question Generation (MIQG).
- [Official Address](https://medvidqa.github.io/index.html)

#### 1.4 Chinese (long-term effective): Medical information processing challenge list CBLUE dataset

- CBLUE 1.0：
  - Source: The Medical Health and Bioinformatics Professional Committee of the Chinese Information Society of China was initiated under the concept of legal openness and sharing, undertaken by Alibaba Cloud Tianchi Platform, and co-sponsored by Yidu Cloud (Beijing) Technology Co., Ltd., Ping An Medical Technology, Peking University, Zhengzhou The University, Pengcheng Laboratory, Harbin Institute of Technology (Shenzhen), Tongji University, Quark, Alibaba Dharma Institute and other units that carry out smart medical research are co-organized to promote the development of Chinese medical NLP technology and communities. **It is composed of the previous academic evaluation competitions of the CHIP conference and the data sets of Ali Quark's medical search business.**
  - Introduction: Covers 4 common medical information processing tasks of medical text information extraction (entity recognition, relationship extraction), medical term normalization, medical text classification, and medical sentence semantic correlation determination, and contains 8 subtasks in total.
- CBLUE 2.0：
  - Source: Compared with 1.0, Fudan University, Tencent Tianyan Lab and Sun Yat-sen University were added.
  - Introduction: Covers 5 common medical information processing tasks including medical text information extraction (entity recognition, relationship extraction), medical terminology normalization, medical text classification, medical sentence semantic correlation determination, medical dialogue understanding and generation, including 15 subtasks.
    - For detailed comparison, please refer to https://zhuanlan.zhihu.com/p/469465499

- [CBLUE evaluation official address](https://tianchi.aliyun.com/dataset/dataDetail?dataId=95414)
- [Paper Address](https://arxiv.org/abs/2106.08087)
- [Github project address](https://github.com/CBLUEbenchmark/CBLUE)

### 2. Ended assessments/competitions (starting in 2021):

> This section contains evaluations/competitions starting from 2021.2.20 Arranged in reverse chronological order

#### 2.1 Chinese: Simple Triage Challenge for Non-Standardized Disease Claims 2.0

- Source: HKUST Xunfei
- Introduction: Simple triage requires certain data and experience to support it. This competition provided part of the real consultation data of Haodofu Online, which was strictly desensitized and provided to the contestants for single-category tasks. Specifically: by processing the written appeal, one of the 20 common treatment directions and one of the 61 disease directions are given.
- [Official address](http://challenge.xfyun.cn/topic/info?type=disease-claims-2022&ch=ds22-dw-sq03)

#### 2.2 Chinese: Evaluation tasks of the 8th China Health Information Processing Conference (CHIP2022)

[Official address](http://cips-chip.org.cn/)

1. Medical\_NLP
   1. 一. Evaluation/Competition
      1. 1. Ongoing Contests:
         1. 1.1 Chinese: Imaging NLP ——Medical Imaging Diagnostic Report Generation
         2. 1.2 English: BioNLP Workshop 2023 Shared tasks
         3. 1.3 English: MedVidQA 2023
         4. 1.4 Chinese (long-term effective): Medical information processing challenge list CBLUE dataset
      2. 2. Ended assessments/competitions (starting in 2021):
         1. 2.1 Chinese: Simple Triage Challenge for Non-Standardized Disease Claims 2.0
         2. 2.2 Chinese: Evaluation tasks of the 8th China Health Information Processing Conference (CHIP2022)
         3. 2.3 Chinese: HKUST Xunfei-Medical Entity and Relationship Recognition Challenge
         4. 2.4 Chinese: The First Intelligent Dialogue Diagnosis and Treatment Evaluation Competition (CCL 2021)
         5. 2.5 English: MEDIQA-2021
         6. 2.6 英文： ICLR-2021-医疗对话生成与自动诊断国际竞赛
   2. 二. data set
      1. 1. Chinese dataset
         1. 1.1 Chinese doctor-patient Q\&A dialogue data (1.1M)
         2. 1.2 Chinese Medical Dialogue Dataset (792K)
         3. 1.3 CPubMed-KG (4.4M triplets)
         4. 1.4 CBLUE evaluation
         5. 1.5 Chinese Medical Knowledge Graph CMeKG (1M triples)
         6. 1.6 cMedQA2 (108K)
         7. 1.7 xywy-KG (294K triplets)
         8. 1.8 39Health-KG (210K triplets)
         9. 1.9 Evaluation of CHIP over the years (official evaluation)
         10. 1.10 Ruijin Hospital Diabetes Dataset (Diabetes)
         11. 1.11 Tianchi COVID-19 Question Matching Competition (COVID-19)
      2. 2. Knowledge and information sources commonly used by Chinese clinicians
         1. 2.1 pubMed
         2. 2.2 Up-to-date
         3. 2.3clinical guidelines
         4. 2.4 medication assistant
         5. 2.5 Lilac Garden
         6. 2.6 Doctor Lilac
      3. 3. English dataset
         1. 3.1 PubMedQA
         2. 3.2 COMETA
         3. 3.3 MedMentions
   3. 三. Open source pre-trained model
      1. 1. Existing Medical NLP large model
         1. 1.1 BioMedLM (2.7B)
         2. 1.2 BioGPT  (1.5B)
         3. 1.3 Medical-chatgpt
         4. 1.4 BioBERT
         5. 1.5 PubMedBERT
      2. 2.Other large models in Chinese that can be fine-tuned in the medical field
         1. 2.1 Awesome List
         2. 2.2 Model parameter scale 0B-5B:
            1. 2.2.1 Mencius (1B)
            2. 2.2.2 GLM-2b
            3. 2.2.3 CPM-1(2.6B)
            4. 2.2.4 gpt2-ml(1.5B)
            5. 2.2.5 Pangu-Alpha(2.6B)
            6. 2.2.6 Chinese-Transformer-XL(2.9B)
         3. 2.3 Model parameter scale 5B-10B:
            1. 2.3.1 **ChatGLM-6B**
            2. 2.3.2 Stanford Alpaca(7B)
            3. 2.3.2 GLM-10B
            4. 2.3.3 ERNIE3.0(10B)
         4. 2.4 Model parameter scale 10B-100B:
            1. 2.4.1 Pangu-Alpha(13B)
            2. 2.4.2 CPM-2(11B)
         5. 2.5 Model parameter size 100B--:
            1. 2.5.1 **GLM-130B** SHOW respects to those guys who firmly overcome difficulties and finally realize the project and selflessly share \[detailed experience\](https ://keg.cs.tsinghua.edu.cn/glm-130b/zh/posts/glm-130b)  !
            2. 2.5.2 CPM-2-MoE(198B)
            3. 2.5.3 Pangu-Alpha(200B)
            4. 2.5.4 Source 1.0(245B)
   4. 四. Related Papers
      1. 1. Papers that may be helpful in the post-ChatGPT era (continuously updated)
         1. 1.1 **ChatGPT Performance on USMLE**: The Potential of Using Large Language Models for AI-Assisted Medical Education
         2. 1.2 Conducting a (Turing) Test on **ChatGPT's Medical Advice**
         3. 1.3 **Toolformer**: The language model can learn to use tools by itself
         4. 1.4 Check your facts and try again: **Leverage external knowledge and automatic feedback to improve large language models**
      2. 2 Review articles
         1. 1. Pretrained Language Models in Biomedical Domains: A Systematic Survey
         2. 2. A Guide to Deep Learning in Healthcare
      3. 3. Summary and archive of papers in the warehouse before 2021
         1. 3.1 Electronic medical records related articles
         2. 3.2 Medical relationship extraction
         3. 3.4 Auxiliary diagnosis
         4. 3.5 ACL2020 list of related papers in the medical field
         5. 3.6 Medical entity Linking (standardization)
         6. 3.7 List of AAAI2020 medical NLP related papers
         7. 3.8 EMNLP2020 Medical NLP related papers list
   5. 5. Open source toolkit
      1. 1. Word segmentation tool: PKUSEG
   6. 6. Industrial-grade product solutions
      1. 1. Spiritual Doctor Wisdom
      2. 2. Left-handed doctor
      3. 3. Yidu Cloud Academy - Medical Natural Language Processing
      4. 4. Baidu-Medical Text Structured
      5. 5. Alibaba Cloud - Medical Natural Language Processing
   7. 7. Blog sharing
      1. 1. Blogs that may be helpful in the post-ChatGPT era (continuously updated)
         1. 1.1 Alpaca: A Powerful Open Source Instruction Following Model
      2. 2. Warehouse blog sharing archive before 2021
         1. 2.1 Experiences and lessons of building natural language processing systems in the medical field
         2. 2.2 Introduction to Medical Public Database and Data Mining Technology in the Big Data Era
         3. 2.3 See the development of NLP in the medical field from ACL 2021, with resource download attached
   8. 8. Friendship Links
      1. 1. awesome\_Chinese\_medical\_NLP
      2. 2. Chinese NLP Dataset Search
      3. 3. medical-data (massive medical-related data)
      4. 4. Tianchi data set (which contains multiple medical NLP data sets)

#### 2.3 Chinese: HKUST Xunfei-Medical Entity and Relationship Recognition Challenge

- Source: HKUST Xunfei

- Introduction: Named entity recognition and entity relationship extraction for medical technical reports (a semi-structured data, different doctors have inconsistent expression styles, and the text form lacks a unified specification).
- [Evaluation official website](https://challenge.xfyun.cn/topic/info?type=medical-entity&ch=dc-web-35)

#### 2.4 Chinese: The First Intelligent Dialogue Diagnosis and Treatment Evaluation Competition (CCL 2021)

- Source: China Conference on Computational Linguistics 2021 (CCL 2021): Teacher Yao Lu from Zhongshan Hospital provided professional guidance and suggestions on the design of the data annotation framework. Chen Wei, Zhong Zongye, Wang Jingzhiyuan, Ge Yu, Wang Yali, Wen Huimei, Si Ruoyan and other students participated in the data labeling process.

- Introduction: Release 5 technical evaluation tasks, including the task of "Intelligent Medical Dialogue Diagnosis and Treatment". This intelligent dialogue diagnosis and treatment evaluation set up four tasks in three tracks: doctor-patient dialogue understanding (named entity recognition, symptom recognition), automatic generation of medical reports, and intelligent medical diagnosis.
- [Task URL](http://www.fudan-disc.com/sharedtask/imcs21/index.html)

#### 2.5 English: MEDIQA-2021

- Source: NAACL-BioNLP 2021 workshop.
- Introduction: Address three summarization tasks in the medical domain: consumer health question summarization, multi-answer summarization, and radiology report summarization, and explore the use of different evaluation metrics for summarization.
- [MEDIQA Evaluation Address](https://sites.google.com/view/mediqa2021)

#### 2.6 英文： ICLR-2021-医疗对话生成与自动诊断国际竞赛

- Source: ICLR 2021 workshop


- Introduction: The theme of this competition is the development of automatic medical diagnosis dialogue system. Currently, there are two tracks: medical dialogue generation track and automatic medical diagnosis track.
- [Competition official address](https://mlpcp21.github.io/pages/challenge)





## 二. data set

> This section contains large or characteristic Chinese and English datasets, basically sorted by dataset size (number of questions) in descending order.

### 1. Chinese dataset

> This section contains large or characteristic Chinese and English datasets, basically sorted by dataset size (number of questions) in descending order.

#### 1.1 Chinese doctor-patient Q&A dialogue data (1.1M)

- Introduction: Chinese doctor-patient dialogue data from haodf.com.

- [Project Address](https://github.com/UCSD-AI4H/Medical-Dialogue-System)

- Dupan download address: https://pan.baidu.com/s/1ZwzNgvAAMQk4klerTspsoA Extraction code: lbo4



#### 1.2 Chinese Medical Dialogue Dataset (792K)

- Introduction: Contains medical question-and-answer data of six departments, github open source data, source unknown.

- [Project Address](https://github.com/Toyhom/Chinese-medical-dialogue-data)



#### 1.3 CPubMed-KG (4.4M triplets)

- Source: Medical Health and Bioinformatics Professional Committee of Chinese Information Society of China, Medical Knowledge Graph Professional Group of Language and Knowledge Computing Committee, Artificial Intelligence Committee of Shenzhen Computer Society, Harbin Institute of Technology (Shenzhen) and domestic high-level medical institutions ,Chinese Medical Association.
- Introduction: The large-scale Chinese open medical knowledge map and open medical knowledge online collaborative construction platform constructed by the high-quality full-text periodical data of the Chinese Medical Association aims to break the bottleneck of Chinese medical knowledge and support wisdom through a completely open and collaborative mechanism Development of medical technology.
- [Project Address](https://cpubmed.openi.org.cn/graph/wiki)

#### 1.4 CBLUE evaluation

- CBLUE 1.0:
  - Source: The Medical Health and Bioinformatics Professional Committee of the Chinese Information Society of China was initiated under the concept of legal openness and sharing, undertaken by Alibaba Cloud Tianchi Platform, and co-sponsored by Yidu Cloud (Beijing) Technology Co., Ltd., Ping An Medical Technology, Peking University, Co-organized by Zhengzhou University, Pengcheng Laboratory, Harbin Institute of Technology (Shenzhen), Tongji University, Quark, Alibaba Dharma Institute and other units that carry out smart medical research, it aims to promote the development of Chinese medical NLP technology and communities. **It is composed of the previous academic evaluation competitions of the CHIP conference and the data sets of Ali Quark's medical search business. **
  - Introduction: Covers 4 common medical information processing tasks of medical text information extraction (entity recognition, relationship extraction), medical term normalization, medical text classification, and medical sentence semantic correlation determination, including 8 subtasks in total.
- CBLUE 2.0:
   - Source: Compared with 1.0, Fudan University, Tencent Tianyan Lab and Sun Yat-sen University were added.
   - Introduction: Covers 5 common medical information processing tasks, medical text information extraction (entity recognition, relationship extraction), medical term normalization, medical text classification, medical sentence semantic correlation determination, medical dialogue understanding and generation. Contains 15 subtasks.
     - For detailed comparison, please refer to https://zhuanlan.zhihu.com/p/469465499

- [CBLUE evaluation official address](https://tianchi.aliyun.com/dataset/dataDetail?dataId=95414)
- [Paper Address](https://arxiv.org/abs/2106.08087)
- [Github project address](https://github.com/CBLUEbenchmark/CBLUE)



#### 1.5 Chinese Medical Knowledge Graph CMeKG (1M triples)

- Introduction: CMeKG (Chinese Medical Knowledge Graph) is a Chinese medical knowledge graph developed by human-computer integration based on large-scale medical text data using natural language processing and text mining technology. The construction of CMeKG refers to authoritative international medical standards such as ICD, ATC, SNOMED, and MeSH, as well as medical text information such as large-scale, multi-source and heterogeneous clinical guidelines, industry standards, diagnosis and treatment norms, and medical encyclopedias. CMeKG 1.0 includes: 6310 kinds of diseases, 19853 kinds of medicines (western medicines, Chinese patent medicines, Chinese herbal medicines), 1237 kinds of structured knowledge descriptions of diagnosis and treatment techniques and equipment, covering clinical symptoms, diseased parts, drug treatment, surgical treatment, differential diagnosis, More than 30 common relationship types such as imaging examination, high-risk factors, transmission routes, high-risk groups, medical departments, etc., as well as drug ingredients, indications, usage and dosage, validity period, contraindications, etc., conceptual relationship examples and attribute triples described by CMeKG Reached more than 1 million.

- [Project Address](http://cmekg.pcl.ac.cn/)



####  1.6 cMedQA2 (108K)

- Introduction: A question-and-answer dataset of Chinese medicine, with more than 100,000 records.

  - questions.csv: All questions and their contents. answers.csv : Answers to all questions.

  - train_candidates.txt, dev_candidates.txt, test_candidates.txt: Split the above two files.

- [dataset address](https://www.kesci.com/home/dataset/5d313070cf76a60036e4b023/document)

- [Dataset github address](https://github.com/zhangsheng93/cMedQA2)



#### 1.7 xywy-KG (294K triplets)

- Source: Xunyiwenyao.com
- Introduction: 44.1K entities 294.1K triples
- [Project Address](https://github.com/baiyang2464/chatbot-base-on-Knowledge-Graph)



#### 1.8 39Health-KG (210K triplets)

- Source: 39 Health Net.
- Introduction: Including 15 items of information, including 7 types of entities, about 37,000 entities, and 210,000 entity relationships.
- [Project Address](https://github.com/zhihao-chen/QASystemOnMedicalGraph)

#### 1.9 Evaluation of CHIP over the years (official evaluation)

1. CHIP2022:  http://cips-chip.org.cn/2022/callforeval
2. CHIP2021: http://www.cips-chip.org.cn/2021/
3. CHIP2020: http://cips-chip.org.cn/2020/



#### 1.10 Ruijin Hospital Diabetes Dataset (Diabetes)

- Introduction: The data set comes from the Tianchi Competition. This data set aims to do diabetes literature mining and build a diabetes knowledge map through diabetes-related textbooks and research papers. Contestants need to design high-accuracy and efficient algorithms to challenge this scientific problem. The topic of the first season is "Entity Annotation Construction Based on Diabetes Clinical Guidelines and Research Papers", and the topic of the second season is "Construction of Entity Relationships Based on Diabetes Clinical Guidelines and Research Papers".
  - The official data only includes the training set, and the actual test set used for the final ranking is not given.

- [dataset address](https://tianchi.aliyun.com/competition/entrance/231687/information)

-Dupan download address: https://pan.baidu.com/s/1CWKblBNBqR-vs2h0xiXSdQ Extraction code: 0c54

#### 1.11 Tianchi COVID-19 Question Matching Competition (COVID-19)

- Introduction: The data of this competition includes: desensitized medical problem data pairs and labeled data. Medical problems involving "pneumonia", "mycoplasma pneumonia", "bronchitis", "upper respiratory infection", "tuberculosis", "asthma", "pleurisy", "emphysema", "cold", "coughing up blood", etc. 10 disease types.

- [dataset address (requires registration)](https://tianchi.aliyun.com/competition/entrance/231776/information)

- [Online fourth place solution and code](https://github.com/Makaixin/similar-sentence-pairs-in-epidemic)

- [Online first place solution and code](https://github.com/zzy99/epidemic-sentence-pair)





### 2. Knowledge and information sources commonly used by Chinese clinicians

#### 2.1 pubMed

 https://pubmed.ncbi.nlm.nih.gov/ 

#### 2.2 Up-to-date

https://www.wolterskluwer.com/en/expert-insights/health

#### 2.3clinical guidelines

 https://guide.medlive.cn/

#### 2.4 medication assistant

 https://drugs.dxy.cn/

#### 2.5 Lilac Garden

 https://www.dxy.cn/

#### 2.6 Doctor Lilac

https://dxy.com/








### 3. English dataset

#### 3.1 PubMedQA

- Introduction: Based on the medical question answering dataset extracted from Pubmed. PubMedQA has 1k expert-annotated, 61.2k unlabeled and 211.3k artificially generated QA instances.
- [Paper Address](https://arxiv.org/abs/1909.06146)

#### 3.2 COMETA

- Presentation: Medical entity link data in social media. Published at EMNLP2020.


- Data acquisition method: https://www.siphs.org/ https://github.com/cambridgeltl/cometa


- [Paper Address](https://arxiv.org/pdf/2010.03295.pdf)

#### 3.3 MedMentions

- Introduction: A Biomedical Entity Linking Dataset Based on Pubmed Abstracts. Published at AKBC 2019.


- [dataset address](https://github.com/chanzuckerberg/MedMentions)

- [Paper Address](https://arxiv.org/abs/1902.09476)







## 三. Open source pre-trained model

This section introduces large-scale language models in the field of medical NLP, and provides practitioners with references to initialization parameters and training methods. Sort basically by model size in descending order.

### 1. Existing Medical NLP large model

#### 1.1 BioMedLM (2.7B)

- Source: Stanford Chris Manning and Percy Liang Group
- Introduction: Introduces a new 2.7B parameter language model trained on biomedical literature, providing improved state-of-the-art for medical question answering. (Note: At the request of the NIH, which holds the "PubMed" trademark, the model has been renamed BioMedLM. Future updates will refer to BioMedLM)

- [Project Address](https://github.com/stanford-crfm/BioMedLM)

- [Interpretation of the article](https://crfm.stanford.edu/2022/12/15/pubmedgpt.html)

- [Model](https://huggingface.co/stanford-crfm/pubmedgpt/tree/main)



#### 1.2 BioGPT  (1.5B)

- Source: Microsoft Tie-Yan Liu Group
- Introduction: BioGPT, a domain-specific generative Transformer language model pre-trained on large-scale biomedical literature, achieved a record-breaking 78.2% accuracy on PubMedQA

- [Project Address](https://github.com/microsoft/BioGPT)

#### 1.3 Medical-chatgpt 

- Source: Google Research and Deep AI
- Presentation: The implementation of ChatGPT tailored to the primary medical health domain, however, rewarding the ability to collect patient histories and present sound differential diagnoses in a thorough and efficient manner
- [Project Address](https://github.com/lucidrains/medical-chatgpt)
- [Paper Address](https://arxiv.org/pdf/2212.13138.pdf)

#### 1.4 BioBERT

- Source: Department of Computer Science and Engineering, Korea University, Interdisciplinary Graduate Program in Bioinformatics, Korea University,
- Introduction: BioBERT (Bidirectional Encoder Representations with Transformers for Biomedical Text Mining) is a domain-specific language representation model pretrained on large-scale biomedical corpora.
- [Project Address](https://github.com/dmis-lab/biobert)
- [Paper Address](https://arxiv.org/ftp/arxiv/papers/1901/1901.08746.pdf)

#### 1.5 PubMedBERT

- Source: National Center for Biotechnology Information National Library of Medicine, National Institutes of Health Bethesda, MD, USA
- Introduction: PubMedBERT is pretrained from scratch using abstracts from PubMed.
- [Paper Address](https://arxiv.org/pdf/2007.15779.pdf)
- [Model Address](https://huggingface.co/microsoft/BiomedNLP-PubMedBERT-base-uncased-abstract)

### 2.Other large models in Chinese that can be fine-tuned in the medical field

#### 2.1 [Awesome List](https://github.com/lonePatient/awesome-pretrained-chinese-nlp-models#GPT) 

#### 2.2 Model parameter scale 0B-5B:

##### 2.2.1 [Mencius (1B)](https://github.com/Langboat/Mengzi)

##### 2.2.2 [GLM-2b](https://github.com/THUDM/glm)

##### 2.2.3 [CPM-1(2.6B)](https://github.com/TsinghuaAI/CPM-1-Generate)

##### 2.2.4 [gpt2-ml(1.5B)](https://github.com/imcaspar/gpt2-ml)

##### 2.2.5 [Pangu-Alpha(2.6B)](https://openi.pcl.ac.cn/PCL-Platform.Intelligence/PanGu-Alpha)

##### 2.2.6 [Chinese-Transformer-XL(2.9B)](https://github.com/THUDM/Chinese-Transformer-XL)

#### 2.3 Model parameter scale 5B-10B:

##### 2.3.1 [**ChatGLM-6B**](https://github.com/THUDM/ChatGLM-6B)

##### 2.3.2 [Stanford Alpaca(7B)](https://github.com/tatsu-lab/stanford_alpaca)

##### 2.3.2 [GLM-10B](https://github.com/THUDM/glm)

##### 2.3.3 [ERNIE3.0(10B)](https://github.com/PaddlePaddle/ERNIE)

#### 2.4 Model parameter scale 10B-100B:

##### 2.4.1 [Pangu-Alpha(13B)](https://openi.pcl.ac.cn/PCL-Platform.Intelligence/PanGu-Alpha)

##### 2.4.2 [CPM-2(11B)](https://github.com/TsinghuaAI/CPM-2-Finetune)

#### 2.5 Model parameter size 100B--:

##### 2.5.1 [**GLM-130B**](https://github.com/THUDM/GLM-130B) SHOW respects to those guys who firmly overcome difficulties and finally realize the project and selflessly share [detailed experience](https ://keg.cs.tsinghua.edu.cn/glm-130b/zh/posts/glm-130b)  !

##### 2.5.2 [CPM-2-MoE(198B)](https://openi.pcl.ac.cn/BAAI/WuDao-Model/src/branch/master/CPM)

##### 2.5.3 [Pangu-Alpha(200B)](https://openi.pcl.ac.cn/PCL-Platform.Intelligence/PanGu-Alpha)

##### 2.5.4 [Source 1.0(245B)](https://github.com/Shawn-Inspur/Yuan-1.0)





## 四. Related Papers

This part focuses more on collecting related papers in the post-ChatGPT era, roughly in order of publication time.

### 1. Papers that may be helpful in the post-ChatGPT era (continuously updated)

#### 1.1 **ChatGPT Performance on USMLE**: The Potential of Using Large Language Models for AI-Assisted Medical Education

- Paper address: https://journals.plos.org/digitalhealth/article?id=10.1371/journal.pdig.0000198
- Abstract Translation: We evaluate the performance of a large language model called ChatGPT on the United States Medical Licensing Examination (USMLE), which consists of three exams: Step1, Step2CK, and Step3. ChatGPT performed at or near the passing threshold on all three exams without requiring any specialized training or reinforcement. Furthermore, ChatGPT shows high consistency and insight in its interpretation. These results suggest that large language models may aid medical education and possibly clinical decision-making.

#### 1.2 Conducting a (Turing) Test on **ChatGPT's Medical Advice**

- Paper address: https://arxiv.org/abs/2301.10035
- Abstract Translation: Objective: To assess the feasibility of using ChatGPT or similar AI-based chatbots for patient-provider communication. PARTICIPANTS: US representative sample of 430 study participants aged 18 years and older. 53.2% of the respondents were female; their average age was 47.1 years. Exposure: Ten representative nonadministrative patient-provider interactions were extracted from EHRs. The patient's questions were placed in ChatGPT, and the chatbot was asked to answer using roughly the same word count as the human provider's responses. In surveys, each patient question is followed by a provider or ChatGPT-generated response. Participants were told that five responses were generated by the provider and five by the chatbot. Participants are required and financially incentivized to correctly identify response sources. Participants were also asked about their trust in the chatbot's function in patient-provider communication, using a Likert scale 1-5. RESULTS: The responses to the different questions were correctly classified between 49.0% and 85.7%. On average, chatbot responses were correctly identified 65.5% of the time, and supplier responses were correctly identified 65.1% of the time. On average, patients reported weak trust responses to the chatbot functionality (mean Likert score: 3.4), with trust decreasing as the health-related complexity of the problem task increased. Conclusions: ChatGPT responses to patient questions were indistinguishable from provider responses. Laymen seem to believe in using chatbots to answer lower-risk health questions.

#### 1.3 **Toolformer**: The language model can learn to use tools by itself

- Paper address: https://arxiv.org/abs/2302.04761
- Abstract Translation: Language Models (LMs) have shown a remarkable ability to solve new tasks with only a few examples or text instructions, especially at scale. Paradoxically, they also struggled with basic functions, such as arithmetic or fact-finding, where simpler, smaller models excel. In this paper, we show that LMs can teach themselves to use external tools through a simple API and achieve the best of both worlds. We introduce the Toolformer, a model trained to decide which APIs to call, when to call them, which parameters to pass, and how to best incorporate the results into future token predictions. This is done in a self-supervised manner, requiring only a small number of demos for each API. We have integrated a range of tools including a calculator, a question answering system, two different search engines, a translation system and a calendar. Toolformer achieves significantly improved zero-shot performance across a variety of downstream tasks, often competing with larger models without sacrificing its core language modeling capabilities.

#### 1.4 Check your facts and try again: **Leverage external knowledge and automatic feedback to improve large language models**

- Paper address: https://arxiv.org/abs/2302.12813
- Summary Translation: Large language models (LLMs), such as ChatGPT, are capable of generating fluent human-like responses for many downstream tasks, such as task-oriented dialogue and question answering. However, applying LLMs to real-world mission-critical applications remains challenging mainly due to their tendency to hallucinate and the inability to use external knowledge. This paper presents an LLM-Augmenter system that augments black-box LLMs with a set of plug-and-play modules. Our system enables the LLM to generate responses based on external knowledge, e.g. stored in a task-specific database. It also iteratively modifies LLM cues to improve model responses using feedback generated by utility functions, such as the ground-truth scores of LLM-generated responses. The effectiveness of LLM-Augmenter is empirically verified in two types of scenarios, task-oriented dialogue and open-domain question answering. LLM-Augmenter significantly reduces ChatGPT hallucinations without sacrificing the fluency and informativeness of its responses. We make the source code and models publicly available.



### 2 Review articles

#### 1. Pretrained Language Models in Biomedical Domains: A Systematic Survey

- Paper address: https://arxiv.org/abs/2110.05006
- Pretrained Language Models (PLMs) have become the de-facto paradigm for most Natural Language Processing (NLP) tasks. This also benefits the biomedical field: Researchers from the informatics, medical, and computer science (CS) communities have proposed various PLMs trained on biomedical datasets, e.g., biomedical text for various biomedical tasks , electronic health records, protein and DNA sequences. However, the interdisciplinary nature of biomedical PLM hinders its dissemination among communities; some existing works are isolated from each other without comprehensive comparison and discussion. It expects a survey not only to systematically review recent advances in biomedical PLM and its applications, but also to standardize terminology and benchmarking. In this paper, we summarize the recent progress of pre-trained language models in the field of biomedicine and their applications to downstream tasks in biomedicine. In particular, we discuss motivations and propose a taxonomy of existing biomedical PLMs. Their application to biomedical downstream tasks is discussed in detail. Finally, we elaborate on various limitations and future trends, hoping to shed light on future research in the research community.

#### 2. A Guide to Deep Learning in Healthcare

- [Paper address](https://www.nature.com/articles/s41591-018-0316-z) Review published by nature medicine
- Abstract translation: Here we introduce deep learning techniques for healthcare, focusing on deep learning in computer vision, natural language processing, reinforcement learning, and general approaches. We describe how these computational technologies impact several key areas of medicine and explore how to build end-to-end systems. Our discussion of computer vision focuses on medical imaging, and we describe applications of natural language processing to areas such as electronic health record data. Likewise, reinforcement learning is discussed in the context of robot-assisted surgery, and generalized deep learning methods for genomics are reviewed.









### 3. Summary and archive of papers in the warehouse before 2021

#### 3.1 Electronic medical records related articles

**Transfer Learning from Medical Literature for Section Prediction in Electronic Health Records**

[Paper Address](https://www.aclweb.org/anthology/D19-1492/)

Paper Summary: Published in EMNLP2019. EHR-related migration learning based on a small amount of in-domain data and a large amount of out-of-domain data.

Abstract: sections such as Assessment and Plan, Social History, and Medications. These sections help physicians find information easily and can be used by an information retrieval system to return specific information sought by a user. However, it is common that the exact format of sections in a particular EHR does not adhere to known patterns. There-fore, being able to predict sections and headers in EHRs automatically is beneficial to physicians. Prior approaches in EHR section prediction have only used text data from EHRs and have required significant manual annotation. We propose using sections from medical literature (e.g., textbooks, journals, web content) that contain content similar to that found in EHR sections. Our approach uses data from a different kind of source where la-bels are provided without the need of a time- consuming annotation effort. We use this data to train two models: an RNN and a BERT-based model. We apply the learned models along with source data via transfer learning to predict sections in EHRs. Our results show that medical literature can provide helpful su-pervision signal for this classification task.

**MUFASA: Multimodal Fusion Architecture Search for Electronic Health Records**

[Paper address](http://arxiv-download.xixiaoyao.cn/pdf/2102.02340.pdf)

Paper Summary: Published in AAAI2021.

Abstract of the paper: One important challenge of applying deep learning to electronic health records (EHR) is the complexity of their multimodal structure. EHR usually contains a mixture of structured (codes) and unstructured (free-text) data with sparse and irregular longitudinal features – all of which doctors utilize when making decisions. In the deep learning regime, determining how different modality representations should be fused together is a difficult problem, which is often addressed by handcrafted modeling and intuition. In this work, we extend state-of-the -art neural architecture search (NAS) methods and propose MUltimodal Fusion Architecture SeArch (MUFASA) to simultaneously search across multimodal fusion strategies and modality-specific architectures for the first time. with comparable computation costs. In addition, MUFASA produces architectures that outperform Transformer and Evolv ed Transformer. Compared with these baselines on CCS diagnosis code prediction, our discovered models improve top-5 recall from 0.88 to 0.91 and demonstrate the ability to generalize to other EHR tasks. Studying our top architecture in depth, we provide that UmFASA' are derived from its ability to both customize modeling for each data modality and find effective fusion strategies.




#### 3.2 Medical relationship extraction

**Leveraging Dependency Forest for Neural Medical Relation Extraction**

[Paper Address](https://www.aclweb.org/anthology/D19-1020/)

Summary of the paper: Published in EMNLP 2019. Based on the dependency forest method, the recall rate of the dependency relationship in the medical sentence is improved, and a part of the noise is introduced at the same time. The feature extraction is based on the graph cycle network, which provides the use of the dependency relationship in the extraction of the medical relationship. At the same time A way to reduce error transmission.

Abstract: Medical relation extraction discovers relations between entity mentions in text, such as research articles. For this task, dependency syntax has been recognized as a crucial source of features. Yet in the medical domain, 1-best parse trees suffer from relatively low accuracies, diminishing their usefulness. We investigate a method to alleviate this problem by utilizing dependency forests. Forests contain more than one possible decisions and therefore have higher recall but more noise compared with 1-best outputs. forests, automatically distinguishing the useful syntactic information from parsing noise. Results on two benchmarks show that our method outperforms the standard tree-based methods, giving the state-of-the-art results in the literature.

####3.3 医学知识图谱

**Learning a Health Knowledge Graph from Electronic Medical Records**

[论文地址](https://www.nature.com/articles/s41598-017-05778-z)

论文概要：发表于nature scientificreports（2017）. 基于27万余份电子病历构建的疾病-症状知识图谱。

论文摘要：Demand for clinical decision support systems in medicine and self-diagnostic symptom checkers has substantially increased in recent years. Existing platforms rely on knowledge bases manually compiled through a labor-intensive process or automatically derived using simple pairwise statistics. This study explored an automated process to learn high quality knowledge bases linking diseases and symptoms directly from electronic medical records. Medical concepts were extracted from 273,174 de-identified patient records and maximum likelihood estimation of three probabilistic models was used to automatically construct knowledge graphs: logistic regression, naive Bayes classifier and a Bayesian network using noisy OR gates. A graph of disease-symptom relationships was elicited from the learned parameters and the constructed knowledge graphs were evaluated and validated, with permission, against Google’s manually-constructed knowledge graph and against expert physician opinions. Our study shows that direct and automated construction of high quality health knowledge graphs from medical records using rudimentary concept extraction is feasible. The noisy OR model produces a high quality knowledge graph reaching precision of 0.85 for a recall of 0.6 in the clinical evaluation. Noisy OR significantly outperforms all tested models across evaluation frameworks (p < 0.01).

#### 3.4 Auxiliary diagnosis

**Evaluation and accurate diagnoses of pediatric diseases using artificial intelligence**

[Paper Address](https://www.nature.com/articles/s41591-018-0335-9)

Summary of the paper: This paper was jointly completed by Guangzhou Women and Children's Medical Center and Yitu Medical and other enterprises and scientific research institutions. The natural language processing (NLP) technology based on machine learning achieves a powerful diagnostic ability that is not inferior to that of human doctors, and has multi-scenario Application Ability. According to reports, this is the world's first research achievement on clinical intelligent diagnosis based on electronic health records (EHR) using natural language processing (NLP) technology published in a top medical journal.

Abstract: Artificial intelligence (AI)-based methods have emerged as powerful tools to transform medical care. Although machine learning classifiers (MLCs) have already demonstrated strong performance in image-based diagnoses, analysis of diverse and massive electronic health) record (EHR data remains challenging. Here, we show that MLCs can query EHRs in a manner similar to the hypothetico-deductive reasoning used by physicians and unearth associations that previous statistical methods have not found. Our model applies an automated natural using language processing system l pediatricians in diagnosing common childhood diseases. Our study provi des a proof of concept for implementing an AI-based system as a means to aid physicians in tackling large amounts of data, augmenting diagnostic evaluations, and to provide clinical decision support in cases of diagnostic uncertainty or complexity. Although this impact may be most evident In areas where healthcare providers are in relative shortage, the benefits of such an AI system are likely to be universal.

#### 3.5 ACL2020 list of related papers in the medical field

**A Generate-and-Rank Framework with Semantic Type Regularization for Biomedical Concept Normalization**

[Paper Address](https://www.aclweb.org/anthology/2020.acl-main.748/)

**Biomedical Entity Representations with Synonym Marginalization**

[Paper Address](https://www.aclweb.org/anthology/2020.acl-main.335/)

**Document Translation vs. Query Translation for Cross-Lingual Information Retrieval in the Medical Domain**

[Paper Address](https://www.aclweb.org/anthology/2020.acl-main.613/)

**MIE: A Medical Information Extractor towards Medical Dialogues**

[Paper Address](https://www.aclweb.org/anthology/2020.acl-main.576/)

**Rationalizing Medical Relation Prediction from Corpus-level Statistics**

[Paper Address](https://www.aclweb.org/anthology/2020.acl-main.719/)

#### 3.6 Medical entity Linking (standardization)

**Medical Entity Linking using Triplet Network**

[Paper address](https://www.aclweb.org/anthology/W19-1912/)

Summary of the paper: Published in ACL2019, the content of the paper is the research on linking of disease entities. Using triplet data, (mention, positive example, negative example), the goal is to make distance(mention, negative example)-distance(mention, positive example)>alpha (a classic scheme for face recognition), and the specific loss function can be found in the paper. The paper mainly includes two parts: 1) Candidate data set generation, for a given mention, calculate cosine similarity and Jaccard overlap score with standard disease set data (standard words and synonyms), and take topK as candidate samples. 2) The network structure is based on Triplet Network. See the paper for details.

**A Generate-and-Rank Framework with Semantic Type Regularization for Biomedical Concept Normalization**

[Paper Address](https://www.aclweb.org/anthology/2020.acl-main.748.pdf)

Abstract of the paper: Published in ACL2020. A learning method based on list-wise sorting. It is mainly divided into two parts: subsequent data set generation and BERT-based list-wise sorting. New ideas: 1) During the sample generation process, the standard words are expanded based on synonyms. 2) Semantic type regularization is introduced in the loss. See the paper for details.

**Deep Neural Models for Medical Concept Normalization in User-Generated Texts**

[Paper Address](https://www.aclweb.org/anthology/P19-2055.pdf)



#### 3.7 List of AAAI2020 medical NLP related papers

**On the Generation of Medical Question-Answer Pairs**

[Paper Address](https://arxiv.org/pdf/1811.00681.pdf)

**LATTE: Latent Type Modeling for Biomedical Entity Linking**

[Paper Address](https://arxiv.org/pdf/1911.09787.pdf)

**Learning Conceptual-Contextual Embeddings for Medical Text**

[Paper Address](https://arxiv.org/pdf/1908.06203.pdf)

**Understanding Medical Conversations with Scattered Keyword Attention and Weak Supervision from Responses**

[Paper address](http://ir.hit.edu.cn/~car/papers/AAAI2020-Shi-medconv.pdf)

**Simultaneously Linking Entities and Extracting Relations from Biomedical Text without Mention-level Supervision**

[Paper Address](https://arxiv.org/pdf/1912.01070.pdf)

**Can Embeddings Adequately Represent Medical Terminology? New Large-Scale Medical Term Similarity Datasets Have the Answer!**

[Paper Address](https://arxiv.org/pdf/2003.11082.pdf)

#### 3.8 EMNLP2020 Medical NLP related papers list

**Towards Medical Machine Reading Comprehension with Structural Knowledge and Plain Text**

[Paper Address](https://www.aclweb.org/anthology/2020.emnlp-main.111.pdf)

**MedDialog: Large-scale Medical Dialogue Datasets**

[Paper Address](https://www.aclweb.org/anthology/2020.emnlp-main.743.pdf)

**COMETA: A Corpus for Medical Entity Linking in the Social Media**

[Paper Address](https://www.aclweb.org/anthology/2020.emnlp-main.253.pdf)

**Biomedical Event Extraction as Sequence Labeling**

[Paper Address](https://www.aclweb.org/anthology/2020.emnlp-main.431.pdf)

**FedED: Federated Learning via Ensemble Distillation for Medical Relation Extraction**

[Paper Address](https://www.aclweb.org/anthology/2020.emnlp-main.165.pdf)

[Paper Analysis: FedED: Federated Learning for Medical Relationship Extraction (Based on Fusion Distillation)](https://blog.csdn.net/lrs1353281004/article/details/111877017)

**Infusing Disease Knowledge into BERT for Health Question Answering, Medical Inference and Disease Name Recognition**

[Paper Address](https://arxiv.org/pdf/2010.03746.pdf)

**A Knowledge-driven Generative Model for Multi-implication Chinese Medical Procedure Entity Normalization**

[Paper Address](https://www.aclweb.org/anthology/2020.emnlp-main.116.pdf)

**BioMegatron: Larger Biomedical Domain Language Model**

[Paper Address](https://www.aclweb.org/anthology/2020.emnlp-main.379.pdf)

**Querying Across Genres for Medical Claims in News**

[Paper Address](https://www.aclweb.org/anthology/2020.emnlp-main.139.pdf)





## 5. Open source toolkit

### 1. Word segmentation tool: PKUSEG

- [Project Address](https://github.com/lancopku/pkuseg-python)
- Project description: The multi-field Chinese word segmentation tool launched by Peking University supports the selection of medical fields.





## 6. Industrial-grade product solutions

### 1. [Spiritual Doctor Wisdom](https://01.baidu.com/index.html)

### 2. [Left-handed doctor](https://open.zuoshouyisheng.com/)

### 3. [Yidu Cloud Academy - Medical Natural Language Processing](https://www.yiducloud.com.cn/academy.html)

### 4. [Baidu-Medical Text Structured](https://ai.baidu.com/solution/mtp)

### 5. [Alibaba Cloud - Medical Natural Language Processing](https://help.aliyun.com/document_detail/179395.html)





## 7. Blog sharing

### 1. Blogs that may be helpful in the post-ChatGPT era (continuously updated)

#### 1.1 [Alpaca: A Powerful Open Source Instruction Following Model](https://crfm.stanford.edu/2023/03/13/alpaca.html)



### 2. Warehouse blog sharing archive before 2021

#### 2.1 [Experiences and lessons of building natural language processing systems in the medical field](http://www.oreilly.com.cn/radar/?p=2083)

#### 2.2 [Introduction to Medical Public Database and Data Mining Technology in the Big Data Era](https://mp.weixin.qq.com/s/tA44U4bJUttnROfrzpNYcQ)

#### 2.3 [See the development of NLP in the medical field from ACL 2021, with resource download attached](https://mp.weixin.qq.com/s/RhcHvRWHRnYUg6u9vXoIGA)





## 8. Friendship Links

### 1. [awesome_Chinese_medical_NLP](https://github.com/GanjinZero/awesome_Chinese_medical_NLP)

### 2. [Chinese NLP Dataset Search](https://www.cluebenchmarks.com/dataSet_search.html)

### 3. [medical-data (massive medical-related data)](https://github.com/beamandrew/medical-data)

### 4. [Tianchi data set (which contains multiple medical NLP data sets)](https://tianchi.aliyun.com/dataset)

