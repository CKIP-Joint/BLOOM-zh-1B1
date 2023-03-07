---
license: bigscience-bloom-rail-1.0
language:
- zh
- en
pipeline_tag: text-generation
widget:
 - text: "四月的某一天，天氣晴朗寒冷，"
 - text: "問：台灣最高的建築物是？答："
---

<h1 style='text-align: center '>BLOOM-zh</h1> 
<h2 style='text-align: center '><em>Traditional Chinese-enhanced BLOOM language model</em> </h2> 
<h3 style='text-align: center '>Model Card</h3>

Version 1.0 / 20.Feb.2023

This model is a joint collaboration between CKIP lab at Acedemia Sinica ([link](https://ckip.iis.sinica.edu.tw/)), MediaTek Research ([連結](https://www.mtkresearch.com/), [连结](https://www.mtkresearch.com/zh-hans/), [link](https://www.mtkresearch.com/en/)), and National Academy for Educational Research ([link](https://www.naer.edu.tw/)).

## Table of Contents
1. [Model Details](#model-details)
2. [Uses](#uses)
3. [Training Data](#training-data)
4. [Risks and Limitations](#risks-and-limitations)
5. [Recommendations](#recommendations)
6. [Model Card Authors](#model-card-authors)

## Model Details  
BLOOM-zh is a language model with enhanced Traditional Chinese capability. It is derived from [BLOOMZ](https://huggingface.co/bigscience/bloomz). 
BLOOM-zh is trained extendedly on large amount of Traditional Chinese text data.

The model can be downloaded on the Huggingface Model Hub: [link](https://huggingface.co/ckip-joint/bloom-1b1-zh)

### Basics
    
* **Developed by:** MediaTek Research
* **Model Type:** Transformer-based Language Model
* **Version:** 1.0.0
* **Languages:** Multiple; see [training data](#training-data)
* **License:** MEDIATEK RESEARCH License ([link](https://huggingface.co/ckip-joint/bloom-1b1-zh/blob/main/LICENSE_MR.md)) and RAIL License v1.0 ([link](https://huggingface.co/spaces/bigscience/license))
* **Release Date Estimate:** Wednesday, 22.February.2023
* **Send Questions to:** info@mtkresearch.com
* **Cite as:** MediaTek Research: Traditional Chinese-enhanced BLOOM language model. International, February 2023.
* **Organizations of contributors:** 
  * MediaTek Research
  * Academia Sinica
  * National Academy for Educational Research


### Technical Specifications
*This section provides information for people who work on model development.*

For technical specifications, please refer to [BLOOM](https://huggingface.co/bigscience/bloom-1b1#model-details).

### Environmental Impact

For environmental impact, please refer to [BLOOM](https://huggingface.co/bigscience/bloom-1b1#model-details).

## Uses

*This section addresses questions around how the model is intended to be used, discusses the foreseeable users of the model (including those affected by the model), and describes uses that are considered out of scope or misuse of the model. 
It provides information for anyone considering using the model or who is affected by the model.*

For the uses of the model, please refer to [BLOOM](https://huggingface.co/bigscience/bloom-1b1#uses).

## Training Data
*This section provides a high-level overview of the training data. It is relevant for anyone who wants to know the basics of what the model is learning.*
    
We trained the 1B1 parameter model on a total of 6 Billion tokens of mostly high quality Traditional Chinese text. Details are provided in the [paper(work in progress)](https://arxiv.org/).

## Risks and Limitations
*This section identifies foreseeable harms and misunderstandings.*
    
For risks and limitations, please refer to [BLOOM](https://huggingface.co/bigscience/bloom-1b1#risks-and-limitations).

### Factors 
*This section lists some different aspects of BLOOM models. Its focus is on those aspects that are likely to give rise to high variance in model behavior.*

- The model is trained on Traditional Chinese and English. However, the pretrained weights capture more than 40 different languages.

- The model is trained on web crawled data, news articles, novels, knowledge sources (encyclopedia, education sector) and instructions


## Recommendations

*This section provides information on warnings and potential mitigations.*

For recommendations, please refer to [BLOOM](https://huggingface.co/bigscience/bloom-1b1#recommendations).

    
## Model Card Authors
*Ordered roughly chronologically and by amount of time spent.*

Philipp Ennen, Po-Chun Hsu, Chan-Jan Hsu, Chang-Le Liu, Yen-Chen Wu, Yin-Hsiang Liao, Chin-Tung Lin, Da-Shan Shiu, Wei-Yun Ma
<!-- # Bloom_eval -->
