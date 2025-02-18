# 🕷️DebugEval 
Official repository for the paper "Enhancing the Code Debugging Ability of LLMs via
Communicative Agent Based Data Refinement".

<p align="center">
    <a href="https://arxiv.org/pdf/2408.05006">📜 Paper</a> •
    <a href="https://huggingface.co/datasets/yangweiqing/DebugEval-Dataset">🤗 Data </a> •
    <a href="https://huggingface.co/yangweiqing">🤖 Model </a>
</p>

## 1. Introduction
This paper presents a benchmark, DebugEval, which is used to evaluate the code debugging ability of LLMs (Large Language Models) and proposals a framework for building training data using multiple agents, MASTER.

### 1.1 Benchmark
#### DebugEval designs four task scenarios: BUG Localization, BUG Identification, Code Repair, and Code Review to comprehensively evaluate the code debugging capability of LLMs.

![image](https://github.com/NEUIR/COAST/blob/main/Figure/benchmark.pdf)
### 1.2 MASTER
#### MASTER is a framework for making use of multiple agents working together to refine training data to improve code debugging capability in LLMs.

![image](https://github.com/NEUIR/COAST/blob/main/Figure/COAST.pdf)
## 2. Installation
You can clone the repository using the following command:

```
git clone DebugEval
cd DebugEval
```

## 3. Inference and Evaluation
Download the dataset we provide.

```
cd src
```
Please refer to `src/README.md` for more details.
## 4. Fine-Tuning
We use DeepSeek-Coder-6.7B-Ins and Llama3-8B-Ins as the base model, and train the models with MASTER framework.

### 4.1 For DeepSeek-Coder-6.7B-Ins
```
cd neural_compiler
```
Please refer to `neural_compiler/README.md` for more details.
### 4.2 For Llama3-8B-Ins
```
cd LLaMA-Factory
```
Please refer to `LLaMA-Factory/README.md` for more details.

We provide the trained NeuDebugger models.

## 5. Result

![image](https://github.com/NEUIR/DebugEval/blob/main/Figure/performance_00.png)
## 6. Citation
Please cite the paper and star the repo if you use DebugEval and find it helpful.

Feel free to contact 2301983@stu.neu.edu.cn or open an issue if you have any questions.
```
@article{DebugEval2024,
      title={Enhancing the Code Debugging Ability of LLMs via Communicative Agent Based Data Refinement}, 
      author={Weiqing Yang, Hanbin Wang, Zhenghao Liu, Xinze Li, Yukun Yan, Shuo Wang, Yu Gu, Minghe Yu, Zhiyuan Liu and Ge Yu},
      year={2024},
}
```
