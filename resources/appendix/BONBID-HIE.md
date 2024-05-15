# BONBID-HIE

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/BONBID-HIE_0.png"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## Dataset Information

The BONBID-HIE 2023 dataset is specifically designed for lesion segmentation tasks in neonatal hypoxic-ischemic encephalopathy (HIE), featuring various modalities of brain MRI data. This dataset includes a total of 133 cases, divided into 85 for training, 4 for validation, and 44 for testing. The dataset aims to support research on HIE lesion segmentation and to advance technology in this field.

Hypoxic-ischemic encephalopathy (HIE) is a severe form of neonatal brain injury that affects about 200,000 full-term newborns worldwide each year. The brain lesions caused by HIE are typically diffuse and minute, making the segmentation task more complex and challenging compared to diseases with larger and more localized lesions, such as brain tumors. Currently, the segmentation performance for HIE lesions remains limited, with a Dice coefficient of about 0.5, whereas the Dice coefficient for brain tumors typically exceeds 0.8. There is an urgent need to improve the precision of HIE lesion segmentation to better estimate prognosis and enhance diagnosis. The BONBID-HIE lesion segmentation challenge is the first to address this critical medical issue using a publicly available MRI dataset.

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/BONBID-HIE_1.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## Dataset Meta Information

| Dimensions | Modality | Task Type     | Anatomical Structures           | Anatomical Area | Number of Categories | Data Volume | File Format |
|------------|----------|---------------|---------------------------------|-----------------|----------------------|-------------|-------------|
| 3D         | MRI      | Segmentation  | Hypoxic-ischemic Encephalopathy | Brain           | 1                    | 133         | .mha        |


### Resolution Details

| Dataset Statistics | spacing (mm)         | size            |
|--------------------|----------------------|-----------------|
| min                | (0.625, 0.625, 2.0)  | (128, 128, 16)  |
| median             | (1.375, 1.375, 2.2)	 | (160, 160, 43)  |
| max                | (2.0, 2.0, 6.0)      | (256, 256, 64)  |

## Label Information Statistics

Key medical information about mothers at the time of delivery, including the average age of mothers at delivery (Maternal age at delivery), race (Race), method of delivery (Delivery), whether there was antepartum hemorrhage (Antepartum hemorrhage), whether thyroid function was normal (Thyroid dysfunction), whether pre-eclampsia was present (Pre-eclampsia), and whether there was a slowdown in fetal heart rate (Fetal decels).

| Maternal Information             | Details                                                                                                     | N=133 |
|----------------------------------|-------------------------------------------------------------------------------------------------------------|-------|
| Maternal age at delivery (years) |  29.5 ± 6.7                                                                                                 | N=133 |
| Race                             | White (43), Black or African American (7), Hispanic or Latino (15), Multi Race (5), Unknown (57), Other (6) | N=133 |
| Delivery                         | C-section (78), Vaginal (55)                                                                                | N=133 |
| Antepartum hemorrhage            | Yes (29), No (104)                                                                                          | N=133 |
| Thyroid dysfunction              | Yes (5), No (128)                                                                                           | N=133 |
| Pre-eclampsia                    | Yes (9), No (124)                                                                                           | N=133 |
| Fetal decels                     | Yes (72), No (61)                                                                                           | N=133 |
| Shoulder dystocia                | Yes (8), No (125)                                                                                           | N=133 |
| Chorioamnionitis                 | Yes (20), No (108)                                                                                          | N=133 |
| Emergency c-section              | Yes (69), No (58)                                                                                           | N=133 |

Statistical information on the volume of brain lesions:

| Lesion Characterisics(N=133)                | Volume (mm³) | Percentage of Brain Injured |
|---------------------------------------------|--------------|-----------------------------|
| Whole-brain lesion volume – minimum         | 0 mm³        | 0% of the brain injured     |
| Whole-brain lesion volume – 25th percentile | 441.96 mm³  | 0.10% of the brain injured  |
| Whole-brain lesion volume – median          | 2765.63 mm³  | 0.63% of the brain injured  |
| Whole-brain lesion volume – 75th percentile | 24264.27 mm³ | 4.86% of the brain injured  |
| Whole-brain lesion volume – maximum         | 412120.00 mm³| 82.59% of the brain injured |

Numbers of Patients by Percentage of Leisions in the Brain (N=133):

| Range of Brain Injury      | Percentage of Patients | Number of Patients |
|----------------------------|------------------------|--------------------|
| [0%, 1%)                   | 55.64%                 | N=74               |
| [1%, 5%)                   | 19.55%                 | N=26               |
| [5%, 10%)                  | 5.26%                  | N=7                |
| [10%, 20%)                 | 4.51%                  | N=6                |
| [20%, 50%)                 | 8.27%                  | N=11               |
| [50%, 100%]                | 6.77%                  | N=9                |

## Visualization

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/BONBID-HIE_2.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## File Structure

Introduce file structure of original dataset folder.

Take representative MSD dataset for example:

``` 
BONBID-HIE
│
├── 0ADC
│   ├── MGHNICU_001-VISIT_01-ADC.nii.gz
│   ├── MGHNICU_001-VISIT_01-anon.json
│   ├── MGHNICU_002-VISIT_01-ADC.nii.gz
│   ├── MGHNICU_002-VISIT_01-anon.json
│   └── ...
│
├── 1ADC_ss
│   ├── MGHNICU_001-VISIT_01-ADC_ss.nii.gz
│   ├── MGHNICU_002-VISIT_01-ADC_ss.nii.gz
│   └── ...
│
├── 2Z_ADC
│   ├── Zmap_MGHNICU_001-VISIT_01-ADC_smooth2mm_clipped10.nii.gz
│   ├── Zmap_MGHNICU_002-VISIT_01-ADC_smooth2mm_clipped10.nii.gz
│   └── ...
│
├── 3LABEL
│   ├── MGHNICU_001_lesion.nii.gz
│   ├── MGHNICU_002_lesion.nii.gz
│   └── ...
│
├── Clinical Data
│   └── ClinicalData_BONBID2023.xlsx
│
├── Atlases
│   ├── Normal_atlas
│   └── Lesion_atlas
│
├── Readme.txt
│
└── Licence
```

## Authors and Institutions

Rina Bao (Boston Children's Hospital, Harvard Medical School)

Yangming Ou (Boston Children's Hospital, Harvard Medical School)

P. Ellen Grant (Boston Children's Hospital, Harvard Medical School)

## Source Information

Official Website: https://bonbid-hie2023.grand-challenge.org

Download Link: https://zenodo.org/records/8104103

Article Address: https://www.biorxiv.org/content/10.1101/2023.06.30.546841v1

Publication Date: 2023-06

## Citation

``` 
@article{bao2023boston,
  title={BOston Neonatal Brain Injury Dataset for Hypoxic Ischemic Encephalopathy (BONBID-HIE): Part I. MRI and Manual Lesion Annotation},
  author={Bao, Rina and Song, Ya’nan and Bates, Sara V and Weiss, Rebecca J and Foster, Anna N and Cobos, Camilo Jaimes and Sotardi, Susan and Zhang, Yue and Gollub, Randy L and Grant, P Ellen and others},
  journal={bioRxiv},
  year={2023},
  publisher={Cold Spring Harbor Laboratory Preprints}
}
```

Original introduction article is [here](https://zhuanlan.zhihu.com/p/697620565).