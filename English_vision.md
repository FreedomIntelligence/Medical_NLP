# Medical_NLP


>Since [Cris Lee](https://github.com/lrs1353281004) left the medical NLP field in 2021, this repo is now maintained by [Xidong Wang](https://github.com/wangxidong06).

Summary of medical NLP evaluations/competitions, datasets, papers and pre-trained models.

[中文版本](https://github.com/FreedomIntelligence/Chinese_medical_NLP) [English_version](https://github.com/FreedomIntelligence/Chinese_medical_NLP/blob/master/English_vision.md)

* [Medical_NLP](#medical_nlp)
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
      * [4.1 Medical LLMs](#41-medical-LLMs)
      * [4.2 Chinese Medical - Refer <a href="https://github.com/HqWu-HITCS/Awesome-Chinese-LLM#%E5%8C%BB%E7%96%97">here</a>](#41-chinese-medical---refer-here)
      * [4.3 General Large-scale Chinese Models - Refer <a href="https://github.com/HqWu-HITCS/Awesome-Chinese-LLM#%E9%80%9A%E7%94%A8">here</a>](#42-general-large-scale-chinese-models---refer-here)
   * [5. Relevant Papers](#5-relevant-papers)
      * [5.1 OpenAI](#51-openai)
      * [5.2 Papers That Might Be Helpful in the Post-ChatGPT Era (Continuously Updated)](#52-papers-that-might-be-helpful-in-the-post-chatgpt-era-continuously-updated)
      * [5.2 The Post-ChatGPT Era: Helpful Papers (Continuous Updates)](#52-the-post-chatgpt-era-helpful-papers-continuous-updates)
      * [5.3 Review Articles](#53-review-articles)
      * [5.4 Task-Specific Articles](#54-task-specific-articles)
      * [5.4 Conference Index](#54-conference-index)
   * [6. Open-source Toolkits](#6-open-source-toolkits)
   * [7. Industrial Solutions](#7-industrial-solutions)
   * [8. Blog Sharing](#8-blog-sharing)
   * [9. Friendly Links](#9-friendly-links)


## 1. Evaluation

### 1.1 Chinese Medical Benchmark Evaluation: CMB / CMExam / PromptCBLUE

| Name        | Source                                                       | GitHub Link                                 |
| ----------- | ------------------------------------------------------------ | ------------------------------------------- |
| CMB         | Various clinical medical examinations; complex clinical case consultations | https://github.com/FreedomIntelligence/CMB  |
| CMExam      | Past questions from the Medical Practitioner Qualification Examination | https://github.com/williamliujl/CMExam      |
| PromptCBLUE | CBLUE                                                        | https://github.com/michael-wzhu/PromptCBLUE |
| CBLUE       | Academic evaluation competitions from past CHIP conferences and datasets from Alibaba Quark's medical search service | https://github.com/CBLUEbenchmark/CBLUE     |

### 1.2 English Medical Benchmark Evaluation:

| Name          | Source | Description                               | GitHub Link | Official Evaluation Website Link |
| ------------- | ------ | ----------------------------------------- | ----------- | -------------------------------- |
| MultiMedBench | Google | A large-scale multimodal generative model |             |                                  |

## 2. Competitions

### 2.1 Ongoing Competitions

None at the moment. Additions are welcome~

### 2.2 Completed Competitions

**English**

| Name                                                         | Source                        | Link                                                         |
| ------------------------------------------------------------ | ----------------------------- | ------------------------------------------------------------ |
| BioNLP Workshop 2023 Shared Task                             | BioNLP Workshop               | https://aclweb.org/aclwiki/BioNLP_Workshop#SHARED_TASKS_2023 |
| MedVidQA 2023                                                | National Institutes of Health | https://medvidqa.github.io/index.html                        |
| MEDIQA-2021                                                  | NAACL-BioNLP 2021 workshop    | https://sites.google.com/view/mediqa2021                     |
| ICLR-2021 International Competition for Medical Dialogue Generation and Automatic Diagnosis | ICLR 2021 workshop            | https://mlpcp21.github.io/pages/challenge                    |

**Chinese**

| Name                                                         | Source                                                       | Link                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| NLP for Medical Imaging - Medical Imaging Diagnostic Report Generation | Track One of 2023 Global AI Technology Innovation Competition | https://gaiic.caai.cn/ai2023/                                |
| Non-standard Disease Claims Simple Triage Challenge 2.0      | iFlytek                                                      | http://challenge.xfyun.cn/topic/info?type=disease-claims-2022&ch=ds22-dw-sq03 |
| Evaluation Task of the 8th China Health Information Processing Conference (CHIP2022) | CHIP2022                                                     | http://cips-chip.org.cn/)                                    |
| iFlytek - Medical Entity and Relationship Recognition Challenge | iFlytek                                                      | http://www.fudan-disc.com/sharedtask/imcs21/index.html       |

## 3. Datasets

### 3.1 Chinese

| Name                                                         | Description                                                  | Link                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Huatuo-26M                                                   | Huatuo-26M is the largest Traditional Chinese Medicine (TCM) Q&A dataset to date. | https://github.com/FreedomIntelligence/Huatuo-26M            |
| Yidu-S4K                                                     | Named Entity Recognition, Entity and Attribute Extraction    | http://openkg.cn/dataset/yidu-s4k                            |
| Yidu-N7K                                                     | Clinical Language Standardization                            | http://openkg.cn/dataset/yidu-n7k                            |
| Chinese Medical Q&A Dataset                                  | Medical Q&A                                                  | https://github.com/zhangsheng93/cMedQA2                      |
| Chinese Doctor-Patient Dialogue Data                         | Medical Q&A                                                  | https://github.com/UCSD-AI4H/Medical-Dialogue-System         |
| Chinese Medical Dialogue Dataset                             | Medical Q&A data from six departments                        | https://github.com/Toyhom/Chinese-medical-dialogue-data      |
| CPubMed-KG (4.4M triples)                                    | Full-text journal data of high quality from the Chinese Medical Association | https://cpubmed.openi.org.cn/graph/wiki                      |
| CBLUE                                                        | Covers medical text information extraction (entity recognition, relation extraction) | https://github.com/CBLUEbenchmark/CBLUE                      |
| Chinese Medical Knowledge Graph CMeKG (1M triples)           | CMeKG (Chinese Medical Knowledge Graph)                      | http://cmekg.pcl.ac.cn/                                      |
| cMedQA2 (108K)                                               | Chinese medical Q&A dataset with over 100,000 entries.       | https://github.com/zhangsheng93/cMedQA2                      |
| xywy-KG(294K triples)                                        | 44.1K entities 294.1K triples                                | https://github.com/baiyang2464/chatbot-base-on-Knowledge-Graph |
| 39Health-KG (210K triples)                                   | Includes 15 pieces of information, with 7 types of entities, about 37,000 entities, and 210,000 entity relationships. | https://github.com/zhihao-chen/QASystemOnMedicalGraph        |
| CHIP Annual Evaluation (Official Evaluation)                 | CHIP Annual Evaluation (Official Evaluation)                 | http://cips-chip.org.cn/2022/callforeval ; http://www.cips-chip.org.cn/2021/ ; http://cips-chip.org.cn/2020/ |
| Ruijin Hospital Diabetes Dataset (Diabetes)                  | Diabetes literature mining and knowledge graph construction using diabetes-related textbooks and research papers | https://tianchi.aliyun.com/competition/entrance/231687/information |
| Tianchi Novel Coronavirus Pneumonia Question Matching Competition (Novel Coronavirus) | The competition data includes: anonymized medical problem data pairs and annotated data. | https://tianchi.aliyun.com/competition/entrance/231776/information |

### 3.2 English

| Name        | Description                                                  | Link                                          |
| ----------- | ------------------------------------------------------------ | --------------------------------------------- |
| PubMedQA    | Medical Q&A dataset extracted from PubMed                    | https://arxiv.org/abs/1909.06146              |
| COMETA      | Medical entity linking data in social media. Published at EMNLP2020 | https://www.siphs.org/                        |
| MedMentions | Biomedical entity linking dataset based on PubMed abstracts  | https://github.com/chanzuckerberg/MedMentions |
| webMedQA    | Medical Q&A                                                  | https://github.com/hejunqing/webMedQA         |
| MediQA      | Text summarization                                           | https://sites.google.com/view/mediqa2021      |

## 4. Open-source Models

### 4.1 Medical LLMs

#### 4.1.1 Chinese Medical Large Language Models

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
  * HuaTuo GPT is a GPT-like model that has undergone fine-tuning with specific medical instructions in Chinese. This model is a Chinese Language Model (LLM) designed specifically for medical consultation. Its training data includes distilled data from ChatGPT and real data from doctors. During the training process, reinforcement learning from human feedback (RLHF) has been incorporated to improve its performance.

#### 4.1.2 English Medical Large Language Models

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

### 4.2 Chinese Medical - Refer [here](https://github.com/HqWu-HITCS/Awesome-Chinese-LLM#医疗)

### 4.3 General Large-scale Chinese Models - Refer [here](https://github.com/HqWu-HITCS/Awesome-Chinese-LLM#通用)



## 5. Relevant Papers

### 5.1 OpenAI

**Previous works in the RLHF domain before RLHF + NLP by OpenAI**

- Bayesian Methods for Policy Learning from Preference Queries in Trajectories (NIPS 2012) Paper link: https://papers.nips.cc/paper/2012/hash/16c222aa19898e5058938167c8ab6c57-Abstract.html
- Training Robots Through Human Feedback: A Case Study (ICSR 2013) Paper link: https://link.springer.com/chapter/10.1007/978-3-319-02675-6_46
- APRIL: Active Preference Learning-based Reinforcement Learning (2012) Paper link: https://arxiv.org/abs/1208.0984
- Programming by Feedback (2014) Paper link: https://hal.inria.fr/hal-00980839
- Learning Rewards from Human Preferences and Demonstrations in Atari (2018) Paper link: https://arxiv.org/abs/1811.06521

**OpenAI RLHF thought chain**

1. Efficient Feedback (2015) Start from this [blog](https://ai-alignment.com/efficient-feedback-a347748b1557#.exjnsupts)! Address: https://ai-alignment.com/efficient-feedback-a347748b1557#.exjnsupts
2. [Reinforcement Learning with Corrupted Reward Channel](https://openai.com/research/faulty-reward-functions)(2017.3 openai) OpenAI's consideration on RL Policy safety, 4/5 of the attempts Paper link: https://arxiv.org/abs/1705.08417 Blog: https://openai.com/research/faulty-reward-functions
3. [Deep Reinforcement Learning from Human Preferences](https://openai.com/research/learning-from-human-preferences)(2017.6 openai) An initial exploration of RLHF in RL Paper link: https://arxiv.org/abs/1706.03741
4. [Improving AI Safety by Debate](https://openai.com/research/debate) (2018.5 openai) Implementing RL safety through debate, addressing 2. Paper link: https://arxiv.org/abs/1805.00899
5. [Supervising Strong Learners by Amplifying Weak Experts](https://openai.com/research/learning-complex-goals-with-iterated-amplification) (2018.10 openai) Iterative amplification of RL safety technology, addressing 2. Paper link: https://arxiv.org/abs/1810.08575
6. [Fine-Tuning GPT-2 from Human Preferences](https://openai.com/research/fine-tuning-gpt-2) (2019 openai) First NLP+RLHF! Paper link: https://arxiv.org/abs/1909.08593
7. [Learning to Summarize with Human Feedback](https://openai.com/research/learning-to-summarize-with-human-feedback)(openai 2020) Second try NLP+RLHF! Paper link: https://arxiv.org/abs/2009.01325
8. [TruthfulQA](https://openai.com/research/truthfulqa): Measuring the Capacity of Models to Mimic Human Lies (2021.8.9) Last sentence of the abstract: The largest models are usually the least truthful, and we suggest that tuning the training objective separately rather than enlarging the model alone improves truthfulness. This directly leads to 9. Paper link: https://arxiv.org/abs/2109.07958
9. [Instruct GPT](https://openai.com/research/instruction-following)(2022.1 openai) The technology explored in 0.0.2.6/7 finally aligns with GPT-3! Key point: Despite having over 100 times fewer parameters, our label creators prefer the outputs of the 1.3B InstructGPT model to those of the 175B GPT-3 model. Paper link: https://arxiv.org/abs/2203.02155

**Iteration process of GPT-x and its variants**

Iteration of hardware resources and scheduling

1. [Kubernetes](https://kubernetes.io/)
2. [Scaling Kubernetes to 2,500 Nodes](https://openai.com/research/scaling-kubernetes-to-2500-nodes) Blog link: https://openai.com/research/scaling-kubernetes-to-2500-nodes
3. [Scaling Kubernetes to 7,500 Nodes](https://openai.com/research/scaling-kubernetes-to-7500-nodes) Provides scalable infrastructure for large models. It also provides infrastructure for fast small-scale iterative research such as neural language model scaling laws. Blog link: https://openai.com/research/scaling-kubernetes-to-7500-nodes

Iteration of models

1. [GPT](https://openai.com/research/language-unsupervised)(2018.6.11 openai) Paper link: https://cdn.openai.com/research-covers/language-unsupervised/language_understanding_paper.pdf
2. [GPT-2](https://openai.com/research/better-language-models)(2019.2.14 openai) Paper link: https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf
3. [GPT-3: Language Models are Few-Shot Learners](https://openai.com/research/language-models-are-few-shot-learners) (2020.3.28 openai) Paper link: https://arxiv.org/abs/2005.14165
4. [CLIP](https://openai.com/research/clip) Learning Transferable Visual Models from Natural Language Supervision (2021.1.5openai) Paper link: https://arxiv.org/abs/2103.00020
5. [CodeX](https://openai.com/blog/openai-codex) Evaluating Large Language Models Trained on Code (2021.6.7 openai) Paper link: https://arxiv.org/abs/2107.03374
6. [Instruct GPT](https://openai.com/research/instruction-following)(2022.6.27 openai) Paper link: https://arxiv.org/abs/2203.02155
7. [GPT-4](https://openai.com/research/gpt-4) (openai 2023.3.14) Paper link: https://cdn.openai.com/papers/gpt-4.pdf

### 5.2 Papers That Might Be Helpful in the Post-ChatGPT Era (Continuously Updated)

1. Large Language Models Encode Clinical Knowledge Paper link: https://arxiv.org/abs/2212.13138
2. Performance of ChatGPT on USMLE: The Potential for AI-Assisted Medical Education Paper link: https://journals.plos.org/digitalhealth/article?id=10.1371/journal.pdig.0000198
3. AI-Generated Writing Imitates Human Writing in Biomedical Research: A Double-Blind Randomized Study Paper link: https://jamanetwork.com/journals/jamanetworkopen/fullarticle/2787608

4. Potential Pitfalls and Promises of Artificial Intelligence in Health Care Paper link: https://jamanetwork.com/journals/jamanetworkopen/fullarticle/2787599
5. Using ChatGPT-4 to Answer Questions about Medicines: A Validation Study Paper link: https://www.jmir.org/2023/7/e33683/
6. The Impact of OpenAI's ChatGPT on Patient-Doctor Communication: An Empirical Study Paper link: https://www.jmir.org/2023/7/e33684/



### 5.2 The Post-ChatGPT Era: Helpful Papers (Continuous Updates)

1. Large Language Models Encode Clinical Knowledge. [Paper Link](https://arxiv.org/abs/2212.13138)
2. Performance of ChatGPT on USMLE: The Potential of Large Language Models for AI-Assisted Medical Education. [Paper Link](https://journals.plos.org/digitalhealth/article?id=10.1371/journal.pdig.0000198)
3. Turing Test for Medical Advice from ChatGPT. [Paper Link](https://arxiv.org/abs/2301.10035)
4. Toolformer: Language Models Can Self-Learn to Use Tools. [Paper Link](https://arxiv.org/abs/2302.04761)
5. Check Your Facts and Try Again: Improving Large Language Models with External Knowledge and Automatic Feedback. [Paper Link](https://arxiv.org/abs/2302.12813)
6. Capability of GPT-4 in Medical Challenge Questions. [Paper Link](https://arxiv.org/abs/2303.13375)

### 5.3 Review Articles

1. Pretrained Language Models in Biomedical Field: A Systematic Review. [Paper Link](https://arxiv.org/abs/2110.05006)
2. Deep Learning Guide for Healthcare. [Paper Link](https://www.nature.com/articles/s41591-018-0316-z) Published in Nature Medicine.

### 5.4 Task-Specific Articles

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
