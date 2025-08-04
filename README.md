
<h1 align="center">
<img src="./docs/images/LogicPro_Logo.png" width="100" alt="LogicPro" />
<br>
LogicPro: Logical Reasoning Enhanced with Program Examples
</h1>

<p align="center">
  <a href="https://arxiv.org/abs/2409.12929"><b>[📑 Paper]</b></a> •
  <a href="https://huggingface.co/datasets/jiangjin/LogicPro"><b>[🤗 HF Dataset]</b></a> •
  <a href="https://github.com/jiangjin1999/LogicPro"><b>[👻 GitHub]</b></a> •
  <a href="https://x.com/JiangJin_PKU/status/1950293851266306207"><b>[🔗 X/Twiiter]</b></a>

</p>

<!-- <p align="center">
Repo for "<a href="https://arxiv.org/abs/2408" target="_blank">LogicPro: Logical Reasoning Enhanced with Program Examples</a>" [arxiv'2024]
</p> -->

<p align="center">
  <img src="./docs/images/LogicPro.png" width="1000">
  <br>
  <em>An overview of LogicPro. Example: Climbing Stairs (LeetCode 70).</em>
</p>

## 🔥 News
- [2025/05/16] 🎉🎉🎉 Our work has been accepted as an ACL 2025 Main Conference paper!
- [2025/02/17] 🔥🔥🔥 LogicPro (500K+) released at [🤗 HuggingFace](https://huggingface.co/datasets/jiangjin/LogicPro)!
- [2024/09/19] LogicPro paper released.

## 💡 Introduction

LogicPro is a data synthesis method that leverages LeetCode-style algorithm **Pro**blems and their corresponding **Pro**gram solutions to generate complex **Logic**al reasoning data in text format. Our approach consists of three key steps:  

1. **Problem Synthesis**: We generate complex reasoning problems based on source algorithm problems and their test cases.  
2. **Answer Generation**: Using standard Python solutions and test cases, we obtain the correct answers and intermediate variable outputs for each problem.  
3. **Reasoning Process Synthesis**: Guided by the intermediate variable outputs, we construct high-quality textual reasoning processes for each problem.  

This method enables us to synthesize reasoning data that is **challenging, scalable, and effective**, while also providing **gold-standard answers** and **high-quality reasoning processes**. With our **540K synthesized dataset**, built from just **2,360 algorithm problems**, LogicPro significantly improves the performance of multiple models on benchmark datasets such as **BBH, LogicBench, DROP, AR-LSAT,** and **GSM8K**, outperforming various existing reasoning datasets.


## 🔗 Related Work  
We would like to recommend some outstanding works that share similar ideas and approaches with ours. Please take a look at the following research:

1. **CodeI/O**: Condensing Reasoning Patterns via Code Input-Output Prediction  
   [https://arxiv.org/abs/2502.07316v2](https://arxiv.org/abs/2502.07316v2)  

2. **SynLogic**: Synthesizing Verifiable Reasoning Data at Scale for Learning Logical Reasoning and Beyond  
   [https://arxiv.org/abs/2505.19641](https://arxiv.org/abs/2505.19641)  

3. **Code2Logic**: Game-Code-Driven Data Synthesis for Enhancing VLMs General Reasoning  
   [https://arxiv.org/abs/2505.13886](https://arxiv.org/abs/2505.13886)  



## ☕️ Citation

If you find this repository helpful, please consider citing our paper:

```
@inproceedings{jiang-etal-2025-logicpro,
    title = "{L}ogic{P}ro: Improving Complex Logical Reasoning via Program-Guided Learning",
    author = "Jiang, Jin  and
      Yan, Yuchen  and
      Liu, Yang  and
      Wang, Jianing  and
      Peng, Shuai  and
      Cai, Xunliang  and
      Cao, Yixin  and
      Zhang, Mengdi  and
      Gao, Liangcai",
    editor = "Che, Wanxiang  and
      Nabende, Joyce  and
      Shutova, Ekaterina  and
      Pilehvar, Mohammad Taher",
    booktitle = "Proceedings of the 63rd Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)",
    month = jul,
    year = "2025",
    address = "Vienna, Austria",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2025.acl-long.1270/",
    pages = "26200--26218",
    ISBN = "979-8-89176-251-0",
    abstract = "In this paper, we propose a new data synthesis method called \textbf{LogicPro}, which leverages LeetCode-style algorithm Problems and their corresponding Program solutions to synthesize Complex Logical Reasoning data in text format. First, we synthesize complex reasoning problems through source algorithm problems and test cases. Then, standard answers and intermediate variable outputs are obtained for each problem based on standard python solutions and test cases. Finally, with the guidance of code intermediate variables, we synthesize the text reasoning process for each reasoning problems. Through this method, we can synthesize data that is difficult, scalable, effective, and comes with golden standard answers and high-quality reasoning processes. As a result, with our 540K synthesized dataset constructed solely from 2,360 algorithm problems, our approach achieves significant improvements in multiple models for the datasets \textit{BBH{\textasciicircum}27}, \textit{LogicBench}, \textit{DROP}, \textit{AR-LSAT}, and \textit{GSM8K}, etc. outperforming a wide range of existing reasoning datasets."
}
```
