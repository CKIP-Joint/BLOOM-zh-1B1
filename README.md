---
license: bigscience-bloom-rail-1.0
language:
- en
- zht
pipeline_tag: text-generation
---

<h1 style='text-align: center '>BLOOM-zh</h1> 
<h2 style='text-align: center '><em>Open-access Multilingual Language Model based on BLOOM</em> </h2> 
<h3 style='text-align: center '>Model Card</h3>

Version 1.0 / 13.Feb.2023

This model is a close collaboration between MediaTek Research, National Academy for Educational Research, and CKIP lab, Acedemia Sinica.

## Table of Contents
1. [Model Details](#model-details)
2. [Uses](#uses)
3. [Training Data](#training-data)
4. [Risks and Limitations](#risks-and-limitations)
5. [Evaluation](#evaluation)
6. [Recommendations](#recommendations)
7. [Glossary and Calculations](#glossary-and-calculations)
8. [More Information](#more-information)
9. [Model Card Authors](#model-card-authors)

## Model Details  
BLOOM-zh is a modification from [BLOOM](https://huggingface.co/bigscience/bloom). 
BLOOM-zh is trained extendedly on larger amounts of Traditional Chinese text data while it still maintains its pretrained English ability.
    

### Basics
*This section provides information for anyone who wants to know about the model.*

<details>
<summary>Click to expand</summary> <br/>
    
**Developed by:** MediaTek Research ([website](https://www.mtkresearch.com/))
    
**Model Type:** Transformer-based Language Model

**Version:** 1.0.0

**Languages:** Multiple; see [training data](#training-data)

**License:** MEDIATEK RESEARCH License ([link](https://huggingface.co/MediaTek-Research/bloom-1b1-zh/blob/main/LICENSE_MR.md)) and RAIL License v1.0 ([link](https://huggingface.co/spaces/bigscience/license))

**Release Date Estimate:** Tuesday, 14.February.2023

**Send Questions to:** info@mtkresearch.com

**Cite as:** MediaTek Research, MediaTek Research Open-access Multilingual Language Model based on BLOOM. International, February 2023.

**Organizations of contributors:** 
    
* MediaTek Research
* Academia Sinica

</details>

### Technical Specifications
*This section provides information for people who work on model development.*

<details>
<summary>Click to expand</summary><br/>

**Model Architecture:** Modified from Megatron-LM GPT2 (see [paper](https://arxiv.org/abs/1909.08053), [BLOOM Megatron code](https://github.com/bigscience-workshop/Megatron-DeepSpeed)):

* Decoder-only architecture

* Layer normalization applied to word embeddings layer (`StableEmbedding`; see [code](https://github.com/facebookresearch/bitsandbytes), [paper](https://arxiv.org/pdf/2110.02861.pdf))

* ALiBI positional encodings (see [paper](https://arxiv.org/pdf/2108.12409.pdf)), with GeLU activation functions

* 1,065,314,304 parameters:

    * 385,351,680 embedding parameters

    * 24 layers, 16 attention heads

    * Hidden layers are 1536-dimensional

    * Sequence length of 2048 tokens used (see [BLOOM tokenizer](https://huggingface.co/bigscience/tokenizer), [tokenizer description](#tokenization))

**Objective Function:** Cross Entropy with mean reduction (see [API documentation](https://pytorch.org/docs/stable/generated/torch.nn.CrossEntropyLoss.html#torch.nn.CrossEntropyLoss)).
    
**Compute infrastructure:** 

* Hardware: 8 A6000 48GB GPUs (1 node):


* Software:
  
    *   Bigscience Megatron-DeepSpeed ([Github link](https://github.com/bigscience-workshop/Megatron-DeepSpeed))
  
    *   Megatron-DeepSpeed ([Github link](https://github.com/bigscience-workshop/Megatron-DeepSpeed))

    *   DeepSpeed ([Github link](https://github.com/microsoft/DeepSpeed))

    *   PyTorch (pytorch-1.11 w/ CUDA-11.5; see [Github link](https://github.com/pytorch/pytorch))

    *   apex ([Github link](https://github.com/NVIDIA/apex))


#### **Training**

Details are provided in the [paper](https://arxiv.org/).

- Number of epochs: 1

- Dates: Feb. 2023

#### **Tokenization**
    
The BLOOM tokenizer ([link](https://huggingface.co/bigscience/tokenizer)) is a learned subword tokenizer trained using:
    
- A byte-level Byte Pair Encoding (BPE) algorithm 

- A simple pre-tokenization rule, no normalization

- A vocabulary size of 250,680

It was trained on a subset of a preliminary version of the corpus using alpha-weighting per language.    
    
</details>


### Environmental Impact

<details>
<summary>Click to expand</summary><br/>

Please refer to [Model card](https://huggingface.co/bigscience/bloom-1b1#model-details).


</details>
<p>&nbsp;</p>

## Uses

*This section addresses questions around how the model is intended to be used, discusses the foreseeable users of the model (including those affected by the model), and describes uses that are considered out of scope or misuse of the model. 
It provides information for anyone considering using the model or who is affected by the model.*


<details>
<summary>Click to expand</summary><br/>
    
Please refer to [Model card](https://huggingface.co/bigscience/bloom-1b1#uses).
    
</details>
<p>&nbsp;</p>

## Training Data
*This section provides a high-level overview of the training data. It is relevant for anyone who wants to know the basics of what the model is learning.*


<details>
<summary>Click to expand</summary><br/>
    
We trained the 1B1 parameter model on a total of 6 Billion tokens mainly crawled from the internet and provided from National Academy for Educational Research, 75% of the training data is Traditional Chinese, 25% is English.
    
</details>    
</details>
<p>&nbsp;</p>

## Risks and Limitations
*This section identifies foreseeable harms and misunderstandings.*

<details>
<summary>Click to expand</summary><br/>
    
Please refer to [Model card](https://huggingface.co/bigscience/bloom-1b1#risks-and-limitations).

</details>
<p>&nbsp;</p>

### Factors 
*This section lists some different aspects of BLOOM models. Its focus is on those aspects that are likely to give rise to high variance in model behavior.*

- The model is trained on Traditional Chinese and English. However, the pretrained weights capture more than 40 different languages.

- The model is trained on web crawled data, news articles, novels, knowledge sources (encyclopedia, education sector) and instructions

</details>
<p>&nbsp;</p>

## Recommendations

*This section provides information on warnings and potential mitigations.*


<details>
<summary>Click to expand</summary><br/>

Please refer to [Model card](https://huggingface.co/bigscience/bloom-1b1#recommendations).

</details>
<p>&nbsp;</p>

    
## Model Card Authors
*Ordered roughly chronologically and by amount of time spent.*

Philipp Ennen, Po-Chun Hsu, Chan-Jan Hsu, Chang-Le Liu, Yin-Hsiang Liao, Chin-Tung Lin, Jezabel Rodriguez Garcia, Federica Freddi, Da-Shan Shiu, Wei-Yun Ma
# Bloom_eval
