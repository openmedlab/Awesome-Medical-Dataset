# OCTA-500

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/OCTA-500_0.png"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## Dataset Information

Optical Coherence Tomography Angiography (OCTA) is a retinal imaging method that allows for the three-dimensional structure of retinal blood vessels to be presented with micrometer-level resolution. The OCTA-500 dataset contains three-dimensional data of OCT and OCTA modalities for 500 eyes, six types of projection images, four types of textual labels (age/gender/eye/disease), and seven types of segmentation labels (large vessels/capillaries/arteries/veins/2D FAZ/3D FAZ/retinal layers).

## Dataset Meta Information

| Dimensions | Modality | Task Type | Anatomical Structures | Anatomical Area | Number of Categories | Data Volume | File Format |
|------------|----------|-----------|-----------------------|-----------------|----------------------|-------------|-------------|
| 2D         | Retinal Image   | Segmentation | Eye                   | Eye             | 1                    | 300 images  | PNG         |


### Resolution Details

| Dataset Statistics | size         |
|--------------------|--------------|
| min                | (400, 400)   |
| median             | (400, 400)   |
| max                | (400, 400)   |

## Label Information Statistics

| Category          | Retinal Vessel |
|-------------------|----------------|
| Number of Images  | 300            |
| Availability      | 100%           |
| Small Vessel Count| 7364          |
| Medium Vessel Count| 20944         |
| Large Vessel Count| 148865         |

## Visualization

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/OCTA-500_0.png"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## File Structure

``` 
OCTA500 Dataset
|
|-- Label.zip
|-- Code.zip
|-- OCTA_3mm_part1.zip
|-- OCTA_3mm_part2.zip
|-- ......
|-- OCTA_3mm_part8.zip
```

## Authors and Institutions

Mingchao Li (School of Computer Science and Engineering, Nanjing University of Science and Technology)

Yerui Chen (School of Computer Science and Engineering, Nanjing University of Science and Technology)

Zexuan Ji (School of Computer Science and Engineering, Nanjing University of Science and Technology)

Keren Xie (Department of Ophthalmology, The First Affiliated Hospital of Nanjing Medical University)

Songtao Yuan (Department of Ophthalmology, The First Affiliated Hospital of Nanjing Medical University)

Qiang Chen (School of Computer Science and Engineering, Nanjing University of Science and Technology)

Shuo Li (Department of Medical Imaging, Western University, Canada)


## Source Information

Official Website: https://ieee-dataport.org/open-access/octa-500

Download Link: https://ieee-dataport.org/open-access/octa-500

Article Address: https://ieeexplore.ieee.org/document/9085991

Publication Date: 2020-06

## Citation

``` 
@article{li2019octa,
  title={OCTA-500},
  author={Li, Mingchao and Chen, Yerui and Yuan, Songtao and Chen, Qiang},
  journal={IEEE Transactions on Medical Imaging},
  volume={39},
  number={9},
  pages={2806--2818},
  year={2019},
  publisher={IEEE},
  doi={10.1109/TMI.2020.2992244},
  url={https://doi.org/10.1109/TMI.2020.2992244}
}

@ARTICLE{9085991,
  author={Li, Mingchao and Chen, Yerui and Ji, Zexuan and Xie, Keren and Yuan, Songtao and Chen, Qiang and Li, Shuo},
  journal={IEEE Transactions on Medical Imaging}, 
  title={Image Projection Network: 3D to 2D Image Segmentation in OCTA Images}, 
  year={2020},
  volume={39},
  number={11},
  pages={3343-3354},
  doi={10.1109/TMI.2020.2992244}}
```

Original introduction article is [here](https://zhuanlan.zhihu.com/p/663867863).