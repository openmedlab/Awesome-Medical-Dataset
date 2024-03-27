# Chinese Medical Dialogue Dataset

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/ChineseMedicalDialogueDataset_0.png"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## Dataset Information

The "Chinese medical dialogue data" dataset consists of 792,099 question and answer pairs, covering six major medical specialties including andrology, internal medicine, gynecology and obstetrics, oncology, pediatrics, and surgery. The detailed categorization and rich content of this dataset provide researchers with a valuable resource for deeply exploring Chinese medical dialogue processing technologies, especially in the fields of natural language processing (NLP) and machine learning (ML).

In the construction and application of large models in the medical field, the significance of this dataset is particularly important. It not only helps researchers train more accurate models to understand and generate medically related dialogues but also provides a foundation for developing efficient, intelligent medical consultation and decision-support systems, greatly advancing the application and development of artificial intelligence technologies in the healthcare sector.

## Dataset Meta Information

| Task Type | Language | Train                                               | Val | Test | File Format | Size |
|-----------|----------|-----------------------------------------------------|-----|------|--------|------|
| QA        | Chinese  | 792099 | -   | -    | .csv   |      |



## Dataset Information Statistics

| file                                 | QA pairs |
|--------------------------------------|-----------------------|
| Andriatria_男科                        | 94596                   |
| IM_内科 (Internal Medicine)            | 220606                  |
| OAGD_妇产科 (Obstetrics and Gynecology) | 183751              |
| Oncology_肿瘤科                         | 75553             |
| Pediatric_儿科                         | 101602             |
| Surgical_外科                          | 115991             |

## Dataset Example


``` 
    {
        "instruction": "现在你是一个神经脑外科医生，请根据患者的问题给出建议：",
        "input": "癫痫病能吃德巴金吗，错觉，有时候感觉看到的和听到的不太一样。",
        "output": "巴金是广谱抗病药物，主要作用于中枢神经系统，对动物的药理研究发现德巴金对各种癫痫的实验模型（全身性和部分性）均有抗惊厥作用，对人的各种类型癫痫发作有抑制作用，作用机理可能与增加γ-氨基丁酸的浓度有关。 主要是治癫痫药物。建议在医生的知道下，用药，祝您身体早日康复。"
    },
    {
        "instruction": "现在你是一个生殖医学科医生，请根据患者的问题给出建议：",
        "input": "男性输精管堵塞的症状会出现什么，男性输精管堵塞的症状会出现什么？输精管堵塞的症状会有哪些？",
        "output": "输精管堵塞的症状一\n输精管道的先天性梗阻：先天性输精管缺如或闭塞、先天性附睾发育不良、附睾与睾丸不连接、先天性精囊缺如或射精管缺如。\n输精管堵塞的症状二\n输精管道的感染：这一输精管堵塞的症状有结核、淋病及血丝虫病，当结核杆菌侵及输精管壁，使输精管壁增厚，输精管变硬变粗，呈串珠状，病变可沿输精管蔓延到附睾尾，然后波及整个附睾和睾丸。球菌感染主要破坏附睾尾部，很少侵及附睾头，输精管也常常受累。丝虫病感染侵及输精管、附睾时，同样可造成其阻塞而不通。当感染侵及前列腺、精囊时，输精管道梗阻症状可表现"
    },

```

## File Structure

The structure of the dataset consists of six folders corresponding to six different medical departments: Andriatria_男科 (Urology), IM_内科 (Internal Medicine), OAGD_妇产科 (Gynecology and Obstetrics), Oncology_肿瘤科 (Oncology), Pediatric_儿科 (Pediatrics), and Surgical_外科 (Surgery). Each folder contains one CSV file with the medical dialogue data for that particular department.

``` 
.
|
├── Andriatria_男科
├── IM_内科
├── OAGD_妇产科 
├── Oncology_肿瘤科
├── Pediatric_儿科
└── Surgical_外科
```

## Authors and Institutions

The dataset is provided by Toyhom, and it is available on GitHub at the repository "Toyhom/Chinese-medical-dialogue-data," which hosts the Chinese medical dialogue data set.

## Source Information

Official Website: https://tianchi.aliyun.com/dataset/90163

Download Link: https://tianchi.aliyun.com/dataset/90163

Article Address: -

Publication Date: 2021.2

## Citation

``` 
TBD
```

Original introduction article is [here](https://zhuanlan.zhihu.com/p/684811168).