# CMB

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/CMB_0.png"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## Dataset Information

The Comprehensive Medical Benchmark in Chinese (CMB) was launched in 2023 by a research team from The Chinese University of Hong Kong, Shenzhen. CMB aims to provide a standardized evaluation platform for the performance of large language models (LLMs) in the medical field. One of its subsets, CMB-Exam, gathers a large collection of publicly available mock exam questions, course practice questions, and common misconception questions, primarily sourced from the Chinese Medical Question Database. The research team made these materials public after obtaining the official authorization to use the data. Compared to the conventional format of CMB-Exam, another subset, CMB-Clin, is somewhat more interesting. It is based on 74 real cases from textbooks, which are more complex and challenging than mere exam questions and are more akin to the interview scenarios of professional doctors, evaluating the reasoning capability of LLMs.

2023 was a year of rapid development for large model technology, and the field of medical question-answering attracted increasing attention under this momentum. How to properly evaluate the medical question-answering ability of large models is a valuable question. The establishment of CMB not only filled a gap in the field of Chinese medical assessment but also offered a new perspective for the localized evaluation of models by combining traditional Chinese medicine and modern medical knowledge. However, looking back in 2024, it's apparent that the total volume of exam data in vertical fields like medicine is relatively limited. Once the pioneers who are "quicker to the draw" have utilized all the main data, the evaluation of medical QA will need to evolve towards more granular dimensions, such as the fairness or credibility of Med QA LLMs (for example, directions like hallucination recognition). It's anticipated that the new year will bring datasets from these unique perspectives.

## Dataset Meta Information

| Task Type | Language | Train                                               | Val | Test | File Format | Size |
|-----------|----------|-----------------------------------------------------|-----|------|---------|------|
| QA        | Chinese  | 269,359 | 280 | 400+74  | .json   | 29.3MB |

## Dataset Information Statistics

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/CMB_1.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

CMB-Clin only includes 74 cases, so there isn't much statistical analysis available; the main statistical analysis for CMB-Exam focuses on the types of questions, as shown in the pie chart above. More specific numerical results can be seen in the table below.

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/CMB_2.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

Overall, in the CMB-Exam dataset, the overwhelming majority of questions are physician QA questions, followed by subject exam questions, with test questions and nursing questions being the least common. This distribution is closely related to the popularity and demand for different types of questions in the real world.

## Dataset Example

The data format of CMB-Exam is as follows, similar to the written exam questions of an examination:

``` 
{
    "exam_type": "医师考试",
    "exam_class": "执业医师",
    "exam_subject": "口腔执业医师",
    "question": "患者，男性，11岁。近2个月来时有低热（37～38℃），全身无明显症状。查体无明显阳性体征。X线检查发现右肺中部有一直径约0.8cm类圆形病灶，边缘稍模糊，肺门淋巴结肿大。此男孩可能患",
    "answer": "D",
    "question_type": "单项选择题",
    "option": {
        "A": "小叶型肺炎",
        "B": "浸润性肺结核",
        "C": "继发性肺结核",
        "D": "原发性肺结核",
        "E": "粟粒型肺结核"
    }
},
```

The CMB-Clin data is stored in the following JSON format: for each case, there is a title and a detailed description, followed by multiple QA pairs. This is a common format for QA datasets.

