# SMILE-UHURA 2023

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/SMILE-UHURA 2023_0.avif"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## Dataset Information

SMILE-UHURA2023 (Small Vessel Segmentation at Mesoscopic Scale from Ultra-High Resolution 7T Magnetic Resonance Angiograms 2023) is a 3D magnetic resonance modality dataset for ultra-high resolution small vessel segmentation, part of a challenge at the International Symposium on Biomedical Imaging (ISBI). The dataset is focused on the segmentation of cerebral arteries, including 12 sets of training samples and 2 sets of validation samples. It utilizes automated pre-segmentation techniques combined with extensive manual refinement to accurately annotate time-of-flight (ToF) angiographic images collected.

The brain's supply of nutrients and oxygen depends on the cerebral vascular system. Pathologies of small vessels at the mesoscopic scale are the weak links in cerebral blood supply, prone to causing serious complications such as cerebral small vessel diseases (CSVD). The advancement of 7T MRI technology allows scientists to observe small vessels in the brain with higher spatial resolution. SMILE-UHURA provides this annotated dataset to train machine learning models and has created a platform to evaluate the performance of different methods.

## Dataset Meta Information

| Dimensions | Modality | Task Type | Anatomical Structures | Anatomical Area | Number of Categories | Data Volume | File Format |
|------------|----------|-----------|-----------------------|-----------------|----------------------|-------------|-------------|
| 3D         | MRI      | Segmentation | Cerebral Artery       | Brain           | 1                    | 14          | .nii.gz     |


### Resolution Details

| Dataset Statistics | spacing (mm)     | size             |
|--------------------|------------------|------------------|
| min                | (0.30, 0.30, 0.30)              | (480, 640, 163)  |
| median             | (0.30, 0.30, 0.30)           | (480, 640, 163)  |
| max                | (0.31, 0.31, 0.30)              | (512, 640, 163)  |

Number of two-dimensional slices in the data set: 1956

## Label Information Statistics

This section is statistics results of label information.

| Metric        | Tumor |
|---------------|-------|
| Case Count    | 12    |
| Coverage      | 100%  |
| Min Volume (cm³) | 11.01   |
| Median Volume (cm³) | 15.54    |
| Max Volume (cm³) | 21.13  |

## Visualization

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/SMILE-UHURA 2023_1.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/SMILE-UHURA 2023_2.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## File Structure

The data set file structure is as follows, divided into training set and validation set. Each set includes original images, standard labels, additional annotation labels, and metadata files.

``` 
.
├── SYNAPSE_METADATA_MANIFEST.tsv
├── TrainingSet
│   ├── SYNAPSE_METADATA_MANIFEST.tsv
│   ├── train
│   │   ├── sub004.nii.gz
│   │   ├── sub005.nii.gz
│   │   ├── ...
│   │   └── SYNAPSE_METADATA_MANIFEST.tsv
│   ├── train_label
│   │   ├── sub004.nii
│   │   ├── sub005.nii
│   │   ├── ...
│   │   └── SYNAPSE_METADATA_MANIFEST.tsv
│   ├── train_OMELETTElabel
│   │   ├── sub004_seg_g0.01.nii.gz
│   │   ├── sub004_seg_g0.02.nii.gz
│   │   ├── sub005_seg_g0.01.nii.gz
│   │   ├── ...
│   │   └── SYNAPSE_METADATA_MANIFEST.tsv
│   └── train_plausiblelabel
│       ├── sub004_Segmentation_0.nii.gz
│       ├── sub004_Segmentation_1.nii.gz
│       ├── sub004_Segmentation_2.nii.gz
│       ├── ...
│       └── SYNAPSE_METADATA_MANIFEST.tsv
├── TrainingSet.tar.gz
├── ValidationSet
│   ├── SYNAPSE_METADATA_MANIFEST.tsv
│   ├── validate
│   │   ├── sub007.nii.gz
│   │   ├── sub017.nii.gz
│   │   └── SYNAPSE_METADATA_MANIFEST.tsv
│   ├── validate_label
│   │   ├── sub007.nii
│   │   ├── sub017.nii
│   │   └── SYNAPSE_METADATA_MANIFEST.tsv
│   ├── validate_OMELETTElabel
│   │   ├── sub007_seg_g0.01.nii.gz
│   │   ├── sub007_seg_g0.02.nii.gz
│   │   ├── sub017_seg_g0.01.nii.gz
│   │   ├── sub017_seg_g0.02.nii.gz
│   │   └── SYNAPSE_METADATA_MANIFEST.tsv
│   └── validate_plausiblelabel
│       ├── sub007_Segmentation_0.nii.gz
│       ├── sub007_Segmentation_1.nii.gz
│       ├── sub007_Segmentation_2.nii.gz
│       ├── ...
│       └── SYNAPSE_METADATA_MANIFEST.tsv
└── ValidationSet.tar.gz
```

## Authors and Institutions

Soumick Chatterjee (University of Magdeburg, Germany)

Hendrik Mattern (University of Magdeburg, Germany)

Florian Dubost (Liminal Sciences, USA)

Stefanie Schreiber (University of Magdeburg, Germany)

Andreas Nürnberger (University of Magdeburg, Germany)

Oliver Speck (University of Magdeburg, Germany)


## Source Information

Official Website: https://www.synapse.org/#!Synapse:syn47164761/wiki/620033

Download Link: https://www.synapse.org/#!Synapse:syn47164761/wiki/620033, https://www.soumick.com/en/uhura/

Article Address: TBD

Publication Date: 2023-03

## Citation

``` 
TBD
```

Original introduction article is [here](https://zhuanlan.zhihu.com/p/688351484).