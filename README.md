# MTVQA
MTVQA: Benchmarking Multilingual Text-Centric Visual Question Answering


<img src="./images/mtvqa_examples.png" width="95%" height="95%">

> Text-Centric Visual Question Answering (TEC-VQA) in its proper format not only facilitates human-machine interaction in text-centric visual environments but also serves as a de facto gold proxy to evaluate AI models in the domain of text-centric scene understanding. Nonetheless, most existing TEC-VQA benchmarks have focused on high-resource languages like English and Chinese. Despite pioneering works to expand multilingual QA pairs in non-text-centric VQA datasets through translation engines, the translation-based protocol encounters a substantial ''Visual-textual misalignment'' problem when applied to TEC-VQA. Specifically, it prioritizes the text in question-answer pairs while disregarding the visual text present in images. Furthermore, it fails to address complexities related to nuanced meaning, contextual distortion, language bias, and question-type diversity. In this work, we tackle multilingual TEC-VQA by introducing MTVQA, the first benchmark featuring high-quality human expert annotations across 9 diverse languages. Further, by comprehensively evaluating numerous state-of-the-art Multimodal Large Language Models (MLLMs), including GPT-4o, GPT-4V, Claude3, and Gemini, on the MTVQA dataset, it is evident that there is still large room for performance improvement, underscoring the value of the dataset. Additionally, we supply multilingual training data within the MTVQA dataset, demonstrating that straightforward fine-tuning with this data can substantially enhance multilingual TEC-VQA performance. We aspire that MTVQA will offer the research community fresh insights and stimulate further exploration in multilingual visual text comprehension.

