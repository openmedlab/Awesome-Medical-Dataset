# Augemnted ocular diseases

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/AOD_0.png"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## Dataset Information

The Augmented Ocular Disease dataset (AOD) is a classification task dataset within the 2D fundus photography modality. The dataset contains a total of 14.8k fundus photographs, covering seven major retinal diseases (Age-related Macular Degeneration (AMD), Cataracts, Diabetes, Glaucoma, Hypertension, Myopia, Normal) and other types. The images are stored in JPG format. The clinical importance of this task lies in its ability to facilitate early disease detection and diagnosis by classifying various diseases in fundus photographs. It helps in the timely discovery and treatment of ocular diseases such as AMD, cataracts, and diabetic retinopathy. AOD advances the field of medical image classification by providing a large number of high-quality fundus images and precise labels. It offers researchers a standardized platform to compare and evaluate the performance of various classification algorithms, fostering innovation and improvement in algorithms.

## Dataset Meta Information

| Dimensions | Modality        | Task Type      | Anatomical Structures  | Number of Categories | Data Volume | File Format |
|------------|-----------------|----------------|------------------------|----------------------|-------------|-------------|
| 2D         | Retinal Images  | Classification | Retinal                | 7+others             | 14.8K       | JPG         |


### Resolution Details

In this dataset, there are eight categories of labels, which are: amd (Age-related Macular Degeneration), Cataracts, Diabetes, Glaucoma, Hypertension, Myopia, Normal and Other.

| Disease Category   | amd            | cataract     | diabetes     | glaucoma     | hypertension | myopia       | normal       |
|--------------------|----------------|--------------|--------------|--------------|--------------|--------------|--------------|
| Number of Images   | 2,128          | 2,344        | 1,608        | 2,272        | 1,024        | 1,856        | 2,873        |
| Percentage         | 14.37%         | 15.82%       | 10.86%       | 15.34%       | 6.91%        | 12.53%       | 19.40%       |
| Max Pixel Value    | (4496, 4496)   | (4496, 4496) | (5184, 3456) | (3888, 3888) | (3888, 3888) | (5184, 5184) | (5184, 3456) |
| Median Pixel Value | (2592, 1728)   | (2592, 1824) | (2592, 1728) | (2560, 1920) | (2592, 1728) | (2304, 1728) | (2592, 1728) |
| Min Pixel Value    | (1065, 1065)   | (894, 894)   | (924, 788)   | (713, 713)   | (893, 893)   | (893, 893)   | (250, 188)   |

The "other" label represents fundus conditions that do not belong to the aforementioned seven diseases, totaling 708 images, accounting for 4.78% of the dataset. The maximum size is (5184, 3456), the median size is (2592, 1728), and the minimum size is (250, 188).

## Label Information Statistics

This section is statistics results of label information.

| Metric        | Tumor    |
|---------------|----------|
| Case Count    | 501      |
| Coverage      | 49.4%    |
| Min Volume (cm³) | 0.1    |
| Median Volume (cm³) | 99 |
| Max Volume (cm³) | 2480   |

## Visualization

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/AOD_0.png"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## File Structure

``` 
Dataset
│
├── AMD
│   ├── 43_left.jpg
│   ├── 43_right.jpg
│   └── ...
├── cataract
│   ├── 0_left.jpg
│   ├── 43_right.jpg
│   ├── ...
├── cataract
│   ├── 2_right.jpg
│   ├── 4_right.jpg
│   ├── ...
├── ...
```

## Authors and Institutions

Abuev Nurmukhammed Baktybekovich


## Source Information

Official Website: https://www.kaggle.com/datasets/nurmukhammed7/augemnted-ocular-diseases

Download Link: https://www.kaggle.com/datasets/nurmukhammed7/augemnted-ocular-diseases

Article Address: TBD

Publication Date: 2021-04

## Citation

``` 
https://www.kaggle.com/datasets/nurmukhammed7/augemnted-ocular-diseases
```

Original introduction article is [here](https://zhuanlan.zhihu.com/p/703638584).