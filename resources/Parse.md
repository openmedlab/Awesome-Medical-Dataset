# Parse 2022

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/Parse_0.avif"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## Dataset Information

Parse 2022 (Pulmonary Artery Segmentation) is a CT dataset for pulmonary artery segmentation and part of a challenge at MICCAI 2022. The dataset includes 200 cases of finely annotated pulmonary artery 3D CT data by 10 doctors. The officials have divided the dataset into 100 cases for training, 30 cases for validation, and 70 cases for testing. Currently, only the images and labels for the 100 training cases have been made public. Images for the validation set are public but do not come with labels, and the online submission on the official website has been closed.

## Dataset Meta Information

| Dimensions | Modality | Task Type | Anatomical Structures         | Anatomical Area | Number of Categories | Data Volume                                       | File Format |
|------------|----------|-----------|-------------------------------|-----------------|--------------------|---------------------------------------------------|-------------|
| 3D         | CT       | Segmentation | Pulmonary artery | Chest           | 1                  | 100 for training, 30 for validation, 70 for test. | .nii.gz     |

Number of two-dimensional slices in the training set: 30,340 (based on statistics from 100 training images).

### Resolution Details

| Dataset Statistics | spacing (mm)     | size            |
|--------------------|------------------|-----------------|
| min                | (0.5039, 0.5039, 0.8)              | (512, 512, 228)     |
| median             | (0.6543, 0.6543, 1.0)           | (512, 512, 301) |
| max                | (0.9238, 0.9238, 1.0)              | (512, 512, 390) |

## Label Information Statistics

| Anatomical Structure | Pulmonary Artery |
|----------------------|------------------|
| Cases                | 100              |
| Coverage             | 100%             |
| Mean Volume (cm³)    | 80.94            |
| Median Volume (cm³)  | 129.31           |
| Max Volume (cm³)     | 357.7            |


## Visualization

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/Parse_1.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em> ITK-SNAP Visualization.</em></p>

## File Structure

The official file structure is divided into two main directories: `train` and `evaluation`. The `train` directory contains 100 subfolders named with sequence numbers, each containing two subdirectories, `image` and `label`, which include the `.nii.gz` files for images and corresponding labels. The `evaluation` directory directly contains 30 `.nii.gz` files for images only.

``` 
train
│
├── PA000005
│   ├── image
│   │   └── PA000005.nii.gz
│   └── label
│       └── PA000005.nii.gz
│
...
│
├── PA000317
│   ├── image
│   │   └── PA000317.nii.gz
│   └── label
│       └── PA000317.nii.gz
│
evaluation
│
├── PA000013.nii.gz
...
│
├── PA000316.nii.gz
```

## Authors and Institutions

Gongning Luo (School of Computer Science and Technology, Harbin Institute of Technology)

Kuanquan Wang (Director of the Center for Perception Computing, School of Computer Science and Technology, Harbin Institute of Technology)

Zhaowen Qiu (Department of Image Science and Technology, Heilongjiang Tuoming Technology Co., Ltd., Northeast Forestry University)

Wei Wang (School of Computer Science and Technology, Harbin Institute of Technology)

Tao Song (Harbin Medical University)

Shaodong Cao (Department of Radiology, The Fourth Affiliated Hospital of Harbin Medical University)

Yi Zhao (Harbin Medical University)

Jun Liu (School of Computer Science and Technology, Harbin Institute of Technology)

Yingte He (School of Computer Science and Technology, Harbin Institute of Technology)

Xinjie Liang (School of Computer Science and Technology, Harbin Institute of Technology)

Mingwang Xu (School of Computer Science and Technology, Harbin Institute of Technology)

Zhenghao Song (School of Computer Science and Technology, Harbin Institute of Technology)

Haokai Chi (School of Computer Science and Technology, Harbin Institute of Technology)

Chunyue Zheng (School of Computer Science and Technology, Harbin Institute of Technology)

Xinghua Ma (School of Computer Science and Technology, Harbin Institute of Technology)

Jinwen Guo (School of Computer Science and Technology, Harbin Institute of Technology)


## Source Information

Official Website: https://parse2022.grand-challenge.org/

Download Link: https://parse2022.grand-challenge.org/Dataset/

Article Address: https://arxiv.org/abs/2304.03708

Publication Date: April, 2022.

## Citation

``` 
@misc{luo2023parse,
    title={Efficient automatic segmentation for multi-level pulmonary arteries: The PARSE challenge},
    author={Gongning Luo and Kuanquan Wang and Jun Liu and Shuo Li and Xinjie Liang and Xiangyu Li and Shaowei Gan and Wei Wang and Suyu Dong and Wenyi Wang and Pengxin Yu and Enyou Liu and Hongrong Wei and Na Wang and Jia Guo and Huiqi Li and Zhao Zhang and Ziwei Zhao and Na Gao and Nan An and Ashkan Pakzad and Bojidar Rangelov and Jiaqi Dou and Song Tian and Zeyu Liu and Yi Wang and Ampatishan Sivalingam and Kumaradevan Punithakumar and Zhaowen Qiu and Xin Gao},
    year={2023},
    eprint={2304.03708},
    archivePrefix={arXiv},
    primaryClass={eess.IV}
}
```

Original introduction article is [here](https://zhuanlan.zhihu.com/p/656438569).