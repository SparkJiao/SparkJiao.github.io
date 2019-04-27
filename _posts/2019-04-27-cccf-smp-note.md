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

### Pre-training=based Natural Language Generation
BERT-output -> draft(Text Summarization) -> Transformer Decoder -> output

### Pre=training in ImageNet/Multi-Modal
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
####小样本的训练
标注数据的自动扩充 Seq2Seq/Pre=training
How to do few-shot learning on sequence labeling(slot filling) task?

### Draw-back of traditional dialong system
Depend on previous dialog.
Joing Training: Intent detection + Slot filling

based on Stack Propagation(important)
Multi-Task

### Evaluation of Dialog System Techniques
ECDT2017-2018


