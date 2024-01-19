# Dataset Name
Here is the template of public medical dataset description.

## Dataset Information

This part is introduction and summarization of the dataset.

## Dataset Meta Information

You can write down meta information about the dataset, take TotalSegmentator for example, it could be:

| Dimensions | Modality | Task Type | Anatomical Structures          | Anatomical Area | Number of Categories | Data Volume | File Format |
|------------|----------|-----------|--------------------------------|-----------------|----------------------|-------------|-------------|
| 3D         | CT       | Segmentation | 27 organs; 59 bones; 10 muscles; 8 vessels | Entire body       | 104                  | 1204        | .nii.gz     |


### Resolution Details

You can also write down the resolution details such as size (x, y, z) and spacing information about the dataset.

For example:

| Dataset Statistics | spacing (mm)     | size            |
|--------------------|------------------|-----------------|
| min                | (1.5, 1.5, 1.5)              | (10, 10, 5)     |
| median             | (1.5, 1.5, 1.5)           | (256, 256, 100) |
| max                | (1.5, 1.5, 1.5)              | (512, 512, 200) |

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

Visualization of dataset, you can use ITK-SNAP to visualize.

Take AutoPET for example:

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/ULS_1.webp"></a>
</div>
<p style="text-align:center;font-size:10px;"><em> ITK-SNAP Visualization.</em></p>

## File Structure

Introduce file structure of original dataset folder.

Take representative MSD dataset for example:

``` 
Task04_Hippocampus
│
├── imagesTr
│   ├── hippocampus_001.nii.gz
│   └── ...
├── labelsTr
│   ├── hippocampus_001.nii.gz
│   └── ...
├── imagesTs
│   ├── hippocampus_002.nii.gz
│   └── ...
└── dataset.json
```

## Authors and Institutions

Introduce authors and their institutions of this dataset.


## Source Information

Official Website: TBD

Download Link: TBD

Article Address: TBD

Publication Date: TBD

## Citation

``` 
TBD
```