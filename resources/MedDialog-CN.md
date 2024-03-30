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

| Dataset                         | #dialogs | #diseases |
|---------------------------------|----------|------------|
| Muzhi (Wei et al., 2018)        | 710      | 4          |
| Dxy (Xu et al., 2019)           | 527      | 5          |
| COVID-EN (Yang et al., 2020)    | 603      | 1          |
| COVID-CN (Yang et al., 2020)    | 1,088    | 1          |
| MedDialog-EN                    | 257,454  | 96         |
| MedDialog-CN                    | 3,407,494| 172        |

Table 1: Comparison with other datasets.
## Dataset Example

An example consultation includes (1) the patient's description of their condition and medical history, (2) the dialogue between the doctor and patient, and (3) the diagnosis and treatment recommendations provided by the doctor.

``` 
### Description of medical conditions and history

疾病：宝宝眼睛红红的，严重时稍微溃烂。
(Disease: The baby’s eyes are red and slightly ulcerated when becoming severe.)

病情描述：宝宝眼睛红红的、痒痒的，用手揉，严重时。用了 burt's bee救急膏后过去又反复出来了
(Description of medical condition: The baby's eyes are red and itchy, scratched with hand, and slightly ulcerated when becoming severe. After using Burt's bee Res-Q ointment, it disappeared quickly but came out after two days.)

需要医生帮助的部分：宝宝眼睛红是怎么回事？
(Help needed: What's wrong with baby's red eyes?)

持续多久：一个月内
(Hong long the condition has been: Less than one month)

过敏史：无
(Allergies: No)

既往病史：无
(Past medical history: No)

### Dialogue

医生：感谢您的信任，病情描述我已详细阅读。根据现有的病情，诊断：睑板腺炎。图片不是很清晰。经常挠吗？
(Doctor: Thank you for your trust. I have read the medical information in detail. Based on the existing information, the diagnosis is blepharitis. The picture is not very clear. Scratch it often, right?)

患者：出生到现在都只喝一点奶，嘴巴老是干干的，也不像别的宝宝流口水
(Patient: Drinks little amount of milk since birth, and the baby’s lips are always dry, and not drooling like other babies.)

医生：眼部局部有关节炎
(Doctor: Eyes have local arthritis.)

患者：是的
(Patient: Yes)

医生：给宝宝用妥布霉素和地塞米松眼药膏一天两次
(Doctor: Use Tobramycin and Dexamethasone eye ointment twice a day)

患者：这个怎么回事
(Patient: What's going on?)

医生：考虑睑板腺炎或者睑炎
(Doctor: Consider blepharitis or blepharitis)

患者：严重吗
(Patient: is it severe?)

医生：目前不，给点药物先用几天看看
(Doctor: At present, it is not severe. Try to take the medications for a few days first.)

患者：哦
(Patient: OK)

医生：治疗有什么效果告诉我
(Doctor: Let me know how it works.)

### Diagnosis and suggestions

病情摘要及初步印象：睑板腺炎
(Summary of the condition and initial impressions: Blepharitis)

总结建议：局部炎症。给宝宝用妥布霉素和地塞米松眼药膏一天两次，观察疗效情况。必要时去医院就诊。
(Summary of recommendations: For local inflammation, use Tobramycin and Dexamethasone eye ointment eye ointment twice a day, monitor the recovery, and go to the hospital if necessary.)
```

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