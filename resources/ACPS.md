# ACPS

## Dataset Information

**ACPS (Automatic Cone Photoreceptor Segmentation)** is a dataset specifically designed for the task of automatic segmentation of cone photoreceptors. The dataset includes 840 images derived from the imaging results of the right eyes of 21 subjects. The average age of the 21 subjects is 25.9 ± 6.5 years, with one subject having green color blindness. The gold standard for each image is based on cone positions previously identified using semi-automatic detection methods, which were meticulously reviewed and corrected by experts. Additionally, any missing cones were manually annotated.

The significance of this dataset lies in its provision of a high-quality reference standard for the retinal cone photoreceptor locations, carefully reviewed and corrected by experts. It serves as a reliable benchmark for validating and optimizing the accuracy of automated cone detection algorithms. By comparing the results of automated algorithms with the manually corrected "gold standard" data, researchers can evaluate and improve the performance of these algorithms, thereby enhancing the precision of retinal image analysis. This dataset not only provides a foundation for validating automated image processing techniques but also lays a solid groundwork for research on retinal structures and the development of automated ophthalmic diagnostics.

## Dataset Meta Information

| Dimensions | Modality         | Task Type     | Anatomical Structures | Anatomical Area | Number of Categories | Data Volume | File Format |
|------------|------------------|---------------|-----------------------|-----------------|----------------------|-------------|-------------|
| 2D         | Optical imaging  | Segmentation  | Cone photoreceptors   | Eye             | 1                    | 840         | .mat        |


### Resolution Details

| Dataset Statistics | size     |
|--------------------|----------|
| min                | 150x150  |
| median             | 150x150  |
| max                | 150x150  |

## Label Information Statistics

| Metric              | Cone Photoreceptor |
|---------------------|--------------------|
| Case Count          | 840                |
| Coverage            | 100%               |

## Visualization

The following figure shows the original image, the outline of the cone photoreceptor, and its center point from left to right:

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/ACPS_0.png"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## File Structure

``` 
DAO-SLOCPASA
└── 2013_BOE_Chiu
    ├── Subject01_QuadrantBL_01.mat
    ├── Subject01_QuadrantBL_02.mat
    ├── Subject01_QuadrantBL_03.mat
    ├── Subject01_QuadrantBL_04.mat
    ├── Subject01_QuadrantBL_05.mat
    └── ...
```

## Authors and Institutions

- Stephanie J. Chiu (Duke University, Department of Biomedical Engineering)

- Yuliya Lokhnygina (Duke University, Department of Biostatistics and Bioinformatics)  

- Adam M. Dubis (Duke University, Department of Ophthalmology)  

- Alfredo Dubra (Medical College of Wisconsin, Department of Ophthalmology)  

- Joseph Carroll (Medical College of Wisconsin, Department of Ophthalmology)  

- Joseph A. Izatt (Duke University, Department of Biomedical Engineering)  

- Sina Farsiu (Duke University, Department of Biomedical Engineering)  

## Source Information

Official Website: https://people.duke.edu/~sf59/Chiu_BOE_2013_dataset.htm

Download Link: https://people.duke.edu/~sf59/Chiu_BOE_2013_dataset.htm

Article Address: https://people.duke.edu/~sf59/Chiu_BOE_2013_dataset.htm

Publication Date: 2013

## Citation

``` 
@article{chiu2013automatic,
  title={Automatic cone photoreceptor segmentation using graph theory and dynamic programming},
  author={Chiu, Stephanie J and Lokhnygina, Yuliya and Dubis, Adam M and Dubra, Alfredo and Carroll, Joseph and Izatt, Joseph A and Farsiu, Sina},
  journal={Biomedical optics express},
  volume={4},
  number={6},
  pages={924--937},
  year={2013},
  publisher={Optica Publishing Group}
}
```

Original introduction article is [here](https://zhuanlan.zhihu.com/p/5723729957).