# MMMU Health&Medicine

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_0.png"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## Dataset Information

MMMU (Massive Multi-discipline Multimodal Understanding and Reasoning Benchmark) is a benchmark designed to assess the performance of multimodal models on large-scale multidisciplinary tasks. MMMU includes 11.5K carefully collected multimodal questions from college exams, quizzes, and textbooks, covering **six core disciplines**: Art & Design, Business, Science, **Health & Medicine**, Humanities & Social Science, and Tech & Engineering. These questions span 30 disciplines and 183 subfields, including 30 different types of images. As of March 14, 2024, the top 3 models on the MMMU validation set achieved accuracies of only 59.4% (Gemini Ultra), 59.4% (Claude 3 Opus), and 56.8% (GPT4-V).

This article will focus on the medical-related evaluation questions in MMMU, namely the MMMU Health & Medicine core discipline. The total number of questions in its test set is **1752**, accounting for **17%** of the overall MMMU evaluation questions, which are further subdivided into **five disciplines**: **Basic Medical Science**, **Clinical Medicine**, **Diagnostics and Laboratory Medicine**, **Pharmacy**, and **Public Health**. For further detailed subdivision and quantity of subfields, please refer to the following figure and table. As of March 14, 2024, the top 4 models on the MMMU Health & Medicine validation set achieved accuracies of 67.3% (Gemini Ultra), 64.7% (GPT4-V), 61.1% (Claude 3 Opus), and 58.7% (**InternVL-Chat**).

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_1.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em>Health & Medicine accounts for 17% of the total in MMMU. It is further divided into 5 disciplines, with the number and proportion of questions for each discipline as shown in the graph.</em></p>


<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_2.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em>MMMU Health & Medicine sub-disciplines and sub-field category names.</em></p>


## Dataset Meta Information

Only the questions from the Health & Medicine discipline are counted. The dataset contains 1752 test questions without answers, including 326 in Basic Medical Science, 325 in Clinical Medicine, 162 in Diagnostics and Laboratory Medicine, 430 in Pharmacy, and 509 in Public Health. Each of the 5 disciplines provides 5 questions with answers for few-shot learning, and a total of 150 questions with answers are provided in the validation set.

| Task Type | Language       | Train | Val | Test | File Format | Size  |
|-----------|----------------|-------|-----|------|-------------|-------|
| VQA       | English | 25    | 150 | 1752 | .parquet   | 391MB |

## Dataset Information Statistics

The statistics of the MMMU core are as follows:

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_3.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

The performance comparison of each model on MMMU Health&Medicine is as follows. The performance between random selection, different multimodal models, and different language models was compared.

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_4.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

The comparison between MMMU and other general multi-modal benchmarks is as follows:

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_5.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

MMMU contains 30 different image types. The distribution of different image types is as shown below.

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_6.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## Dataset Example

The following shows the answers to the questions of the 5 subject example cases shown in the paper and the answers to GPT4-V.

### Basic Medical Science

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_7.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em>Basic Medical Sciences, GPT-4V Answer the correct Case.</em></p>

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_8.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em>Basic Medical Sciences, GPT-4V Answer the wrong Case.</em></p>

### Clinical Medicine

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_9.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em>Clinical Medicine, GPT-4V Answer the correct Case.</em></p>

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_10.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em>Clinical Medicine, GPT-4V Answer the correct Case.</em></p>

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_11.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em>Clinical Medicine, GPT-4V Answer the correct Case.</em></p>

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_12.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em>Clinical Medicine, GPT-4V Answer the wrong Case.</em></p>

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_13.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em>Clinical Medicine, GPT-4V Answer the wrong Case.</em></p>

### Diagnostics and Laboratory Medicine

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_14.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em>Diagnostics and Laboratory Medicine, GPT-4V Answer the correct Case.</em></p>

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_15.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em>Diagnostics and Laboratory Medicine, GPT-4V Answer the wrong Case.</em></p>

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_16.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em>Diagnostics and Laboratory Medicine, GPT-4V Answer the wrong Case.</em></p>

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_17.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em>Diagnostics and Laboratory Medicine, GPT-4V Answer the wrong Case.</em></p>

