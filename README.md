# MTVQA
MTVQA: Benchmarking Multilingual Text-Centric Visual Question Answering

<img src="./images/mtvqa_examples.png" width="95%" height="95%">

> Text-Centric Visual Question Answering (TEC-VQA) in its proper format not only facilitates human-machine interaction in text-centric visual environments but also serves as a de facto gold proxy to evaluate AI models in the domain of text-centric scene understanding. Nonetheless, most existing TEC-VQA benchmarks have focused on high-resource languages like English and Chinese. Despite pioneering works to expand multilingual QA pairs in non-text-centric VQA datasets through translation engines, the translation-based protocol encounters a substantial ''Visual-textual misalignment'' problem when applied to TEC-VQA. Specifically, it prioritizes the text in question-answer pairs while disregarding the visual text present in images. Furthermore, it fails to address complexities related to nuanced meaning, contextual distortion, language bias, and question-type diversity. In this work, we tackle multilingual TEC-VQA by introducing MTVQA, the first benchmark featuring high-quality human expert annotations across 9 diverse languages. Further, by comprehensively evaluating numerous state-of-the-art Multimodal Large Language Models (MLLMs), including GPT-4o, GPT-4V, Claude3, and Gemini, on the MTVQA dataset, it is evident that there is still large room for performance improvement, underscoring the value of the dataset. Additionally, we supply multilingual training data within the MTVQA dataset, demonstrating that straightforward fine-tuning with this data can substantially enhance multilingual TEC-VQA performance. We aspire that MTVQA will offer the research community fresh insights and stimulate further exploration in multilingual visual text comprehension.

**[Project Page [This Page]](https://github.com/bytedance/MTVQA)** | **[Paper](https://arxiv.org/abs/2405.11985)** |**[Dataset and Leaderboard](https://huggingface.co/datasets/ByteDance/MTVQA)**|

# Data
| [RawData] (https://drive.google.com/file/d/1u09EVNVj17ws_AHEB7Y0eZiSPseTJUTx/view?usp=sharing) | [Huggingface Dataset](https://huggingface.co/datasets/ByteDance/MTVQA)

# Evaluation
The test code for evaluating models in the paper can be found in [scripts](./scripts)


# Citation
If you wish to refer to the baseline results published here, please use the following BibTeX entries:
```BibTeX
@misc{tang2024mtvqa,
      title={MTVQA: Benchmarking Multilingual Text-Centric Visual Question Answering}, 
      author={Jingqun Tang and Qi Liu and Yongjie Ye and Jinghui Lu and Shu Wei and Chunhui Lin and Wanqing Li and Mohamad Fitri Faiz Bin Mahmood and Hao Feng and Zhen Zhao and Yanjie Wang and Yuliang Liu and Hao Liu and Xiang Bai and Can Huang},
      year={2024},
      eprint={2405.11985},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```

# Bias, Risks, and Limitations
Your access to and use of this dataset are at your own risk. We do not guarantee the accuracy of this dataset. The dataset is provided “as is” and we make no warranty or representation to you with respect to it and we expressly disclaim, and hereby expressly waive, all warranties, express, implied, statutory or otherwise. This includes, without limitation, warranties of quality, performance, merchantability or fitness for a particular purpose, non-infringement, absence of latent or other defects, accuracy, or the presence or absence of errors, whether or not known or discoverable. In no event will we be liable to you on any legal theory (including, without limitation, negligence) or otherwise for any direct, special, indirect, incidental, consequential, punitive, exemplary, or other losses, costs, expenses, or damages arising out of this public license or use of the licensed material. The disclaimer of warranties and limitation of liability provided above shall be interpreted in a manner that, to the extent possible, most closely approximates an absolute disclaimer and waiver of all liability.