``` 
{
    "id": "2",
    "title": "结、直肠与肛管疾病 案例分析-痔",
    "description": "现病史\n（1）病史摘要\n    周XX，男，34岁，2年前无明显诱因反复出现肛门部肿物脱出，可自行回纳，1周前出现大便后点滴样出血，无发热、恶心、呕吐、腹泻。\n（2）主诉\n    反复肛门部肿物脱出2年，便血1周。\n\n体格检查\n结果 T36.8℃，P74次/分，R20次/分，Bp116/70mmHg。\n    自主体位，神志清楚，全身皮肤及巩膜无黄染，全身浅表淋巴结无肿大。两肺呼吸音清晰，未闻及干湿啰音。心率74次/分，律齐，未闻及病理性杂音，腹部平软，肝、脾脏肋下未触及，未触及腹部包块，肠鸣音正常。\n     专科查体：患者左侧卧位，肛周无溃疡、红肿、疤痕等，肛门7点位可见肿物脱出，直肠空虚，直肠光滑，未及肿物，无压痛，指套退出无血染。\n\n辅助检查\n（1）实验室检查\n    血常规 WBC 6.02×109/L，N 70%，RBC 3.15×109/L，Hb 103g/L，肝功能、肾功能均正常。\n（2）心电图\n    窦性心律。\n（3）胸片\n    心肺未见明显异常。\n（4）纤维结肠镜检查\n    所见回肠末端、结直肠粘膜未见异常；痔。",
    "QA_pairs": [
        {
            "question": "分析本例病人的病史、体格检查和辅助检查。",
            "answer": "（1）病史分析：该病例病史比较简单，肛门部肿物脱出，伴有大便后点滴样出血，需要行进一步的辅助检查以明确诊断。进一步检查主要是针对是否存在远端肠道疾病，要考虑到肠道肿瘤、息肉以及直肠脱垂等。\n    本病例特点为：①反复肛门部肿物脱出；②便后点滴样出血。\n   （2）体格检查分析：肛门7点位可见肿物脱出，直肠空虚，直肠光滑，未及肿物，无压痛，指套退出无血染，可初步排除直肠脱垂、直肠肿瘤、息肉等病史。\n   （3）辅助检查分析：本例病人实验室检查中主要是血常规有轻度贫血的表现，提示病人可能有一个慢性失血的过程。"
        },
        {
            "question": "简述本例病人的诊断及诊断依据，鉴别诊断要点。",
            "answer": "（1）诊断：混合痔\n   （2）诊断依据：①反复肛门部肿物脱出2年，便血1周。②体格检查发现肛门可见肛门7点位可见肿物脱出。③实验室检查：红细胞计数及血红蛋白水平下降。④纤维结肠镜检查：远端肠道未见异常。\n   （3）鉴别诊断：①结直肠肿瘤：肠镜未见异常，可排除。②直肠脱垂：指检直肠空虚，肠镜未见异常。"
        },
        {
            "question": "简述本例病人的治疗原则。",
            "answer": "本例患者患者症状明显，影响生活质量，考虑行手术治疗，查体可见痔疮以单个痔核为主，考虑行混合痔外剥内扎术。术后予软化大便等对症处理。"
        }
    ]
},
```

## File Structure

The dataset file structure is as follows: as a small-scale simple test set, CMB-Clin uses a single JSON file to save all data.

``` 
CMB-Clin
|———— CMB-Clin-qa.json
```

## Authors and Institutions

Xidong Wang (The Chinese University of Hong Kong)
Guiming Hardy Chen (The Chinese University of Hong Kong)
Dingjie Song (The Chinese University of Hong Kong)
Zhiyi Zhang (The Chinese University of Hong Kong)
Zhihong Chen (The Chinese University of Hong Kong)
Qingying Xiao (The Chinese University of Hong Kong)
Feng Jiang (The Chinese University of Hong Kong)
Jianquan Li (The Chinese University of Hong Kong)
Xiang Wan (The Chinese University of Hong Kong)
Benyou Wang (The Chinese University of Hong Kong)
Haizhou Li (The Chinese University of Hong Kong)

## Source Information

Official Website: https://github.com/FreedomIntelligence/CMB/tree/main

Download Link: https://github.com/FreedomIntelligence/CMB/blob/main/data/CMB.zip

Article Address: https://arxiv.org/abs/2308.08833

Publication Date: 2023-08

## Citation

``` 
@article{wang2023cmb,
  title={CMB: A Comprehensive Medical Benchmark in Chinese},
  author={Wang, Xidong and Chen, Guiming Hardy and Song, Dingjie and Zhang, Zhiyi and Chen, Zhihong and Xiao, Qingying and Jiang, Feng and Li, Jianquan and Wan, Xiang and Wang, Benyou and others},
  journal={arXiv preprint arXiv:2308.08833},
  year={2023}
}
```

Original introduction article is [here](https://zhuanlan.zhihu.com/p/685444407).