### Pharmacy

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_18.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em>Pharmacy, GPT-4V Answer the correct Case.</em></p>

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_19.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em>Pharmacy, GPT-4V Answer the wrong Case.</em></p>

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_20.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em>Pharmacy, GPT-4V Answer the wrong Case.</em></p>

### Public Health

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_21.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em>Public Health, GPT-4V Answer the correct Case.</em></p>

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_22.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em>Public Health, GPT-4V Answer the wrong Case.</em></p>

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_23.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em>Public Health, GPT-4V Answer the wrong Case.</em></p>


## File Structure

MMMU provides directories for 30 disciplines. After downloading, the data related to the 5 disciplines within Health & Medicine are as follows. Each discipline offers a dev set of 5 questions for few-shot learning, which includes questions and answers, a validation set that contains both questions and answers, and a test set that only provides the questions.

``` 
MMMU
│
├── Basic_Medical_Science
│   ├── dev-00000-of-00001.parquet
│   ├── test-00000-of-00001.parquet
│   └── validation-00000-of-00001.parquet
│
├── Clinical_Medicine
│   ├── dev-00000-of-00001.parquet
│   ├── test-00000-of-00001.parquet
│   └── validation-00000-of-00001.parquet
│
├── Diagnostics_and_Laboratory_Medicine
│   ├── dev-00000-of-00001.parquet
│   ├── test-00000-of-00001.parquet
│   └── validation-00000-of-00001.parquet
│
├── Pharmacy
│   ├── dev-00000-of-00001.parquet
│   ├── test-00000-of-00001.parquet
│   └── validation-00000-of-00001.parquet
│
└── Public_Health
    ├── dev-00000-of-00001.parquet
    ├── test-00000-of-00001.parquet
    └── validation-00000-of-00001.parquet
```

The file visualization is as shown in the following figure. A complete visualization can be viewed at https://huggingface.co/datasets/MMMU/MMMU/viewer. The validation set provides both questions and answers, while the test set only provides the questions.

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_24.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em>Clinical_Medicine/dev-00000-of-00001.parquet</em></p>

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MMMUHealth&Medicine_25.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em>Clinical_Medicine/test-00000-of-00001.parquet</em></p>

## Authors and Institutions

Here only the core contributors are listed. For the full list of authors, refer to the original paper.

Xiang Yue (IN.AI Research)

Yuansheng Ni (University of Waterloo, Canada)

Kai Zhang (The Ohio State University, USA)

Tianyu Zheng (Independent Researcher)

Huan Sun (The Ohio State University, USA)

Yu Su (The Ohio State University, USA)

Wenhu Chen (University of Waterloo, Canada)

## Source Information

Official Website: https://mmmu-benchmark.github.io/

Download Link: https://huggingface.co/datasets/MMMU/MMMU

Article Address: https://arxiv.org/abs/2311.16502

Publication Date: 2023-11

## Citation

``` 
@article{yue2023mmmu,
    title={MMMU: A Massive Multi-discipline Multimodal Understanding and Reasoning Benchmark for Expert AGI},
    author={Xiang Yue and Yuansheng Ni and Kai Zhang and Tianyu Zheng and Ruoqi Liu and Ge Zhang and Samuel Stevens and Dongfu Jiang and Weiming Ren and Yuxuan Sun and Cong Wei and Botao Yu and Ruibin Yuan and Renliang Sun and Ming Yin and Boyuan Zheng and Zhenzhu Yang and Yibo Liu and Wenhao Huang and Huan Sun and Yu Su and Wenhu Chen},
    journal={arXiv preprint arXiv:2311.16502},
    year={2023},
}
```

Original introduction article is [here](https://zhuanlan.zhihu.com/p/686799693).