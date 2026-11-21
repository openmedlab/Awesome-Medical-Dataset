# Brain MRI ND-5

## Dataset Information

Brain MRI ND-5 is a labeled brain tumor MRI dataset released by Arché Intelligence Lab on IEEE DataPort, curated for brain tumor classification and detection. It combines five public datasets (as described in the T3SSLNet paper) and was built for self-supervised pre-training and tumor classification. Each MRI image is labeled with one of four classes: glioma, meningioma, pituitary tumor, or no tumor. The data is split into a training set and a testing set.

The dataset is licensed under CC BY 4.0 (per the DOI record). It is free for academic research, and the files are shared by the authors on request.

## Dataset Meta Information

| Dimensions | Modality | Task Type      | Anatomical Structures | Anatomical Area | Number of Categories | Data Volume                     | File Format |
|------------|----------|----------------|-----------------------|-----------------|----------------------|---------------------------------|-------------|
| 2D         | MRI      | Classification | Brain                 | Brain Tumor     | 4                    | Not stated (993.69 MB ZIP file) | ZIP         |

## Label Information Statistics

| Category   | Description                                  |
|------------|----------------------------------------------|
| Glioma     | MRI images of patients with glioma tumors     |
| Meningioma | MRI images of patients with meningioma tumors |
| Pituitary  | MRI images of patients with pituitary tumors  |
| No-Tumor   | MRI images of patients without any tumor      |

## File Structure

```
Brain MRI ND-5 Dataset.zip
│
├── Training
│   ├── Glioma
│   ├── Meningioma
│   ├── Pituitary
│   └── No-Tumor
│
└── Testing
    ├── Glioma
    ├── Meningioma
    ├── Pituitary
    └── No-Tumor
```

## Authors and Institutions

Md. Nasif Safwan (Arché Intelligence Lab)

Souhardo Rahman (Arché Intelligence Lab)

Mahamodul Hasan Mahadi (Arché Intelligence Lab)

Taharat Muhammad Jabir (Arché Intelligence Lab)

## Source Information

Official Website: https://doi.org/10.21227/q2vt-tf46

Download Link: https://doi.org/10.21227/q2vt-tf46 (files are shared by the authors on request; more info: https://www.archelab.org/datasets/brain-mri-nd-5)

Article Address: https://doi.org/10.1109/ACCESS.2025.3589619

Publication Date: 2024-10

## Citation

```
@data{q2vt-tf46,
  author = {Safwan, Md. Nasif and Rahman, Souhardo and Mahadi, Mahamodul Hasan and Jabir, Taharat Muhammad},
  title = {Brain MRI ND-5 Dataset},
  publisher = {IEEE Dataport},
  year = {2024},
  doi = {10.21227/q2vt-tf46},
  url = {https://doi.org/10.21227/q2vt-tf46}
}
```
