# MedDialog-CN

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MedDialog-CN_0.png"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## Dataset Information

MedDialog-CN is a large-scale dataset specifically designed for research on Chinese medical dialogues, containing more than 1.1 million dialogues and 4 million utterances. These original dialogues are sourced from Haodaoctor Online (http://haodf.com). All data copyrights are owned by Haodaoctor Online. This dataset encompasses a wide range of topics from common disease consultations to professional medical advice, aimed at supporting and promoting the development of medical dialogue systems. These systems are expected to improve the accessibility and quality of medical services by providing automated health consultations and support.

The value of the MedDialog-CN dataset lies in providing a precious resource for researchers in the fields of artificial intelligence and machine learning, enabling them to develop and test advanced natural language processing algorithms. These algorithms aim to understand and generate human-like medical dialogues, thus providing patients with accurate and timely medical information, helping to alleviate doctors' workload, and improving the overall efficiency of the medical system.

## Dataset Meta Information

| Task Type | Language | Train | Val | Test | File Format | Size |
|-----------|----------|-------|-----|------|-------------|------|
| QA        | Chinese  | 1.1M  | -   | -    | .txt        | 6.64G |


## Dataset Information Statistics

These consultations cover 29 broad professional fields, including internal medicine, pediatrics, dentistry, etc., as well as 172 sub-specialties, including cardiology, neurology, gastroenterology, urology, and more. The consultations took place between 2010 and 2020.

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MedDialog-CN_1.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## Dataset Example

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MedDialog-CN_2.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em>An example consultation includes (1) the patient's description of their condition and medical history, (2) the dialogue between the doctor and patient, and (3) the diagnosis and treatment recommendations provided by the doctor.</em></p>


## File Structure

The dataset is divided into 11 text files named after the years, each representing the data crawled from the http://haodf.com website for that particular year.

``` 
.
|
├── 2010.txt
├── 2011.txt
├── ...
└── 2020.txt
```

## Authors and Institutions

Xuehai He, Shu Chen, Zeqian Ju, Xiangyu Dong, Hongchao Fang, Sicheng

Wang, Yue Yang, Jiaqi Zeng, Ruisi Zhang, Ruoyu Zhang, Meng Zhou, Penghui

Zhu, Pengtao Xie (University of California San Diego)


## Source Information

Official Website: https://github.com/UCSD-AI4H/Medical-Dialogue-System

Download Link: https://drive.google.com/drive/folders/1r09_i8nJ9c1nliXVGXwSqRYqklcHd9e2

Article Address: https://arxiv.org/pdf/2004.03329v2.pdf

Publication Date: 2020.7

## Citation

``` 
@article{chen2020meddiag,
  title={MedDialog: a large-scale medical dialogue dataset},
  author={Chen, Shu and Ju, Zeqian and Dong, Xiangyu and Fang, Hongchao and Wang, Sicheng and Yang, Yue and Zeng, Jiaqi and Zhang, Ruisi and Zhang, Ruoyu and Zhou, Meng and Zhu, Penghui and Xie, Pengtao},
  journal={arXiv preprint arXiv:2004.03329}, 
  year={2020}
}
```

Original introduction article is [here](https://zhuanlan.zhihu.com/p/684788517).