# PALM19

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/PALM19_0.png"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## Dataset Information

The Pathological Myopia Challenge (PALM) is focused on the research and development of advanced algorithms for the diagnosis of pathological myopia (PM) and the precise segmentation of lesion areas in fundus photographs of PM patients. This event is part of the 2019 International Medical Imaging Conference (ISBI) and is also one of the highly regarded iChallenge series competitions. The main objective of the PALM challenge is to compare and evaluate the performance of various automated algorithms for detecting pathological myopia on a standardized dataset of retinal fundus images. For this purpose, the challenge provides a total of 1200 annotated images, which are divided into 400 training images, 400 validation images, and 400 test images to support the development and testing of participants' algorithms. The challenge primarily focuses on: (1) the classification of normal and myopic fundus; (2) segmentation of typical lesions of pathological myopia (retinal atrophy, hemorrhage, macular lesions). All photographs were taken with a Zeiss Visucam 500.

Myopia has become a global public health burden. Among people with myopia, approximately 35% suffer from high myopia. Myopia leads to elongation of the eyeball, which can cause pathological changes in the retina and choroid. As the degree of myopia increases, high myopia can develop into pathological myopia, characterized by pathological changes forming in the following locations: (1) the posterior pole, including retinal detachment, posterior staphyloma, retinochoroidal degeneration, etc.; (2) the optic disc, including peripapillary atrophy, tilting, etc.; (3) myopic maculopathy, including lacquer cracks, Forster's spots, choroidal neovascularization (CNV), etc. Pathological myopia can cause irreversible visual impairment in patients. Therefore, early diagnosis and regular follow-up are very important.


## Dataset Meta Information

| Dimensions | Modality | Task Type     | Anatomical Structures | Number of Categories | Data Volume                     | File Format |
|------------|----------|---------------|-----------------------|----------------------|---------------------------------|-------------|
| 2D         | Retinal Image   | Segmentation  | Eye             | 1                    | train: 400, val: 400, test: 400 | PNG         |


### Resolution Details

| Dataset Statistics | size          |
|--------------------|---------------|
| min                | (2056, 2124)  |
| median             | (2056, 2124)  |
| max                | (2056, 2124)  |

## Label Information Statistics

| Category          | Retinal Vessel |
|-------------------|----------------|
| Number of Images  | 384            |
| Availability      | 96%            |
| Small Vessel Count| 0              |
| Medium Vessel Count| 66045         |
| Large Vessel Count| 131973         |

## Visualization

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/PALM19_1.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em> Test set visualization results: The optic disc (green contour) is detected and segmented in A, B, and C. Retinal atrophy is detected and segmented (white contour) in B and C. Retinal detachment is detected in C, where the entire fundus is outlined in yellow. Finally, in all cases, the macula is located, indicated by a purple cross.</em></p>

## File Structure

The dataset file structure is as follows. The PALM19 dataset consists of two folders: `images` and `masks`, where the former contains the images and the latter contains the corresponding annotations.

``` 
PALM19          
├── images            
│   ├── train
│       ├── H0001.png
│       ├── H0002.png
│       └──  ...
│   ├── val
│       ├── V0001.png
│       ├── V0002.png
│       └──  ...
│   ├── test
│       ├── T0001.png
│       ├── T0002.png
│       └──  ...
├── masks            
│   ├── train
│       ├── H0001.png
│       ├── H0002.png
│       └──  ...
│   ├── val
│       ├── V0001.png
│       ├── V0002.png
│       └──  ...
│   ├── test
│       ├── T0001.png
│       ├── T0002.png
│       └──  ...
```

## Authors and Institutions

Yanwu Xu (Artificial Intelligence Innovation Business, Baidu Inc., China)

José Ignacio Orlando (Medical University of Vienna, Austria)

Hrvoje Bogunovic (Medical University of Vienna, Austria)

Xiulan Zhang (Zhongshan Ophthalmic Center, Sun Yat-sen University, China)

Fei Li (Zhongshan Ophthalmic Center, Sun Yat-sen University, China)

Xu Sun (Intelligent Healthcare Department, Baidu Inc., China)

Xingxing Cao (Intelligent Healthcare Department, Baidu Inc., China)

Jinling Li (Intelligent Healthcare Department, Baidu Inc., China)


## Source Information

Official Website: https://palm.grand-challenge.org/Home/

Download Link: https://ieee-dataport.org/documents/palm-pathologic-myopia-challenge

Article Address: https://ieee-dataport.org/documents/palm-pathologic-myopia-challenge

Publication Date: 2019

## Citation

``` 
@data{55pk-8z03-19,
doi = {10.21227/55pk-8z03},
url = {https://dx.doi.org/10.21227/55pk-8z03},
author = {Fu, Huazhu and Li, Fei and Orlando, José Ignacio and Bogunović, Hrvoje and Sun, Xu and Liao, Jingan and Xu, Yanwu and Zhang, Shaochong and Zhang, Xiulan},
publisher = {IEEE Dataport},
title = {PALM: PAthoLogic Myopia Challenge},
year = {2019} }
```

Original introduction article is [here](https://zhuanlan.zhihu.com/p/677543244).
