# BLOOM-zh: Extending the Pre-Training of BLOOM for Improved Support of Traditional Chinese

The multilingual language model BLOOM-zh features enhanced support for Traditional Chinese. BLOOM-zh has its origins in the open-source BLOOM models presented by BigScience in 2022. The technical specification can be found in the corresponding [paper](https://arxiv.org/abs/2303.04715). As of March 9nd 2023, the 1B1 parameter model is released with following unique features:

- Multilingual: supports Traditional Chinese as well as the pretrained languages of BLOOM

- Performance: performs significantly better on Traditional Chinese than the original BLOOM

- Free-to-download: model weights are free to download 

## News

- **[2023.03.09]** Our [paper](https://arxiv.org/abs/2303.04715) for Bloom-zh is out!

- **[2023.03.07]** [Bloom-zh 1B1](https://huggingface.co/ckip-joint/bloom-1b1-zh) is out!

## Getting Started

### Model weights

| Model        | Additional training tokens | Download                                       |
| ------------ | --------------- | ---------------------------------------------- |
| Bloom-zh 1B1 | 11.5 B           | (to be updated) https://huggingface.co/ckip-joint/bloom-1b1-zh |
| Bloom-zh 3B  | 13 B           | -                                              |

### Evaluation

For perplexity evaluation, we used the evaluation pipeline presented in the original [megatron-deepspeed](https://github.com/microsoft/Megatron-DeepSpeed) library. For evaluating the downstream task performance, please follow the instructions of the [Traditional Chinese Evaluation Suite](https://github.com/CKIP-Joint/Evaluator). We evaluated Bloom-zh on following downstream tasks:

- TTQA: Taiwan Trivia Question Answering. Please refer to [paper](https://arxiv.org/abs/2303.04715) 
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
