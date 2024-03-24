# MedQA

## Dataset Information

MedQA is a medical text question and answer dataset in a multiple-choice format, with questions drawn from the medical licensing examinations in the United States, mainland China, and Taiwan. These examinations are designed to assess the professional knowledge and clinical decision-making abilities of physicians. The content of the questions is diverse and answering them typically requires a deep understanding of related medical concepts. The dataset contains a total of 61,097 questions, with 12,723 in English, 34,251 in Simplified Chinese, and 14,123 in Traditional Chinese. The official website from which the original data was collected is indicated in the figure below. During the data cleaning phase, duplicate questions and superfluous incorrect options were removed. The dataset is provided in both the original version and a tidied version with four options. A collection of reference books that can provide answers to these questions is also compiled to enable users to make the best use of this dataset.

| Datasets | Websites                                   |
|----------|--------------------------------------------|
| USMLE    | https://step1.medbullets.com               |
|          | https://www.amboss.com/us/usmle            |
|          | https://www.lecturio.com/usmle-step-1      |
| MCML     | http://www.offcn.com/yixue/linchuang       |
| TWML     | https://wwwq.moex.gov.tw/exam/wFrmExamQandASearch.aspx |


## Dataset Meta Information

| Task Type | Language       | Train | Val | Test | File Format | Size |
|-----------|----------------|-------|-----|------|---------|------|
| QA        | Simplified Chinese, Traditional Chinese, English | English 10178, Simplified Chinese 27400, Traditional Chinese 11298   | English 1272, Simplified Chinese 3425, Traditional Chinese 1412 | English 1273, Simplified Chinese 3426, Traditional Chinese 1413  | .json   | 373MB |



## Dataset Information Statistics

The division of the data set, the length statistics of questions and answers are shown in the figure below.

| Metric                         | USMLE        | MCML         | TWML          |
|--------------------------------|--------------|--------------|---------------|
| # of options per question      | 4            | 4            | 4             |
| Avg./Max. option len.          | 3.5 / 45     | 7.3 / 100    | 20.6 / 210    |
| Avg./Max. question len.        | 116.6 / 530  | 45.7 / 333   | 61.0 / 1950   |
| vocab/character size           | 63317        | 3263         | 3588          |
| **# of questions**             |              |              |               |
| Train                          | 10178        | 27400        | 11298         |
| Development                    | 1272         | 3425         | 1412          |
| Test                           | 1273         | 3426         | 1413          |
| All                            | 12723        | 34251        | 14123         |

Table 3: Overall statistics of MedQA. Question/option length and vocabulary/character size are calculated in tokens for English and in characters for Chinese. Vocabulary/character size is measured on the combination of questions and options. “Avg./Max. option len.” represents “Average/Maximum option length”.

The distribution proportion of correct options is shown in the figure below

| Options | USMLE | MCMLE | TWMLE |
|---------|-------|-------|-------|
| A       | 22.5  | 25.9  | 20.3  |
| B       | 27.1  | 24.8  | 25.8  |
| C       | 26.1  | 27.7  | 29.0  |
| D       | 24.3  | 21.5  | 24.9  |

Table A.12: Percentages of each option as the correct answer for the development sets.

## Dataset Example

- USMLE 

```
{"question": "A 23-year-old pregnant woman at 22 weeks gestation presents with burning upon urination. She states it started 1 day ago and has been worsening despite drinking more water and taking cranberry extract. She otherwise feels well and is followed by a doctor for her pregnancy. Her temperature is 97.7°F (36.5°C), blood pressure is 122/77 mmHg, pulse is 80/min, respirations are 19/min, and oxygen saturation is 98% on room air. Physical exam is notable for an absence of costovertebral angle tenderness and a gravid uterus. Which of the following is the best treatment for this patient?", "answer": "Nitrofurantoin", "options": {"A": "Ampicillin", "B": "Ceftriaxone", "C": "Ciprofloxacin", "D": "Doxycycline", "E": "Nitrofurantoin"}, "meta_info": "step2&3", "answer_idx": "E"}
```

- MCMLE

