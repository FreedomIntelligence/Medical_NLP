# Medical_NLP

Summary of medical NLP evaluations/competitions, datasets, papers and pre-trained models.

[中文版本](https://github.com/FreedomIntelligence/Chinese_medical_NLP) [English_version](https://github.com/FreedomIntelligence/Chinese_medical_NLP/blob/master/English_vision.md)

>Since [Cris Lee](https://github.com/lrs1353281004) left the medical NLP field in 2021, this repo is now maintained by [Xidong Wang](https://github.com/wangxidong06), [Ziyue Lin](https://github.com/RobinLin2002), [Jing Tang](https://github.com/vaew).

[Medical_NLP](#medical_nlp)

* [1. Evaluation](#1-evaluation)
   * [1.1 Chinese Medical Benchmark Evaluation: CMB / CMExam / PromptCBLUE](#11-chinese-medical-benchmark-evaluation-cmb--cmexam--promptcblue)
   * [1.2 English Medical Benchmark Evaluation:](#12-english-medical-benchmark-evaluation)
* [2. Competitions](#2-competitions)
   * [2.1 Ongoing Competitions](#21-ongoing-competitions)
   * [2.2 Completed Competitions](#22-completed-competitions)
* [3. Datasets](#3-datasets)
   * [3.1 Chinese](#31-chinese)
   * [3.2 English](#32-english)
* [4. Open-source Models](#4-open-source-models)
   * [4.1 Medical PLMs](#41-medical-PLMs)
   * [4.2 Medical LLMs](#42-medical-LLMs)
* [5. Relevant Papers](#5-relevant-papers)
   * [5.1 The Post-ChatGPT Era: Helpful Papers](#51-the-post-chatgpt-era-helpful-papers)
   * [5.2 Review Articles](#52-review-articles)
   * [5.3 Task-Specific Articles](#53-task-specific-articles)
   * [5.4 Conference Index](#54-conference-index)
* [6. Open-source Toolkits](#6-open-source-toolkits)
* [7. Industrial Solutions](#7-industrial-solutions)
* [8. Blog Sharing](#8-blog-sharing)
* [9. Friendly Links](#9-friendly-links)


## 1. Evaluation

### 1.1 Chinese Medical Benchmark Evaluation: CMB / CMExam / PromptCBLUE

* CMB

  * GitHub Link：https://github.com/FreedomIntelligence/CMB
    ![](https://img.shields.io/github/stars/FreedomIntelligence/CMB)
  * Source：Various clinical medical examinations; complex clinical case consultations
* CMExam

  * GitHub Link：https://github.com/williamliujl/CMExam
    ![](https://img.shields.io/github/stars/williamliujl/CMExam)
  * Source：Past questions from the Medical Practitioner Qualification Examination
* PromptCBLUE
  * GitHub Link：https://github.com/michael-wzhu/PromptCBLUE
    ![](https://img.shields.io/github/stars/michael-wzhu/PromptCBLUE)
  * Source：CBLUE
* PromptCBLUE
  * GitHub Link：https://github.com/CBLUEbenchmark/CBLUE
    ![](https://img.shields.io/github/stars/CBLUEbenchmark/CBLUE)
  * Source：Academic evaluation competitions from past CHIP conferences and datasets from Alibaba Quark's medical search service

### 1.2 English Medical Benchmark Evaluation:、

* MultiMedBench

  * Desription: A large-scale multimodal generative model



## 2. Competitions

### 2.1 Ongoing Competitions

* None at the moment. Additions are welcome~

### 2.2 Completed Competitions

#### 2.2.1 English competitions

* BioNLP Workshop 2023 Shared Task

  * Link:  https://aclweb.org/aclwiki/BioNLP_Workshop#SHARED_TASKS_2023
  * Source: BioNLP Workshop

* MedVidQA 2023

  * Link:  https://medvidqa.github.io/index.html
  * Source: National Institutes of Health

* MEDIQA-2021

  * Link:  https://sites.google.com/view/mediqa2021
  * Source: NAACL-BioNLP 2021 workshop

* ICLR-2021 International Competition for Medical Dialogue Generation and Automatic Diagnosis

  * Link:  https://mlpcp21.github.io/pages/challenge

  * Source: ICLR 2021 workshop


#### **2.2.1 Chinese competitions**

* NLP for Medical Imaging - Medical Imaging Diagnostic Report Generation

  * Link: https://gaiic.caai.cn/ai2023/
  * Source: NLP for Medical Imaging - Medical Imaging Diagnostic Report Generation
* NLP for Medical Imaging - Medical Imaging Diagnostic Report Generation

  * Link: http://challenge.xfyun.cn/topic/info?type=disease-claims-2022&ch=ds22-dw-sq03
  * Source: iFlytek
* Evaluation Task of the 8th China Health Information Processing Conference (CHIP2022)

  * Link: http://cips-chip.org.cn/
  * Source: CHIP2022
* iFlytek - Medical Entity and Relationship Recognition Challenge

  * Link: http://www.fudan-disc.com/sharedtask/imcs21/index.html
  * Source: iFlytek



## 3. Datasets

### 3.1 Chinese

* Huatuo-26M

  * Link: https://github.com/FreedomIntelligence/Huatuo-26M
    ![](https://img.shields.io/github/stars/FreedomIntelligence/Huatuo-26M)
  * Description: Huatuo-26M is the largest Traditional Chinese Medicine (TCM) Q&A dataset to date.
* Chinese Medical Dialogue Dataset

  * Link: https://github.com/FreedomIntelligence/Huatuo-26M
    ![](https://img.shields.io/github/stars/Toyhom/Chinese-medical-dialogue-data)
  * Description: Medical Q&A data from six departments
* CBLUE

  * Link: https://github.com/CBLUEbenchmark/CBLUE
    ![](https://img.shields.io/github/stars/CBLUEbenchmark/CBLUE)
  * Description: Covers medical text information extraction (entity recognition, relation extraction)
* cMedQA2 (108K)

  * Link: https://github.com/zhangsheng93/cMedQA2
    ![](https://img.shields.io/github/stars/zhangsheng93/cMedQA2)
  * Description: Chinese medical Q&A dataset with over 100,000 entries.
* xywy-KG(294K triples)

  * Link: https://github.com/baiyang2464/chatbot-base-on-Knowledge-Graph
    ![](https://img.shields.io/github/stars/baiyang2464/chatbot-base-on-Knowledge-Graph)
  * Description: 44.1K entities 294.1K triples
* 39Health-KG (210K triples)

  * Link: https://github.com/zhihao-chen/QASystemOnMedicalGraph
    ![](https://img.shields.io/github/stars/zhihao-chen/QASystemOnMedicalGraph)
  * Desription: Includes 15 pieces of information, with 7 types of entities, about 37,000 entities, and 210,000 entity relationships.
* Medical-Dialogue-System
  * Link: https://github.com/UCSD-AI4H/Medical-Dialogue-System
    ![](https://img.shields.io/github/stars/UCSD-AI4H/Medical-Dialogue-System)
  * The MedDialog dataset (Chinese) contains conversations (in Chinese) between doctors and patients. It has 1.1 million dialogues and 4 million utterances. The data is continuously growing and more dialogues will be added.
* Chinese medical dialogue data
  * 地址：https://github.com/Toyhom/Chinese-medical-dialogue-data
    ![](https://img.shields.io/github/stars/Toyhom/Chinese-medical-dialogue-data)
  * The dataset contains a total of 792,099 data from six different departments including Male, Pediatrics, Obstetrics and Gynecology, Internal Medicine, Surgery, and Oncology.
* Yidu-S4K

  * Link: http://openkg.cn/dataset/yidu-s4k
  * Description: Named Entity Recognition, Entity and Attribute Extraction
* Yidu-N7K

  * Link: http://openkg.cn/dataset/yidu-n7k
  * Description: Clinical Language Standardization
* Chinese Medical Q&A Dataset

  * Link: https://github.com/zhangsheng93/cMedQA2
  * Description: Medical Q&A
* Chinese Doctor-Patient Dialogue Data

  * 地址：https://github.com/UCSD-AI4H/Medical-Dialogue-System
  * Description: Medical Q&A
* CPubMed-KG (4.4M triples)

  * Link: https://cpubmed.openi.org.cn/graph/wiki
  * Description: Full-text journal data of high quality from the Chinese Medical Association
* Chinese Medical Knowledge Graph CMeKG (1M triples)

  * Link: http://cmekg.pcl.ac.cn/
  * Description: CMeKG（Chinese Medical Knowledge  Graph）
* CHIP Annual Evaluation (Official Evaluation)

  * Link: http://cips-chip.org.cn/2022/callforeval ;  http://www.cips-chip.org.cn/2021/ ;   http://cips-chip.org.cn/2020/
  * Description: CHIP Annual Evaluation (Official Evaluation)
* Ruijin Hospital Diabetes Dataset (Diabetes)

  * Link: https://tianchi.aliyun.com/competition/entrance/231687/information
  * Description: Diabetes literature mining and knowledge graph construction using diabetes-related textbooks and research papers
* Tianchi Novel Coronavirus Pneumonia Question Matching Competition (Novel Coronavirus)

  * Link: https://tianchi.aliyun.com/competition/entrance/231776/information

  * Description: The competition data includes: anonymized medical problem data pairs and annotated data.


### 3.2 English

- MedMentions

  * Link:  https://github.com/chanzuckerberg/MedMentions
    ![](https://img.shields.io/github/stars/chanzuckerberg/MedMentions)
  * Desription: Biomedical entity linking dataset based on PubMed abstracts
- webMedQA
  - Link:  https://github.com/hejunqing/webMedQA
    ![](https://img.shields.io/github/stars/hejunqing/webMedQA)
  - Description: Medical Q&A
- COMETA

  * Link:  https://www.siphs.org/
  * Description: Medical entity linking data in social media. Published at EMNLP2020
- PubMedQA

  * Link:  https://arxiv.org/abs/1909.06146
  * Description: Medical entity linking data in social media. Published at EMNLP2020
- MediQA
  - Link:  https://sites.google.com/view/mediqa2021
  - Description: Text summarization
- ChatDoctor Dataset-1
  - Link:  https://drive.google.com/file/d/1lyfqIwlLSClhgrCutWuEe_IACNq6XNUt/view?usp=sharing
  - Description: 100k real conversations between patients and doctors from HealthCareMagic.com
- ChatDoctor Dataset-2
  - Link:  https://drive.google.com/file/d/1ZKbqgYqWc7DJHs3N9TQYQVPdDQmZaClA/view?usp=sharing
  - Description:  10k real conversations between patients and doctors from icliniq.com
- Visual Med-Alpaca Data
  - Link:  https://github.com/cambridgeltl/visual-med-alpaca/tree/main/data
  - Description: These data are used for Visual Med-Alpaca traning, being produced based on  [BigBio](https://huggingface.co/bigbio), [ROCO](https://github.com/razorx89/roco-dataset) and [GPT-3.5-Turbo](https://chat.openai.com/chat)





## 4. Open-source Models

### 4.1 Medical PLMs

* BioBERT：
  * Website: https://github.com/naver/biobert-pretrained
    ![](https://img.shields.io/github/stars/naver/biobert-pretrained)
  * Introduction: A language representation model for biomedical domain, especially designed for biomedical text mining tasks such as biomedical named entity recognition, relation extraction, question answering, etc.
* BlueBERT：
  * Website: https://github.com/ncbi-nlp/BLUE_Benchmark
    ![](https://img.shields.io/github/stars/ncbi-nlp/BLUE_Benchmark)
  * Introduction: BLUE benchmark consists of five different biomedicine text-mining tasks with ten corpora.   BLUE benchmark rely on preexisting datasets because they have been widely used by the BioNLP community as shared tasks.  These tasks cover a diverse range of text genres (biomedical literature and clinical notes), dataset sizes, and degrees of difficulty and, more importantly, highlight common biomedicine text-mining challenges.
* BioFLAIR：
  * Website: https://github.com/flairNLP/flair
    ![](https://img.shields.io/github/stars/flairNLP/flair)
  * Introduction: Flair is a powerful NLP library, which allows you to apply our state-of-the-art natural language processing (NLP) models to your text, such as named entity recognition (NER), sentiment analysis, part-of-speech tagging (PoS), special support for [biomedical data](https://github.com/flairNLP/flair/blob/master/resources/docs/HUNFLAIR.md), sense disambiguation and classification, with support for a rapidly growing number of languages. Flair is also a A text embedding library and a PyTorch NLP framework.
* COVID-Twitter-BERT：
  * Website: https://github.com/digitalepidemiologylab/covid-twitter-bert
    ![](https://img.shields.io/github/stars/digitalepidemiologylab/covid-twitter-bert)
  * Introduction: COVID-Twitter-BERT (CT-BERT) is a transformer-based model pretrained on a large corpus of Twitter messages on the topic of COVID-19.  The v2 model is trained on 97M tweets (1.2B training examples).
* bio-lm (Biomedical and Clinical Language Models)
  * Website: https://github.com/facebookresearch/bio-lm
    ![](https://img.shields.io/github/stars/facebookresearch/bio-lm)
  * Introduction: This work evaluates many models used for biomedical and clinical nlp tasks, and train new models that perform much better.
* BioALBERT
  * Website: https://github.com/usmaann/BioALBERT
    ![](https://img.shields.io/github/stars/usmaann/BioALBERT)
  * Introduction: A biomedical language representation model trained on large domain specific (biomedical) corpora for designed for biomedical text mining tasks. 

### 4.2 Medical LLMs

#### 4.2.1 Chinese Medical Large Language Models

* BenTsao：
  * Website: https://github.com/SCIR-HI/Huatuo-Llama-Med-Chinese
    ![](https://img.shields.io/github/stars/SCIR-HI/Huatuo-Llama-Med-Chinese)
  * Introduction: BenTsao is based on LLaMA-7B and has undergone fine-tuning with Chinese medical instructions through instruct-tuning. Researchers built a Chinese medical instruction dataset using a medical knowledge graph and the GPT3.5 API, and used this dataset as the basis for instruct-tuning LLaMA, thereby improving its question-answering capabilities in the medical field.
* BianQue：
  * Website: https://github.com/scutcyr/BianQue
    ![](https://img.shields.io/github/stars/scutcyr/BianQue)
  * Introduction: A large medical conversation model fine-tuned through joint training with instructions and multi-turn inquiry dialogues. It is based on ClueAI/ChatYuan-large-v2 and fine-tuned using a blended dataset of Chinese medical question and answer instructions as well as multi-turn inquiry dialogues.
* SoulChat：
  * Website: https://github.com/scutcyr/SoulChat
    ![](https://img.shields.io/github/stars/scutcyr/SoulChat)
  * Introduction: SoulChat initialized with ChatGLM-6B, underwent instruct-tuning using a large-scale dataset of Chinese long-form instructions and multi-turn empathetic conversations in the field of psychological counseling. This instruct-tuning process aimed to enhance the model's empathy ability to guide users in expressing themselves, and capacity to provide thoughtful advice.
* DoctorGLM：
  * Website: https://github.com/Kent0n-Li/ChatDoctor
    ![](https://img.shields.io/github/stars/Kent0n-Li/ChatDoctor)
  * Introduction: A large Chinese diagnostic model based on ChatGLM-6B. This model has been fine-tuned using a Chinese medical conversation dataset, incorporating various fine-tuning techniques such as Lora and P-tuningv2, and has been deployed for practical use.
* HuatuoGPT：
  * Website: https://github.com/FreedomIntelligence/HuatuoGPT
    ![](https://img.shields.io/github/stars/FreedomIntelligence/HuatuoGPT)
  * Introduction: HuaTuo GPT is a GPT-like model that has undergone fine-tuning with specific medical instructions in Chinese. This model is a Chinese Language Model (LLM) designed specifically for medical consultation. Its training data includes distilled data from ChatGPT and real data from doctors. During the training process, reinforcement learning from human feedback (RLHF) has been incorporated to improve its performance.
* HuatuoGPT-II：
  * Website: https://github.com/FreedomIntelligence/HuatuoGPT-II
    ![](https://img.shields.io/github/stars/FreedomIntelligence/HuatuoGPT-II)
  * Introduction: HuatuoGPT2 employs an innovative domain adaptation method to significantly boost its medical knowledge and dialogue proficiency. It showcases state-of-the-art performance in several medical benchmarks, especially surpassing GPT-4 in expert evaluations and the fresh medical licensing exams.

#### 4.2.2 English Medical Large Language Models

* GatorTron：
  * Website: https://github.com/uf-hobi-informatics-lab/GatorTron
    ![](https://img.shields.io/github/stars/uf-hobi-informatics-lab/GatorTron)
  * Introduction: An early LLM developed for the Healthcare domain, aims to investigate how systems utilizing unstructured EHRs can benefit from clinical LLMs with billions of parameters.
* Codex-Med：
  * Website: https://github.com/vlievin/medical-reasoning
    ![](https://img.shields.io/github/stars/uf-hobi-informatics-lab/GatorTron)
  * Introduction: Codex-Med aimed to investigate the effectiveness of GPT-3.5 models. Two multiple-choice medical exam question datasets, namely USMLE and MedMCQA, as well as a medical reading comprehension dataset called PubMedQA were utilized.
* Galactica：
  * Website: https://galactica.org/
  * Aiming to solve the problem of information overload in the scientific field, Galactica was proposed to store, combine, and reason about scientific knowledge, including Healthcare. Galactica was trained on a large corpus of papers, reference material, and knowledge bases to potentially discover hidden connections between different research and bring insights to the surface. 
* DeID-GPT：
  * Website: https://github.com/yhydhx/ChatGPT-API
    ![](https://img.shields.io/github/stars/yhydhx/ChatGPT-API)
  * Introduction: A novel GPT4-enabled de-identification framework which enables to automatically identify and remove the identifying information. 
* ChatDoctor：
  * Website: https://github.com/Kent0n-Li/ChatDoctor
    ![](https://img.shields.io/github/stars/Kent0n-Li/ChatDoctor)
  * Introduction: A Medical Chat Model Fine-Tuned on a Large Language Model Meta-AI (LLaMA) Using Medical Domain Knowledge.
* MedAlpaca：
  * Website: https://github.com/kbressem/medAlpaca
    ![](https://img.shields.io/github/stars/kbressem/medAlpaca)
  * Introduction: MedAlpaca employed an open-source policy that enables on-site implementation, aiming at mitigating privacy concerns. MedAlpaca is built upon the LLaMA with 7 and 13 billion parameters. 
* PMC-LLaMA：
  * Website: https://github.com/chaoyi-wu/PMC-LLaMA
    ![](https://img.shields.io/github/stars/chaoyi-wu/PMC-LLaMA)
  * Introduction: PMC-LLaMA is an open-source language model that by tuning LLaMA-7B on a total of 4.8 million biomedical academic papers for further injecting medical knowledge, enhancing its capability in the medical domain.
* Visual Med-Alpaca：
  * Website: https://github.com/cambridgeltl/visual-med-alpaca
    ![](https://img.shields.io/github/stars/cambridgeltl/visual-med-alpaca)
  * Introduction: Visual Med-Alpaca is an open-source, parameter-efficient biomedical foundation model that can be integrated with medical "visual experts" for multimodal biomedical tasks. Built upon the LLaMa-7B architecture, this model is trained using an instruction set curated collaboratively by GPT-3.5-Turbo and human experts. 
* GatorTronGPT：
  * Website: https://github.com/uf-hobi-informatics-lab/GatorTronGPT
    ![](https://img.shields.io/github/stars/uf-hobi-informatics-lab/GatorTronGPT)
  * Introduction: GatorTronGPT is a clinical generative LLM designed with a GPT-3 architecture comprising 5 or 20 billion parameters.  It utilizes a vast corpus of 277 billion words, consisting of a combination of clinical and English text. 
* MedAGI：
  * Website: https://github.com/JoshuaChou2018/MedAGI
    ![](https://img.shields.io/github/stars/JoshuaChou2018/MedAGI)
  * Introduction: A paradigm to unify domain-specific medical LLMs with the lowest cost and a possible path to achieving medical AGI, rather than it is a LLM.
* LLaVA-Med：
  * Website: https://github.com/microsoft/LLaVA-Med
    ![](https://img.shields.io/github/stars/microsoft/LLaVA-Med)
  * Introduction: LLaVA-Med was initialized with the general-domain LLaVA and then continuously trained in a curriculum learning fashion (first biomedical concept alignment then full-blown instruction-tuning).  
* Med-Flamingo：
  * Website: https://github.com/snap-stanford/med-flamingo
    ![](https://img.shields.io/github/stars/snap-stanford/med-flamingo)
  * Introduction: Med-Flamingo is a vision language model specifically designed to handle interleaved multimodal data comprising both images and text. Building on the achievements of Flamingo,  Med-Flamingo further enhances these capabilities for the medical domain by pre-training diverse multimodal knowledge sources across various medical disciplines.



## 5. Relevant Papers

### 5.1 The Post-ChatGPT Era: Helpful Papers

1. Large Language Models Encode Clinical Knowledge. [Paper Link](https://arxiv.org/abs/2212.13138)
2. Performance of ChatGPT on USMLE: The Potential of Large Language Models for AI-Assisted Medical Education. [Paper Link](https://journals.plos.org/digitalhealth/article?id=10.1371/journal.pdig.0000198)
3. Turing Test for Medical Advice from ChatGPT. [Paper Link](https://arxiv.org/abs/2301.10035)
4. Toolformer: Language Models Can Self-Learn to Use Tools. [Paper Link](https://arxiv.org/abs/2302.04761)
5. Check Your Facts and Try Again: Improving Large Language Models with External Knowledge and Automatic Feedback. [Paper Link](https://arxiv.org/abs/2302.12813)
6. Capability of GPT-4 in Medical Challenge Questions. [Paper Link](https://arxiv.org/abs/2303.13375)

### 5.2 Review Articles

1. Pretrained Language Models in Biomedical Field: A Systematic Review. [Paper Link](https://arxiv.org/abs/2110.05006)
2. Deep Learning Guide for Healthcare. [Paper Link](https://www.nature.com/articles/s41591-018-0316-z) Published in Nature Medicine.
3. A Survey of Large Language Models for Healthcare. [Paper Link](https://arxiv.org/abs/2310.05694) 

### 5.3 Task-Specific Articles

**Articles Related to Electronic Health Records**

1. Transfer Learning from Medical Literature for Section Prediction in Electronic Health Records. [Paper Link](https://www.aclweb.org/anthology/D19-1492/)
2. MUFASA: Multimodal Fusion Architecture Search for Electronic Health Records. [Paper Link](http://arxiv-download.xixiaoyao.cn/pdf/2102.02340.pdf)

**Medical Relation Extraction**

1. Leveraging Dependency Forest for Neural Medical Relation Extraction. [Paper Link](https://www.aclweb.org/anthology/D19-1020/)

**Medical Knowledge Graph**

1. Learning a Health Knowledge Graph from Electronic Medical Records. [Paper Link](https://www.nature.com/articles/s41598-017-05778-z)

**Auxiliary Diagnosis**

1. Evaluation and Accurate Diagnoses of Pediatric Diseases Using Artificial Intelligence. [Paper Link](https://www.nature.com/articles/s41591-018-0335-9)

**Medical Entity Linking (Normalization)**

1. Medical Entity Linking Using Triplet Network. [Paper Link](https://www.aclweb.org/anthology/W19-1912/)
2. A Generate-and-Rank Framework with Semantic Type Regularization for Biomedical Concept Normalization. [Paper Link](https://www.aclweb.org/anthology/2020.acl-main.748.pdf)
3. Deep Neural Models for Medical Concept Normalization in User-Generated Texts. [Paper Link](https://www.aclweb.org/anthology/P19-2055.pdf)

### 5.4 Conference Index

**List of Medical-Related Papers from ACL 2020**

1. A Generate-and-Rank Framework with Semantic Type Regularization for Biomedical Concept Normalization. [Paper Link](https://www.aclweb.org/anthology/2020.acl-main.748/)
2. Biomedical Entity Representations with Synonym Marginalization. [Paper Link](https://www.aclweb.org/anthology/2020.acl-main.335/)
3. Document Translation vs. Query Translation for Cross-Lingual Information Retrieval in the Medical Domain. [Paper Link](https://www.aclweb.org/anthology/2020.acl-main.613/)
4. MIE: A Medical Information Extractor towards Medical Dialogues. [Paper Link](https://www.aclweb.org/anthology/2020.acl-main.576/)
5. Rationalizing Medical Relation Prediction from Corpus-level Statistics. [Paper Link](https://www.aclweb.org/anthology/2020.acl-main.719/)

**List of Medical NLP Related Papers from AAAI 2020**

1. On the Generation of Medical Question-Answer Pairs. [Paper Link](https://arxiv.org/pdf/1811.00681.pdf)
2. LATTE: Latent Type Modeling for Biomedical Entity Linking. [Paper Link](https://arxiv.org/pdf/1911.09787.pdf)
3. Learning Conceptual-Contextual Embeddings for Medical Text. [Paper Link](https://arxiv.org/pdf/1908.06203.pdf)
4. Understanding Medical Conversations with Scattered Keyword Attention and Weak Supervision from Responses. [Paper Link](http://ir.hit.edu.cn/~car/papers/AAAI2020-Shi-medconv.pdf)
5. Simultaneously Linking Entities and Extracting Relations from Biomedical Text without Mention-level Supervision. [Paper Link](https://arxiv.org/pdf/1912.01070.pdf)
6. Can Embeddings Adequately Represent Medical Terminology? New Large-Scale Medical Term Similarity Datasets Have the Answer! [Paper Link](https://arxiv.org/pdf/2003.11082.pdf)

**List of Medical NLP Related Papers from EMNLP 2020**

1. Towards Medical Machine Reading Comprehension with Structural Knowledge and Plain Text. [Paper Link](https://www.aclweb.org/anthology/2020.emnlp-main.111.pdf)
2. MedDialog: Large-scale Medical Dialogue Datasets. [Paper Link](https://www.aclweb.org/anthology/2020.emnlp-main.743.pdf)
3. COMETA: A Corpus for Medical Entity Linking in the Social Media. [Paper Link](https://www.aclweb.org/anthology/2020.emnlp-main.253.pdf)
4. Biomedical Event Extraction as Sequence Labeling. [Paper Link](https://www.aclweb.org/anthology/2020.emnlp-main.431.pdf)
5. FedED: Federated Learning via Ensemble Distillation for Medical Relation Extraction. [Paper Link](https://www.aclweb.org/anthology/2020.emnlp-main.165.pdf) [Paper Analysis](https://blog.csdn.net/lrs1353281004/article/details/111877017)
6. Infusing Disease Knowledge into BERT for Health Question Answering, Medical Inference and Disease Name Recognition. [Paper Link](https://arxiv.org/pdf/2010.03746.pdf)
7. A Knowledge-driven Generative Model for Multi-implication Chinese Medical Procedure Entity Normalization. [Paper Link](https://www.aclweb.org/anthology/2020.emnlp-main.116.pdf)
8. BioMegatron: Larger Biomedical Domain Language Model. [Paper Link](https://www.aclweb.org/anthology/2020.emnlp-main.379.pdf)
9. Querying Across Genres for Medical Claims in News. [Paper Link](https://www.aclweb.org/anthology/2020.emnlp-main.139.pdf)



## 6. Open-source Toolkits

1. Tokenization tool: PKUSEG [Project Link](https://github.com/lancopku/pkuseg-python) Project Description: A multi-domain Chinese tokenization tool launched by Peking University, which supports selection in the medical field.



## 7. Industrial Solutions

1. [Lingyi Wisdom](https://01.baidu.com/index.html)
2. [Left Hand Doctor](https://open.zuoshouyisheng.com/)
3. [Yidu Cloud Research Institute - Medical Natural Language Processing](https://www.yiducloud.com.cn/academy.html)
4. [Baidu - Medical Text Structuring](https://ai.baidu.com/solution/mtp)
5. [Alibaba Cloud - Medical Natural Language Processing](https://help.aliyun.com/document_detail/179395.html)



## 8. Blog Sharing

1. [Alpaca: A Powerful Open Source Instruction Following Model](https://crfm.stanford.edu/2023/03/13/alpaca.html)
2. [Lessons Learned from Building Natural Language Processing Systems in the Medical Field](http://www.oreilly.com.cn/radar/?p=2083)
3. [Introduction to Medical Public Databases and Data Mining Techniques in the Big Data Era](https://mp.weixin.qq.com/s/tA44U4bJUttnROfrzpNYcQ)
4. [Looking at the Development of NLP Application in the Medical Field from ACL 2021, with Resource Download](https://mp.weixin.qq.com/s/RhcHvRWHRnYUg6u9vXoIGA)



## 9. Friendly Links

1. [awesome_Chinese_medical_NLP](https://github.com/GanjinZero/awesome_Chinese_medical_NLP)
2. [Chinese NLP Dataset Search](https://www.cluebenchmarks.com/dataSet_search.html)
3. [medical-data(Large Amount of Medical Related Data)](https://github.com/beamandrew/medical-data)
4. [Tianchi Dataset (Includes Multiple Medical NLP Datasets)](https://tianchi.aliyun.com/dataset)

