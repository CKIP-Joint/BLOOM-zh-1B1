# BLOOM-zh: Traditional Chinese-Improved BLOOM 

The multilingual language model BLOOM-zh features enhanced support for Traditional Chinese over BLOOM. BLOOM-zh has its origins in the open-source BLOOM models presented by BigScience in 2022. The technical specification can be found in the corresponding [paper](https://arxiv.org/abs/2303.04715). 

The first 1B1 parameter model was released on March 9, 2023. The 3B parameter model was released on April 10, 2023. We will continue to release larger models trained on more tokens with performance/behavior fixes. 

## Features

- Performance: BLOOM-zh performs significantly better on Traditional Chinese than the stock BLOOM

- Free-to-download: model weights are free to download 

## News

- **[2023.04.10]** [Bloom-zh 3B](https://huggingface.co/ckip-joint/bloom-3b-zh) is out!

- **[2023.04.10]** First iteration of [Bloom-zh 1B1](https://huggingface.co/ckip-joint/bloom-1b1-zh), this one pre-trained with 11B Traditional Chinese tokens.

- **[2023.03.09]** Our [paper](https://arxiv.org/abs/2303.04715) for Bloom-zh is out!

- **[2023.03.07]** [Bloom-zh 1B1](https://huggingface.co/ckip-joint/bloom-1b1-zh) is out!

## Getting Started

### Model weights

| Model        | Additional training tokens | Download                                       |
| ------------ | -------------------------- | ---------------------------------------------- |
| Bloom-zh 1B1 | 11.5 B                     | https://huggingface.co/ckip-joint/bloom-1b1-zh |
| Bloom-zh 3B  | 13 B                       | https://huggingface.co/ckip-joint/bloom-3b-zh  |

### Evaluation

For perplexity evaluation, we used the evaluation pipeline presented in the original [megatron-deepspeed](https://github.com/microsoft/Megatron-DeepSpeed) library. For evaluating the downstream task performance, please follow the instructions of the [Traditional Chinese Evaluation Suite](https://github.com/CKIP-Joint/Evaluator). We evaluated Bloom-zh on following downstream tasks:

- TTQA: Taiwan Trivia Question Answering. Please refer to our [paper](https://arxiv.org/abs/2303.04715) 
- DRCD: Please refer to [DRCD](https://github.com/DRCKnowledgeTeam/DRCD)
- FGC: Please refer to [科技大擂台](https://scidm.nchc.org.tw/dataset/grandchallenge2020/resource/af730fe7-7f95-4af2-b4f4-1ca09406b35a)

## License

The use of BLOOM-zh model weights is subject to the [Model License](https://huggingface.co/ckip-joint/bloom-1b1-zh/blob/main/LICENSE_MR.md).

## Citation

If you find our work useful, please consider citing BLOOM-zh:

```
@article{ennen2023extending,
  title={Extending the Pre-Training of BLOOM for Improved Support of Traditional Chinese: Models, Methods and Results},
  author={Ennen, Philipp and Hsu, Po-Chun and Hsu, Chan-Jan and Liu, Chang-Le and Wu, Yen-Chen and Liao, Yin-Hsiang and Lin, Chin-Tung and Shiu, Da-Shan and Ma, Wei-Yun},
  journal={arXiv preprint arXiv:2303.04715},
  year={2023}
}
```