|**[🍎 Project Page](https://bytedance.github.io/MTVQA/)** | **[📖 Paper](https://arxiv.org/abs/2405.11985)** |**[📊 Dataset](https://huggingface.co/datasets/ByteDance/MTVQA)** | **[🏆 Leaderboard](https://github.com/bytedance/MTVQA?tab=readme-ov-file#-leaderboard)** 

## 🔥 News
* **`2024.09.04`** 🌟 InternVL2 tests its performance on MTVQA, InternVL2 76B model outperforms GPT-4V, thanks to the [InternVL2](https://internvl.readthedocs.io/en/latest/internvl2.0/evaluation.html#mtvqa) team. 
* **`2024.08.30`** 🌟 Qwen2VL 72B is released, outperforming GPT-4o and achieving the best performance overall, congratulations!
* **`2024.07.23`** 🌟 MTVQA is now supported in [VLMEvalKit](https://github.com/open-compass/VLMEvalKit).
* **`2024.07.23`** 🌟 MTVQA is now supported in [OpenCompass](https://opencompass.org.cn/home).
* **`2024.06.04`** 🌟 We are excited to launch MTVQA, the first multilingual visual text comprehension evaluation benchmark for MLLMs! MTVQA includes **9** widely-used but low-resource languages, i.t., AR, DE, FR, IT, JA, KO, RU, TH, and VI.
* **`2024.06.04`** 🌟 GPT-4o achieves the best performance overall, MiniCPM-V2.5 achieves the best performance among open-source models!

## 👀 Data
| [RawData (Google Drive)](https://drive.google.com/file/d/1u09EVNVj17ws_AHEB7Y0eZiSPseTJUTx/view?usp=sharing) | [Huggingface Dataset](https://huggingface.co/datasets/ByteDance/MTVQA)


## 🔮 Evaluation
The test code for evaluating models in the paper can be found in [scripts](./scripts).

If you want to add your results to the MTVQA leaderboard, feel free to email us directly at tangjingqun@bytedance.com , haoliu.0128@bytedance.com or can.huang@bytedance.com.

## 🏆 LeaderBoard

<table style="width:75%;">
    <tr>
        <th>Models</th>
        <td><b>Open-Source</b></td>
        <td><b>AR</b></td>
        <td><b><b>DE</b></td>
        <td><b>FR</b></td>
        <td><b>IT</b></td>
        <td><b>JA</b></td>
        <td><b>KO</b></td>
        <td><b>RU</b></td>
        <td><b>TH</b></td>
        <td><b>VI</b></td>
        <td><b>Average</b> </td>
    </tr>
    <tr>
        <th align="left"><font color=darkred>Qwen2-VL 72B🥇</font></th>
        <td align="middle">✘</td>
        <td>20.7 </td>
        <td>36.5 </td>
        <td>44.1 </td>
        <td>42.8 </td>
        <td>21.6 </td>
        <td>37.4 </td>
        <td>15.6 </td>
        <td>17.7 </td>
        <td>41.6 </td>
        <td><font color=red><b>30.9</b></font></td>
    </tr>
    <tr>
        <th align="left"><font color=darkred>GPT-4o 🥈 </font></th>
        <td align="middle">✘</td>
        <td>20.2 </td>
        <td>34.2 </td>
        <td>41.2 </td>
        <td>32.7 </td>
        <td>20.0 </td>
        <td>33.9 </td>
        <td>11.5 </td>
        <td>22.5 </td>
        <td>34.2 </td>
        <td><font color=red><b>27.8</b></font></td>
    </tr>
    <tr>
        <th align="left"><font color=darkred>Claude3 Opus 🥉 </font></th>
        <td align="middle">✘</td>
        <td>15.1 </td>
        <td>33.4 </td>
        <td>40.6 </td>
        <td>34.4 </td>
        <td>19.4 </td>
        <td>27.2 </td>
        <td>13.0 </td>
        <td>19.5 </td>
        <td>29.1 </td>
        <td><font color=red> <b> 25.7 </b> </font> </td>
    </tr>
    <tr>
        <th align="left"><font color=darkred>Qwen2-VL 7B </font></th>
        <td align="middle"> ✅ </td>
        <td>15.5 </td>
        <td>32.1 </td>
        <td>41.6 </td>
        <td>38.9 </td>
        <td>17.8 </td>
        <td>30.6 </td>
        <td>13.0 </td>
        <td>10.8 </td>
        <td>30.0 </td>
        <td><font color=red>25.6</font></td>
    </tr>
    <tr>
        <th align="left"><font color=darkred>Gemini Ultra </font></th>
        <td align="middle">✘</td>
        <td>14.7 </td>
        <td>32.3 </td>
        <td>40.0 </td>
        <td>31.8 </td>
        <td>12.3 </td>
        <td>17.2 </td>
        <td>11.8 </td>
        <td>20.3 </td>
        <td>28.6 </td>
        <td><font color=red>23.2</font></td>
    </tr>
     <tr>
        <th align="left">InternVL2 76B</th>
        <td align="middle"> ✅ </td>
        <td>9.5 </td>
        <td>31.3 </td>
        <td>35.7 </td>
        <td>35.2 </td>
        <td>11.1 </td>
        <td>14.3 </td>
        <td>11.9 </td>
        <td>10.0 </td>
        <td>26.9 </td>
        <td>22.0 </td>
    </tr>
    <tr>
        <th align="left">GPT-4V</th>
        <td align="middle">✘</td>
        <td>11.5 </td>
        <td>31.5 </td>
        <td>40.4 </td>
        <td>32.3 </td>
        <td>11.5 </td>
        <td>16.7 </td>
        <td>10.3 </td>
        <td>15.0 </td>
        <td>28.9 </td>
        <td>22.0  </td>
    </tr>
    <tr>
        <th align="left">QwenVL Max</th>
        <td align="middle">✘</td>
        <td>7.7 </td>
        <td>31.4 </td>
        <td>37.6 </td>
        <td>30.2 </td>
        <td>18.6 </td>
        <td>25.4 </td>
        <td>10.4 </td>
        <td>4.8 </td>
        <td>23.5 </td>
        <td>21.1  </td>
    </tr>
    <tr>
        <th align="left">Claude3 Sonnet</th>
        <td align="middle">✘</td>
        <td>10.5 </td>
        <td>28.9 </td>
        <td>35.6 </td>
        <td>31.8 </td>
        <td>13.9 </td>
        <td>22.2 </td>
        <td>11.0 </td>
        <td>15.2 </td>
        <td>20.8 </td>
        <td>21.1  </td>
    </tr>
    <tr>
        <th align="left">QwenVL Plus</th>
        <td align="middle">✘</td>
        <td>4.8 </td>
        <td>28.8 </td>
        <td>33.7 </td>
        <td>27.1 </td>
        <td>12.8 </td>
        <td>19.9 </td>
        <td>9.4 </td>
        <td>5.6 </td>
        <td>18.1 </td>
        <td>17.8  </td>
    </tr>
    <tr>
        <th align="left"><font color=blue>MiniCPM-V2.5</font></th>
        <td align="middle">✅</td>
        <td>6.1 </td>
        <td>29.6 </td>
        <td>35.7 </td>
        <td>26.0 </td>
        <td>12.1 </td>
        <td>13.1 </td>
        <td>5.7 </td>
        <td>12.6 </td>
        <td>15.3 </td>
        <td><font color=blue><b>17.3 </b></font></td>
    </tr>
    <tr>
        <th align="left">InternVL-V1.5</th>
        <td align="middle">✅</td>
        <td>3.4 </td>
        <td>27.1 </td>
        <td>31.4 </td>
        <td>27.1 </td>
        <td>9.9 </td>
        <td>9.0 </td>
        <td>4.9 </td>
        <td>8.7 </td>
        <td>12.4 </td>
        <td>14.9  </td>
    </tr>
    <tr>
        <th align="left">GLM4V</th>
        <td align="middle">✘</td>
        <td>0.3 </td>
        <td>30.0 </td>
        <td>34.1 </td>
        <td>30.1 </td>
        <td>3.4 </td>
        <td>5.7 </td>
        <td>3.0 </td>
        <td>3.5 </td>
        <td>12.3 </td>
        <td>13.6  </td>
    </tr>
    <tr>
        <th align="left">TextSquare</th>
        <td align="middle">✅</td>
        <td>3.7 </td>
        <td>27.0 </td>
        <td>30.8 </td>
        <td>26.7 </td>
        <td>3.2 </td>
        <td>7.2 </td>
        <td>6.7 </td>
        <td>5.2 </td>
        <td>12.4 </td>
        <td>13.6  </td>
    </tr>
    <tr>
        <th align="left">Mini-Gemini-HD-34B</th>
        <td align="middle">✅</td>
        <td>2.2 </td>
        <td>25.0 </td>
        <td>29.2 </td>
        <td>25.5 </td>
        <td>6.1 </td>
        <td>8.6 </td>
        <td>4.1 </td>
        <td>4.3 </td>
        <td>11.8 </td>
        <td>13.0  </td>
    </tr>
    <tr>
        <th align="left">InternLM-Xcomposer2-4KHD</th>
        <td align="middle">✅</td>
        <td>2.0 </td>
        <td>20.6 </td>
        <td>23.2 </td>
        <td>21.6 </td>
        <td>5.6 </td>
        <td>7.7 </td>
        <td>4.1 </td>
        <td>6.1 </td>
        <td>10.1 </td>
        <td>11.2  </td>
    </tr>
    <tr>
        <th align="left">Llava-Next-34B</th>
        <td align="middle">✅</td>
        <td>3.3 </td>
        <td>24.0 </td>
        <td>28.0 </td>
        <td>22.3 </td>
        <td>3.6 </td>
        <td>6.1 </td>
        <td>2.6 </td>
        <td>0.4 </td>
        <td>9.8 </td>
        <td>11.1  </td>
    </tr>
    <tr>
        <th align="left">TextMonkey</th>
        <td align="middle">✅</td>
        <td>2.0 </td>
        <td>18.1 </td>
        <td>19.9 </td>
        <td>22.1 </td>
        <td>4.6 </td>
        <td>7.2 </td>
        <td>3.2 </td>
        <td>0.9 </td>
        <td>11.1 </td>
        <td>9.9  </td>
    </tr>
    <tr>
        <th align="left">MiniCPM-V2.0</th>
        <td align="middle">✅</td>
        <td>1.3 </td>
        <td>12.7 </td>
        <td>14.9 </td>
        <td>17.0 </td>
        <td>3.7 </td>
        <td>5.6 </td>
        <td>2.2 </td>
        <td>2.2 </td>
        <td>6.8 </td>
        <td>7.4 </td>
    </tr>
    <tr>
        <th align="left">mPLUG-DocOwl 1.5</th>
        <td align="middle">✅</td>
        <td>1.0 </td>
        <td>13.9 </td>
        <td>14.9 </td>
        <td>18.2 </td>
        <td>2.9 </td>
        <td>5.0 </td>
        <td>2.0 </td>
        <td>0.9 </td>
        <td>6.4 </td>
        <td>7.2  </td>
    </tr>
    <tr>
        <th align="left">YI-VL-34B</th>
        <td align="middle">✅</td>
        <td>1.7 </td>
        <td>13.5 </td>
        <td>15.7 </td>
        <td>12.1 </td>
        <td>4.8 </td>
        <td>5.2 </td>
        <td>0.8 </td>
        <td>3.5 </td>
        <td>4.1 </td>
        <td>6.8  </td>
    </tr>
    <tr>
        <th align="left">DeepSeek-VL</th>
        <td align="middle">✅</td>
        <td>0.6 </td>
        <td>14.2 </td>
        <td>15.3 </td>
        <td>15.2 </td>
        <td>2.9 </td>
        <td>3.8 </td>
        <td>1.6 </td>
        <td>0.9 </td>
        <td>5.2 </td>
        <td>6.6 </td>
    </tr>
</table>


## :black_nib: Citation
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

## Licence

[CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/)


## Bias, Risks, and Limitations
Your access to and use of this dataset are at your own risk. We do not guarantee the accuracy of this dataset. The dataset is provided “as is” and we make no warranty or representation to you with respect to it and we expressly disclaim, and hereby expressly waive, all warranties, express, implied, statutory or otherwise. This includes, without limitation, warranties of quality, performance, merchantability or fitness for a particular purpose, non-infringement, absence of latent or other defects, accuracy, or the presence or absence of errors, whether or not known or discoverable. In no event will we be liable to you on any legal theory (including, without limitation, negligence) or otherwise for any direct, special, indirect, incidental, consequential, punitive, exemplary, or other losses, costs, expenses, or damages arising out of this public license or use of the licensed material. The disclaimer of warranties and limitation of liability provided above shall be interpreted in a manner that, to the extent possible, most closely approximates an absolute disclaimer and waiver of all liability.