``` 
{"question": "卧位腰椎穿刺，脑脊液压力正常值是（　　）。", "options": {"A": "190～220mmH2O（1.86～2.16kPa）", "B": "80～180mmH2O（0.78～1.76kPa）", "C": "50～70mmH2O（0.49～0.69kPa）", "D": "230～250mmH2O（2.25～2.45kPa）", "E": "260～280mmH2O（2.55～2.74kPa）"}, "answer": "80～180mmH2O（0.78～1.76kPa）", "meta_info": "第三部分　精神神经系统疾病", "answer_idx": "B"}
```

- TWMLE

``` 
{"question": "下列何者不是病人長期臥床不動（immobilization）之後的生理機能反應？", "options": {"A": "肌肉萎縮", "B": "肌力減退", "C": "韌帶鬆弛，延展性增加", "D": "動作協調性變差"}, "answer": "韌帶鬆弛，延展性增加", "meta_info": "taiwanese_test_Q", "answer_idx": "C"} 
```

## File Structure

The MedQA dataset is divided into two parts: questions and textbooks. The question part is further subdivided by region (Mainland, Taiwan, US) and stored in the corresponding folders. All question files are in jsonl format, with each line representing a data sample in dictionary format. The "XX_qbank.jsonl" file contains all data samples and also provides official random assignments of the training set, development set, and test set. Files located in the "metamap" folder are phrases related to medicine extracted using the Metamap tool. The textbook part provides versions in two languages: English and Simplified Chinese. For Simplified Chinese, two types of sentence segmentation are provided: one segmented by sentences (zh_sentence) and the other segmented by paragraphs (zh_paragraph).

``` 
MedQA
├── data_clean
│   ├── questions
│   │   ├── Mainland
│   │   │   ├── 4_options
│   │   │   │   ├── chinese_qbank.jsonl
│   │   │   │   ├── dev.jsonl
│   │   │   │   ├── test.jsonl
│   │   │   │   └── train.jsonl
│   │   ├── Taiwan
│   │   │   ├── metamap
│   │   │   ├── tw_translated_jsonl
│   │   │   │   ├── dev.jsonl
│   │   │   │   ├── taiwanese_qbank.jsonl
│   │   │   │   ├── test.jsonl
│   │   │   │   └── train.jsonl
│   │   └── US
│   │       ├── 4_options
│   │       ├── metamap_extracted_phrases
│   │       │   ├── dev.jsonl
│   │       │   ├── test.jsonl
│   │       │   ├── train.jsonl
│   │       │   └── US_qbank.jsonl
│   └── textbooks
│       ├── en
│       ├── zh_paragraph
│       └── zh_sentence
```

## Authors and Institutions

Di Jin (MIT, Computer Science and Artificial Intelligence Laboratory, USA)

Eileen Pan (MIT, Computer Science and Artificial Intelligence Laboratory, USA)

Nassim Oufattole (MIT, Computer Science and Artificial Intelligence Laboratory, USA)

Wei-Hung Weng (MIT, Computer Science and Artificial Intelligence Laboratory, USA)

Hanyi Fang (Tongji Medical College, Huazhong University of Science and Technology, China)

Peter Szolovits (MIT, Computer Science and Artificial Intelligence Laboratory, USA)


## Source Information

Official Website: https://github.com/jind11/MedQA

Download Link: https://drive.google.com/file/d/1ImYUSLk9JbgHXOemfvyiDiirluZHPeQw/view?usp=sharing

Article Address: https://www.mdpi.com/2076-3417/11/14/6421

Publication Date: 2020-09

## Citation

``` 
@article{jin2020disease,
  title={What Disease does this Patient Have? A Large-scale Open Domain Question Answering Dataset from Medical Exams},
  author={Jin, Di and Pan, Eileen and Oufattole, Nassim and Weng, Wei-Hung and Fang, Hanyi and Szolovits, Peter},
  journal={arXiv preprint arXiv:2009.13081},
  year={2020}
}
```

Original introduction article is [here](https://zhuanlan.zhihu.com/p/679590312).