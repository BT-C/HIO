# HIO (Alleviating Hallucinations in Large Vision-Language Models through Hallucination-Induced Optimization) <a href='https://arxiv.org/pdf/2405.15356'><img src='https://img.shields.io/badge/Paper-Arxiv-red'></a>

**Center for Future Media, University of Electronic Science and Technology of China**

Beitao Chen, Xinyu Lyu, Lianli Gao, Jingkuan Song, Heng Tao Shen

<img src="./assets/framework.png">

# Abstract
Although Large Visual Language Models (LVLMs) have demonstrated exceptional abilities in understanding multimodal data, they invariably suffer from hallucinations, leading to a disconnect between the generated text and the corresponding images. Almost all current visual contrastive decoding methods attempt to mitigate these hallucinations by introducing visual uncertainty information that appropriately widens the contrastive logits gap between hallucinatory and targeted ones. However, due to uncontrollable nature of the global visual uncertainty, they struggle to precisely induce the hallucinatory tokens, which severely limits their effectiveness in mitigating hallucinations and may even lead to the generation of undesired hallucinations. To tackle this issue, we conducted the theoretical analysis to promote the effectiveness of contrast decoding. Building on this insight, we introduce a novel optimization strategy named Hallucination-Induced Optimization (HIO). This strategy seeks to amplify the contrast between hallucinatory and targeted tokens relying on a fine-tuned theoretical preference model (i.e., Contrary Bradley-Terry Model), thereby facilitating efficient contrast decoding to alleviate hallucinations in LVLMs. Extensive experimental research demonstrates that our HIO strategy can effectively reduce hallucinations in LVLMs, outperforming state-of-the-art methods across various benchmarks.

## Install
1. Clone this repository and navigate to HIO folder
``` 
git clone https://github.com/BT-C/HIO.git
cd HIO
```
2. Install Requirements
```
conda create -n hio python=3.10 -y
conda activate hio
pip install --upgrade pip
pip install -e .
```


## Acknowledgement
   - [LLaVA-1.5](https://github.com/haotian-liu/LLaVA). The LLaVA-v1.5 part of HIO is based on the official LLaVA-1.5 implementation, which is a great open-source work on LVLM.
   - [MiniGPT-4](https://github.com/Vision-CAIR/MiniGPT-4). The MiniGPT-4 part of HIO is based on the official MiniGPT-4 implementation. 

## Paper and Citing HIO

You can find more details in our [paper](https://arxiv.org/pdf/2405.15356).

If you're using HIO in your research or applications, please cite using this BibTeX:

```bibtex
@article{chen2024alleviating,
  title={Alleviating Hallucinations in Large Vision-Language Models through Hallucination-Induced Optimization},
  author={Chen, Beitao and Lyu, Xinyu and Gao, Lianli and Song, Jingkuan and Shen, Heng Tao},
  journal={arXiv preprint arXiv:2405.15356},
  year={2024}
}
```

## Contact us
If you have any questions, comments or suggestions, please do not hesitate to contact us.

## License
[Apache License 2.0](LICENSE.txt)

