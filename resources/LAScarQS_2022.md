# LAScarQS 2022
<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/LAScarQS_2022.png"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## Dataset Information

LAScarQS (Left Atrial and Scar Quantification & Segmentation Challenge) 2022 is a dataset specifically for patients with Atrial Fibrillation (AF), featuring late gadolinium enhancement (LGE) MRI, aimed at precise segmentation of the Left Atrium (LA) and Left Atrial Scar (LA Scar) and is part of the MICCAI 2022 challenge. Atrial Fibrillation is the most common cardiac arrhythmia, especially with rapidly increasing incidence in the elderly population. To treat AF, radiofrequency catheter ablation, particularly pulmonary vein isolation techniques, has become a mainstream method. LGE MRI clearly displays atrial scars, and their location and size provide key information for assessing the pathophysiology and progression of AF. The challenge is divided into two tasks: Task 1 aims to segment both LA and LA Scar, with data including 60 training cases and 34 test cases of post-ablation LGE MRI, without public annotations for the test set. Task 2 aims to segment only LA, with data including both pre- and post-ablation LGE MRI, featuring 130 training cases and 64 test cases, with the test set containing data from unknown domains and without public annotations. The dataset comes from data at three centers: the University of Utah, Beth Israel Deaconess Medical Center, and King's College London, each scanned with different equipment and resolutions to ensure model generalizability across different clinical scenarios.

## Dataset Meta Information

| Dimensions | Modality | Task Type | Anatomical Structures          | Anatomical Area | Number of Categories | Data Volume                                                                 | File Format |
|------------|----------|-----------|--------------------------------|-----------------|----------------------|-----------------------------------------------------------------------------|-------------|
| 3D         | LGE MR	       | Segmentation | left atrium, left atrium scar | Heart           | Task 1: 2, Task 2: 1 | Task 1: 60 for training, 34 for test; Task 2: 130 for training, 64 for test | .nii.gz     |

Training set 130 two-dimensional slices: 7040

### Resolution Details

Use task 2 data to count left atrial labels, and use task 1 data to count left atrial scar labels.

| Dataset Statistics | spacing (mm)     | size            |
|--------------------|------------------|-----------------|
| min                | (0.625, 0.625, 1.0)              | (576, 576, 44)     |
| median             | (0.625, 0.625, 2.5)           | (640, 640, 44) |
| max                | (1.0, 1.0, 2.5)              | (640, 640, 88) |

## Label Information Statistics

| Anatomical Structure | Left Atrium | Left Atrial Scar |
|----------------------|---------------|--------------------------|
| Number of Cases      | 130           | 60                       |
| Coverage Percentage  | 100%          | 100%                     |
| Minimum Volume (cm³) | 37            | 0.89                     |
| Median Volume (cm³)  | 113           | 3.18                     |
| Maximum Volume (cm³) | 410           | 8.33                     |


## Visualization

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/LAScarQS_2022.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em> ITK-SNAP Visualization. Red: left atrium scar, green: left atrium.</em></p>

## File Structure

The official file structure is divided into task1 and task2. In task1, `atriumSegImgMO.nii.gz` is the annotation for the left atrium, `enhanced.nii.gz` is the LGE MR image, and `scarSegImgM.nii.gz` is the annotation for the left atrial scar. In contrast, task2 only includes `atriumSegImgMO.nii.gz`, which is the annotation for the left atrium.

``` 
LAScarQS2022
│
├── task1
│   ├── readme.txt
│   └── train_data
│       ├── train_1
│       │   ├── atriumSegImgMO.nii.gz
│       │   ├── enhanced.nii.gz
│       │   └── scarSegImgM.nii.gz
│       ├── ...
│       └── train_60
│
├── task1_val
│
├── task2
│   ├── readme.txt
│   └── train_data
│       ├── train_1
│       │   ├── atriumSegImgMO.nii.gz
│       │   └── enhanced.nii.gz
│       ├── ...
│       └── train_130
│
└── task2_val
```

## Authors and Institutions

Xiahai Zhuang (Fudan University)

Lei Li (University of Oxford, UK)

Sihan Wang (Fudan University)

Fuping Wu (University of Oxford, UK)


## Source Information

Official Website: https://zmiclab.github.io/projects/lascarqs22/

Download Link: https://zmiclab.github.io/projects/lascarqs22/data.html

Article Address: https://www.sciencedirect.com/science/article/pii/S1361841521003480, https://www.sciencedirect.com/science/article/pii/S1361841522000135, https://link.springer.com/chapter/10.1007/978-3-030-87231-1_54

Publication Date: 2022-04

## Citation

``` 
@article{li2022atrialjsqnet,
  title={AtrialJSQnet: A New framework for joint segmentation and quantification of left atrium and scars incorporating spatial and shape information},
  author={Li, Lei and Zimmer, Veronika A and Schnabel, Julia A and Zhuang, Xiahai},
  journal={Medical image analysis},
  volume={76},
  pages={102303},
  year={2022},
  publisher={Elsevier}
}
@article{li2022medical,
  title={Medical image analysis on left atrial LGE MRI for atrial fibrillation studies: A review},
  author={Li, Lei and Zimmer, Veronika A and Schnabel, Julia A and Zhuang, Xiahai},
  journal={Medical image analysis},
  volume={77},
  pages={102360},
  year={2022},
  publisher={Elsevier}
}

@inproceedings{li2021atrialgeneral, 
  title={AtrialGeneral: domain generalization for left atrial segmentation of multi-center LGE MRIs},
  author={Li, Lei and Zimmer, Veronika A and Schnabel, Julia A and Zhuang, Xiahai},
  booktitle={Medical Image Computing and Computer Assisted Intervention--MICCAI 2021: 24th International Conference, Strasbourg, France, September 27--October 1, 2021, Proceedings, Part VI 24},
  pages={557--566},
  year={2021},
  organization={Springer}
}
```

Original introduction article is [here](https://zhuanlan.zhihu.com/p/659905750).