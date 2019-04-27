---
title: '4.27 CCCF SMP Notes'
date: 2019-04-27
permalink: /posts/2019/0427/cccf-smp-notes/
tags:
  - notes
---

4.27 中国中文信息学会 社会媒体处理（SMP）专委会 首届“社交机器人”论坛

## Pretraining in NLP and CV

### ULMFit
double fine-tune

### CoVe
Supervised Language Model

### MS: KnowledgeBERT for Semantic Parsing
MSPars: A Multi-Perspective Semantic Parsing Dataset for Knowledge-based Question Answering

### Pre-training-based Natural Language Generation
BERT-output -> draft(Text Summarization) -> Transformer Decoder -> output

### Pre-training in ImageNet/Multi-Modal
ImageBERT
Image object + text -> BERT

### VideoBERT(Google)
videos -> frames -> token -> BERT

### Application: Video QA, Summarization and Chat.
Video span like machine reading comprehension.

## NLU in Task-Oriented Dialog System
intent detection, slot filling, state tracking.

### Intent Detection
### Slot Filling
### Dialog Management
Reinforcement Learning

### Dialog Generation
based on Pattern/LM/Seq2Seq

### 对话技术平台
希望中小型开发者只需要上传自己的数据，即可开发自己的对话系统。

哈工大聊天机器人“笨笨”/任务型对话系统

### Few-shot Learning
#### 小样本的训练
标注数据的自动扩充 Seq2Seq/Pre-training

How to do few-shot learning on sequence labeling(slot filling) task?

### Draw-back of traditional dialong system
Depend on previous dialog.

Joing Training: Intent detection + Slot filling based on Stack Propagation(important) and Multi-Task

### Evaluation of Dialog System Techniques
ECDT2017-2018

## Alibaba

Asememble Learning
Hybrid CNN   
冷启动快速端到端测试 Deep reinforcement Learning


### MRC for Unstructured Data
based on SLQA -> EMNLP

## Open-Domain Non-Oriented Dialog System

### Retrieval-Based Chatbot

### Multi-View: Relevence, Interestingness, Informativeness,

### Non-Sentential Utterance Resolution

### Retrieval from Non-Dialogue Corpus
- 和阅读理解有什么区别？ 专业知识可能会粒度特别的细，所以需要开放域（大概是这个意思）

### Neural Responce Generation
- The "Bland Response" Problem: I dont't know/Well/Great/Fine, Jiwei Li
  - Adversarial Training
  - discriminator生成的是比较细粒度的东西，用一个单一的score作为reward去回传会不会有问题，所以把？？？？和embedding直接乘起来， 剩下的没记下来orz 好像组会讲过XD
- The "Myopia Problem" of Beam Search

### Child Friendly Social Chatbot
- 避免一些对小孩不合适的话题，谈恋爱，结婚生子等
- 先用一个用儿童语料库训练的语言模型去过滤
- 生成模型本身比较保守，双重过滤后概率会远小于真实世界的概率

## Q&A

### Constraint on Dialog Generation
