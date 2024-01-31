# BUSI

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="400px" height="auto" src="appendix/BUSI_0.png"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## Dataset Information

BUSI (Breast Ultrasound Image) is a classification and segmentation dataset containing breast ultrasound images. The dataset includes breast ultrasound images collected in 2018, covering female patients aged between 25 to 75 years. The dataset consists of 780 images with an average size of 500*500 pixels. These images are categorized into three classes: normal, benign, and malignant. In the benign and malignant breast ultrasound images, there are also detailed segmentation annotations of the corresponding chest tumors, providing key information for in-depth study and accurate diagnosis. This dataset offers a rich image resource and valuable support for breast cancer research.

## Dataset Meta Information

| Dimensions | Modality    | Task Type                    | Anatomical Structures | Anatomical Area | Number of Categories | Data Volume | File Format |
|------------|-------------|------------------------------|-----------------------|-----------------|----------------------|-------------|-------------|
| 2D         | Ultra Sound | Classification, Segmentation | Breast                | Chest           | 3                    | 780         | PNG         |


### Resolution Details

| Dataset Statistics | size        |
|--------------------|-------------|
| min                | [310,190]   |
| median             | [474,190]   |
| max                | [719,190]   |

## Label Information Statistics

| Category  | Normal | Benign | Malignant |
|-----------|--------|--------|-----------|
| Case Count| 133    | 437    | 210       |
| Missing   | 0      | 6.67%  | 14.4%     |

## Visualization

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/BUSI_1.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em> Normal breast ultra sound image.</em></p>

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/BUSI_2.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em> Benign tumor, the red mask indicates the tumor area.</em></p>

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/BUSI_3.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em> Malignant tumor, the red mask indicates the tumor area.</em></p>

## File Structure

The file structure of the dataset is as follows, containing three different folders: benign, malignant, and normal. Each folder contains images and corresponding annotations of breast tumors.

``` 
dataset
├── benign
│   ├── benign (100).png
│   ├── benign (100)_mask.png
│   │    ...
├── malignant
│   ├── malignant (100).png
│   ├── malignant (100)_mask.png
│   ├── ...
├── normal
│   ├── normal (100).png
│   ├── normal (100)_mask.png
│   ├── ...
```

## Authors and Institutions

Walid Al-Dhabyani (Faculty of Computers and Artificial Intelligence, Cairo University, Egypt)

Mohammed Gomaa (National Cancer Institute, Cairo University, Egypt)

Hussien Khaled (National Cancer Institute, Cairo University, Egypt)

Aly Fahmy (Faculty of Computers and Artificial Intelligence, Cairo University, Egypt)


## Source Information

Official Website: https://scholar.cu.edu.eg/?q=afahmy/pages/dataset

Download Link: https://scholar.cu.edu.eg/?q=afahmy/pages/dataset

Article Address: https://www.sciencedirect.com/science/article/pii/S2352340919312181

Publication Date: 11.21.2019.

## Citation

``` 
@article{al2020dataset,
  title={Dataset of breast ultrasound images},
  author={Al-Dhabyani, Walid and Gomaa, Mohammed and Khaled, Hussien and Fahmy, Aly},
  journal={Data in brief},
  volume={28},
  pages={104863},
  year={2020},
  publisher={Elsevier}
}
```

Original introduction article is [here](https://zhuanlan.zhihu.com/p/661462948).