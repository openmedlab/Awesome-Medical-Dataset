# CT-ORG

## Dataset Information

CT-ORG (CT volume with multiple organ segmentations) is a CT dataset containing multiple organ segmentations. It consists of 140 CT volumes, among which 131 volumes are paired with PET-CT datasets. The dataset extends the list of organs from the LITS challenge, including 9 additional organs, resulting in a total of 6 categories and 21 organs. The dataset is divided into training, validation, and testing subsets based on LITS, with an emphasis on organs commonly segmented in clinical practice, aiming for a comprehensive organ coverage for CT body scans.

## Dataset Meta Information

| Dimensions | Modality | Task Type | Anatomical Structures          | Anatomical Area | Number of Categories | Data Volume                   | File Format |
|------------|----------|-----------|--------------------------------|-----------------|----------------------|-------------------------------|-------------|
| 3D         | CT       | Segmentation | Lung, Bone, Liver, Kidney, Bladder, Brain | Whole Body       | 6                    | 119 for training, 21 for test | .nii.gz     |

### Resolution Details

| Resolution Level | spacing (mm)     | size             |
|------------------|------------------|------------------|
| Original Image   | (0.56, 0.56, 0.70) | (512, 512, 74)  |
| Medium Resolution| (0.78, 0.78, 1.0)  | (512, 512, 458) |
| High Resolution  | (1.37, 1.37, 5.0)  | (512, 512, 987) |

The CT-ORG dataset contains a total of 63,503 images.

## Label Information Statistics

| Organ    | Liver     | Bladder  | Lungs    | Kidneys  | Bone     | Brain    |
|----------|-----------|----------|----------|----------|----------|----------|
| Case Count   | 140       | 114      | 140      | 140      | 140      | 9        |
| Coverage    | 100%      | 80%      | 100%     | 100%     | 100%     | 6.43%    |
| Min Volume (cm³) | 1220      | 12       | 875      | 90       | 348      | 340      |
| Median Volume (cm³) | 1480      | 144      | 2269     | 317      | 2499     | 1432     |
| Max Volume (cm³) | 3144      | 950      | 8822     | 494      | 9485     | 1516     |

## Visualization

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/CT-ORG.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em> ITK-SNAP Visualization. Red: Liver, Green: Bladder, Dark Blue: Lungs, Yellow: Kidneys, Light Blue: Bone.</em></p>

## File Structure

The official file structure is as follows: images are stored in the form of "volume-x.nii.gz", where x is a one to three-digit case number, ranging from 0 to 139. The first 21 images, numbered 0-20, make up the test set. The remaining images make up the training set. Segmentation data is stored in the form of "labels-x.nii.gz", where x corresponds to the number of the associated image file.

## Authors and Institutions

Blaine Rister (Stanford University, Department of Electrical Engineering, USA)

Darvin Yi (Stanford University, Department of Biomedical Data Science, USA)

Kaushik Shivakumar (Stanford University, Department of Biomedical Data Science, USA)

Daniel L. Rubin (Stanford University, Department of Biomedical Data Science & Department of Radiology, USA)

Tomomi Nobashi (Stanford University, Department of Radiology, USA)

## Source Information

Official Website: https://github.com/bbrister/ctOrganSegmentation

Download Link: https://wiki.cancerimagingarchive.net/pages/viewpage.action?pageId=61080890

Article Address: https://www.nature.com/articles/s41597-020-00715-8

Publication Date: 2020

## Citation

``` 
@article{rister2020ct,
  title={CT-ORG, a new dataset for multiple organ segmentation in computed tomography},
  author={Rister, Blaine and Yi, Darvin and Shivakumar, Kaushik and Nobashi, Tomomi and Rubin, Daniel L},
  journal={Scientific Data},
  volume={7},
  number={1},
  pages={381},
  year={2020},
  publisher={Nature Publishing Group UK London}
}
```

Original introduction article is [here](https://zhuanlan.zhihu.com/p/659785937).