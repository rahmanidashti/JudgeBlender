# JudgeBlender
JudgeBlender: Ensembling Judgments for Automatic Relevance Assessment

> <font color="red">This repo is updating, more codes and data will be available soon!</font>

<div align="center">

  [![arxiv-link](https://img.shields.io/badge/Paper-PDF-red?style=flat&logo=arXiv&logoColor=red)](https://arxiv.org/abs/2412.13268)
  [![made-with-pytorch](https://img.shields.io/badge/Made%20with-PyTorch-brightgreen)](https://pytorch.org/)
  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
</div>

## Abstract
The effective training and evaluation of retrieval systems require a substantial amount of relevance judgments, which are traditionally collected from human assessors – a process that is both costly and time-consuming. Large Language Models (LLMs) have shown promise in generating relevance labels for search tasks, offering a potential alternative to manual assessments. Current approaches often rely on a single LLM, such as GPT-4, which, despite being effective, are expensive and prone to intra-model biases that can favour systems leveraging similar models. In this work, we introduce JudgeBlender, a framework that employs smaller, open-source models to provide relevance judgments by combining evaluations across multiple LLMs (LLMBlender) or multiple prompts (PromptBlender). By leveraging the LLMJudge benchmark [18], we compare JudgeBlender with state-of-the-art methods and the top performers in the LLMJudge challenge. Our results show that JudgeBlender achieves competitive performance, demonstrating that very large models are often unnecessary for reliable relevance assessments.

## Methods

### PromptBlender
<p align="center">
  <img src="figs/promptblender.png" width="500">
</p>

### LLMBlender
<p align="center">
  <img src="figs/llmblender.png" width="500">
</p>
<br />

## Baselines
The baseline models jusgments and prompts are available at [https://llm4eval.github.io/LLM-as-a-rel/](https://llm4eval.github.io/LLM-as-a-rel/)

## Results
<p align="center">
  <img src="figs/results.png" width="600">
</p>

## Cite
```
@article{rahmani2024judgeblender,
  title={JudgeBlender: Ensembling Judgments for Automatic Relevance Assessment},
  author={Rahmani, Hossein A and Yilmaz, Emine and Craswell, Nick and Mitra, Bhaskar},
  journal={arXiv preprint arXiv:2412.13268},
  year={2024}
}
```

## Acknowledgments
This research is supported by the Engineering and Physical Sciences Research Council [EP/S021566/1] and the EPSRC Fellowship titled "Task Based Information Retrieval" [EP/P024289/1].
