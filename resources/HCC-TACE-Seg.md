# HCC-TACE-Seg

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/HCC-TACE-Seg_0.avif"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## Dataset Information

The HCC-TACE-Seg dataset is a CT modality dataset for segmenting organs and tumors, part of the TCIA database. It contains pre- and post-treatment CT data from 105 patients with hepatocellular carcinoma (HCC), the most common type of primary liver cancer. The incidence of HCC has doubled in the past two decades due to increased risk factors. Most cases are diagnosed late when only transarterial chemoembolization (TACE) or systemic treatment is feasible. Up to 60% of patients undergoing TACE experience treatment failure, leading to significant financial and emotional burdens. Radiomics, a new tool, can predict tumor response to TACE from pre-treatment CT studies.

This dataset includes data from 105 HCC-diagnosed patients, spanning from 2002 to 2012, featuring pre- and post-treatment multi-phase enhanced CT images, free from artifacts like surgical clips, and taken within 1 to 12 weeks (average 3 weeks) before initial TACE treatment. Segmentation was semi-automatically performed using AMIRA, including the liver, tumors, and vessels, with manual clinical corrections. Data were converted from NIfTI to DICOM-SEG format for segmentation. These pre-treatment CT segmentations are used for predicting and training automatic liver tumor segmentation algorithms, as well as studying the relationship between pre-treatment CT image features and TACE treatment outcomes, aiming to predict patient response to TACE. Analyzing the imaging and treatment outcome data within this dataset enhances understanding of HCC, improving diagnostic and treatment strategies. All images are artifact-free, ensuring high-quality data for analysis and algorithm training. The segmentation results, clinically manually corrected, cover a decade of clinical data, offering high research value. This dataset provides a valuable resource for further clinical research and radiomics analysis, aiding in the improvement of diagnostic and therapeutic approaches for HCC.

## Dataset Meta Information

| Dimensions | Modality | Task Type    | Anatomical Structures | Anatomical Area | Number of Categories | Data Volume | File Format |
|------------|----------|--------------|-----------------------|-----------------|----------------------|-------------|-------------|
| 3D         | CT       | Segmentation | Liver, Liver Tumor    | Abdomen         | 4                    | 628         | .dcm        |


### Resolution Details

You can also write down the resolution details such as size (x, y, z) and spacing information about the dataset.

For example:

| Dataset Statistics | spacing (mm)        | size            |
|--------------------|---------------------|-----------------|
| min                | (0.58, 0.58, 2.50)  | (512, 512, 40)  |
| median             | (0.78, 0.78, 2.50)  | (512, 512, 87)  |
| max                | (0.98, 0.98, 5.00)  | (512, 512, 185) |

Number of 2D slices in the dataset: 19844.

## Label Information Statistics

| Anatomy     | Total Cases | Coverage | Minimum Volume (cm³)  | Median Volume (cm³) | Maximum Volume (cm³) |
|-------------|-------------|----------|-----------------------|---------------------|----------------------|
| liver       | 224         | 100%     | 600.28                | 1391.05             | 2804.7               |
| liver tumor | 224         | 100%     | 3.94                  | 113.965             | 4054.63              |
| portal vein | 224         | 100%     | 3.29                  | 20.3                | 188.73               |
| aorta       | 224         | 100%     | 2.85                  | 10.71               | 126.53               |


## Visualization

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/HCC-TACE-Seg_1.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em>Red indicates the liver, green indicates liver tumors, small blue areas indicate the portal vein, and yellow indicates the aorta.</em></p>

## File Structure

The main directory contains the identification number for each patient, which includes both pre-operative and post-operative data, presented in the form of DICOM (dcm) files.

``` 
HCC-TACE-Seg
│
├── HCC-TACE-Seg
│   ├── HCC_001
│   │   ├── 04-21-2000-NA-CT ABDPEL WC-49771
│   │   ├── 3.000000-Recon 2 PRE LIVER-07012
│   │   │   ├──1-01.dcm
│   │   │   ├──1-02.dcm
│   │   │   ├──1-03.dcm
│   │   │   ├──...
│   │   ├── 100.000000-NA-46705
│   │   │   ├──1-01.dcm
│   │   │   ├──1-02.dcm
│   │   │   ├──1-03.dcm
│   │   │   ├──...
│   │   ├── 101.000000-NA-35194
│   │   │   ├──1-01.dcm
│   │   │   ├──1-02.dcm
│   │   │   ├──1-03.dcm
│   │   │   ├──...
│   │   ├──  11-30-1999-NA-CT-CAP WWO CON-00377
│   │   │   ├── 2.000000-PRE LIVER-76970
│   │   │   │   ├──1-01.dcm
│   │   │   │   ├──1-02.dcm
│   │   │   │   ├──1-03.dcm
│   │   │   │   ├──...
│   │   │   ├── 3.000000-C-A-P-42120
│   │   │   │   ├──1-01.dcm
│   │   │   │   ├──1-02.dcm
│   │   │   │   ├──1-03.dcm
│   │   │   │   ├──...
│   │   │   ├── 300.000000-Segmentation-99942
│   │   │   │   ├──1-01.dcm
│   ├── ...
```

## Source Information

Official Website: https://www.cancerimagingarchive.net/collection/hcc-tace-seg/

Download Link: https://www.cancerimagingarchive.net/collection/hcc-tace-seg/

Publication Date: 2022-08

## Citation

``` 
@article{moawad2021multimodality,
  title={Multimodality annotated HCC cases with and without advanced imaging segmentation [data set]},
  author={Moawad, A and Fuentes, D and Morshid, A and Khalaf, A and Elmohr, M and Abusaif, A and Hazle, JD and Kaseb, AO and Hassan, M and Mahvash, A and others},
  journal={The Cancer Imaging Archive},
  year={2021}
}
```

Original introduction article is [here](https://zhuanlan.zhihu.com/p/708599534).