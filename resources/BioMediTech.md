# BioMediTech

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/BioMediTech_0.avif"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## Dataset Information

To assess the suitability of human pluripotent stem cell (hPSC)-derived retinal pigment epithelium (RPE) cells for implantation or in vitro use, a rapid, non-invasive, and observer-independent method is required to analyze their homogeneity and maturity. The BioMediTech dataset aids in the development and validation of classification and feature description algorithms. This dataset consists of 195 microscopy original images containing RPE cells at different stages. Each original image is divided into 16 sub-images using a 4x4 grid division method. Any sub-images that are too chaotic, out of focus, or have only background are discarded, resulting in a total of 1862 images. Each sub-image is categorized by two professional annotators, with four candidate categories available.

## Dataset Meta Information

| Dimensions | Modality | Task Type       | Anatomical Structures | Anatomical Area | Number of Categories | Data Volume                               | File Format |
|------------|----------|-----------------|-----------------------|-----------------|----------------------|-------------------------------------------|-------------|
| 2D         | Microscopy       | Classification  | Cell                  | Retinal         | 4                    | 195 - original picture; 1862 - subpicture | .tif        |


### Resolution Details

| Dataset Statistics | size         |
|--------------------|--------------|
| min                | [2560,1920]- original picture, [640,480] - subpicture   |
| median             | [2560,1920]- original picture, [640,480] - subpicture   |
| max                | [2560,1920]- original picture, [640,480] - subpicture   |



## Label Information Statistics

| Category        | Number |
|-----------------|--------|
| Fusiform        | 216    |
| Epithelioid     | 547    |
| Cobblestone     | 949    |
| Mixed           | 150    |

## Visualization

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/BioMediTech_1.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em> Original image example.</em></p>

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/BioMediTech_2.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em> Class 1 "Fusiform" image example.</em></p>

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/BioMediTech_3.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em> Class 2 "Epithelioid" image example.</em></p>

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/BioMediTech_4.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em> Class 3 "Cobblestone" image example.</em></p>

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/BioMediTech_5.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em> Class 4 "Mixed" image example.</em></p>


## File Structure

After unzipping, you obtain the ToolRPE tool folder and the RPE_dataset data set folder. The file structure of the dataset is as follows, containing an original image folder, a sub-image folder, an explanatory PDF file, and a license text file.
``` 
RPE_dataset
├── Images
│   ├── 1_00001.tif
│   ├── 1_00002.tif
│   │    ...
├── Subwindows
│   ├── 1_00001_001_1_1.tif
│   ├── 1_00001_002_1_1.tif
│   ├── ...
├── Description.pdf
├── license.txt
```

## Authors and Institutions

Loris Nanni (University of Padua, Italy)

Michelangelo Paci (Tampere University of Technology, Finland)

Florentino Luciano Caetano dos Santos (Tampere University of Technology, Finland)

Heli Skottman (University of Tampere, Finland)

Kati Juuti-Uusitalo (University of Tampere, Finland)

Jari Hyttinen (Tampere University of Technology, Finland)


## Source Information

Official Website: https://figshare.com/s/d6fb591f1beb4f8efa6f

Download Link: https://figshare.com/ndownloader/articles/2070109?private_link=d6fb591f1beb4f8efa6f

Article Address: https://journals.plos.org/plosone/article/file?id=10.1371/journal.pone.0149399&type=printable

Publication Date: 2016-02-04

## Citation

``` 
@article{nanni2016texture,
  title={Texture descriptors ensembles enable image-based classification of maturation of human stem cell-derived retinal pigmented epithelium},
  author={Nanni, Loris and Paci, Michelangelo and Caetano dos Santos, Florentino Luciano and Skottman, Heli and Juuti-Uusitalo, Kati and Hyttinen, Jari},
  journal={PLoS One},
  volume={11},
  number={2},
  pages={e0149399},
  year={2016},
  publisher={Public Library of Science San Francisco, CA USA}
}
```

Original introduction article is [here](https://zhuanlan.zhihu.com/p/663725649).