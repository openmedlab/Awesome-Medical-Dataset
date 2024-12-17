# DICOM-LIDC-IDRI-Nodules Dataset

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/DICOM-LIDC-IDRI-Nodules_0.png"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## Dataset Information

**DICOM-LIDC-IDRI-Nodules** (Standardized representation of the TCIA LIDC-IDRI annotations using DICOM) is a standardized DICOM representation of the LIDC-IDRI annotations, containing expert radiologist annotations and characterization data for lung nodules. The dataset focuses on nodules with a diameter of **3 mm or larger**. Originally stored in **XML format**, the data has been converted into **DICOM Segmentation Objects** and **DICOM Structured Report Objects** using the **pylidc** and **dcmqi** libraries. The dataset consists of **1,018 cases** with a total size of **2.51 GB**, including tumor segmentations and image feature information.

This dataset is significant for developing and validating algorithms for lung nodule segmentation and characterization. Through the standardized **DICOM format**, researchers can conveniently access and utilize these annotated data, advancing research related to lung cancer diagnosis and treatment. Additionally, the provided scripts and library tools facilitate further analysis and data conversion.

## Dataset Meta Information

| Dimensions | Modality | Task Type | Anatomical Structures | Anatomical Area | Number of Categories | Data Volume | File Format |
|------------|----------|-----------|-----------------------|-----------------|----------------------|-------------|-------------|
| 3D         | CT       | Segmentation | Lung Nodule           | Lung            | 1                    | 31          | DICOM       |


### Resolution Details

| Dataset Statistics | spacing (mm)        | size             |
|--------------------|---------------------|------------------|
| min                | (0.51, 0.51, 0.625) | (512, 512, 103)  |
| median             | (0.68, 0.68, 1.25)  | (512, 512, 237)  |
| max                | (0.86, 0.86, 3.0)   | (512, 512, 481)  |

Number of 2D slices in the dataset: 6814.

## Label Information Statistics

| Metric              | Lung Nodule |
|---------------------|-------------|
| Case Count          | 31          |
| Coverage            | 100%        |
| Min Volume (cm³)    | 0.03        |
| Median Volume (cm³) | 4.06        |
| Max Volume (cm³)    | 45.28       |

## Visualization

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/DICOM-LIDC-IDRI-Nodules_0.png"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## File Structure

``` 
QIN LUNG CT
│
├── QIN-LSC-0003
│   ├── 04-01-2015-1-NA-41946
│   ├── 08-06-2003-1-CT Thorax wContrast-41946
│   ├── 11-06-2014-1-NA-41946
├── QIN-LSC-00014
│   ├── ..
├── QIN-LSC-00028
│   ├── ..
├── ...
```

## Authors and Institutions

Jayashree Kalpathy-Cramer (Massachusetts General Hospital and Harvard Medical School, Boston, MA, USA

Binsheng Zhao (Department of Radiology, Columbia University Medical Center, New York, NY, USA)

Dmitry Goldgof (Department of Computer Science and Engineering, University of South Florida, Tampa, FL, USA)

Yuhua Gu (Departments of Cancer Imaging and Metabolism, H. Lee Moffitt Cancer Center and Research Institute, Tampa, FL, USA)

Xingwei Wang (Department of Radiology, Stanford University School of Medicine, James H. Clark Center S323 318 Campus Drive, Stanford, CA, 94305-5450, USA)

Hao Yang (Department of Radiology, Columbia University Medical Center, New York, NY, USA)

Yongqiang Tan (Department of Radiology, Columbia University Medical Center, New York, NY, USA)

Robert Gillies (Departments of Cancer Imaging and Metabolism, H. Lee Moffitt Cancer Center and Research Institute, Tampa, FL, USA)

Sandy Napel (Department of Radiology, Stanford University School of Medicine, James H. Clark Center S323 318 Campus Drive, Stanford, CA, 94305-5450, USA)

## Source Information

Official Website: https://www.cancerimagingarchive.net/analysis-result/qin-lungct-seg/

Download Link: https://www.cancerimagingarchive.net/analysis-result/qin-lungct-seg/

Article Address: https://link.springer.com/article/10.1007/s10278-016-9859-z

Publication Date: 2018-12

## Citation

``` 
@article{kalpathy2016comparison,
  title={A comparison of lung nodule segmentation algorithms: methods and results from a multi-institutional study},
  author={Kalpathy-Cramer, Jayashree and Zhao, Binsheng and Goldgof, Dmitry and Gu, Yuhua and Wang, Xingwei and Yang, Hao and Tan, Yongqiang and Gillies, Robert and Napel, Sandy},
  journal={Journal of digital imaging},
  volume={29},
  pages={476--487},
  year={2016},
  publisher={Springer}
}
```

Original introduction article is [here](https://zhuanlan.zhihu.com/p/1213729444).