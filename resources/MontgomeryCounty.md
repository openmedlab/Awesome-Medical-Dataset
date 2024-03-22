# MontgomeryCounty

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MontgomeryCounty_0.png"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## Dataset Information

The Montgomery County Chest X-ray (CXR) dataset was created through a collaboration between the National Library of Medicine and the Montgomery County Department of Health and Human Services, Maryland, USA, collecting X-ray data from the tuberculosis screening program in Montgomery County. The dataset contains 138 posteroanterior (PA) chest X-rays, of which 80 are normal and 58 show abnormalities consistent with tuberculosis. All images have been anonymized and are provided in PNG format, with accompanying lung masks for the left and right PA views. The image filenames follow the format "MCUCXR_#####0/1.png," where "0" indicates normal and "1" indicates abnormal. Clinical readings for each X-ray are saved in text file format, named "MCUCXR#####_0/1.txt," containing information about the patient's age, gender, and pulmonary abnormalities (such as tuberculosis). Additionally, the dataset includes consensus annotations and radiological readings made by two radiologists on images resized to 1024×1024 pixels.

This database provides medical researchers and clinicians with a rich resource of chest X-ray images of tuberculosis, aiding them in studying the various manifestations of tuberculosis to improve diagnostic accuracy. As artificial intelligence and machine learning technologies continue to evolve in the medical field, this database has become a valuable resource for developing and testing automated diagnostic algorithms. These advanced technologies can assist in the rapid identification and classification of tuberculosis images, expediting the diagnostic process. Given that tuberculosis is a major global public health issue, this database offers important data support to researchers and public health experts to understand the distribution and presentation of tuberculosis across different populations, aiding in devising more effective prevention and treatment strategies.

## Dataset Meta Information

| Task Type | Language       | Train | Val | Test | File Format | Size  |
|-----------|----------------|-------|-----|------|-------------|-------|
| VQA       | English | 138   | -   | -    | .png/.txt   | 589M |

### Resolution Details

| Dataset Statistics | size          |
|--------------------|---------------|
| min                | (4020, 4892)  |
| median             | (4020, 4892)  |
| max                | (4020, 4892)  |

## Label Information Statistics

| Category                  | Tuberculosis |
|---------------------------|--------------|
| The number of occurrences | 58           |
| Appearance ratio          | 42.03%       |


## Dataset Example

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/MontgomeryCounty_0.png"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## File Structure

The dataset consists of three folders: "ClinicalReadings", "CXR_png", and "ManualMask". "ClinicalReadings" contains information corresponding to each Chest X-Ray, including gender, age, and lung status. "CXR_png" stores the images of each Chest X-Ray, and "ManualMask" contains segmentation masks for the left and right lungs.

``` 
├── ClinicalReadings
│   ├── MCUCXR_0001_0.txt
│   ├── MCUCXR_0002_0.txt
│   ├── MCUCXR_0003_0.txt
│   └── ...
│
├── CXR_png
│   ├── MCUCXR_0001_0.png
│   ├── MCUCXR_0002_0.png
│   ├── MCUCXR_0003_0.png
│   ├── MCUCXR_0004_0.png
│   └── ...
├
├── ManualMask
│   ├── leftMask
│   └── rightMask
└── NLM-MontgomeryCXRSet-ReadMe.pdf
```

## Authors and Institutions

Stefan Jaeger (Lister Hill National Center for Biomedical Communications, National Library of Medicine, National Institutes of Health, USA)

Sema Candemir (Lister Hill National Center for Biomedical Communications, National Library of Medicine, National Institutes of Health, USA)

Sameer Antani (Lister Hill National Center for Biomedical Communications, National Library of Medicine, National Institutes of Health, USA)

Yì-Xiáng J. Wáng (Department of Imaging and Interventional Radiology, Prince of Wales Hospital, The Chinese University of Hong Kong)

Pu-Xuan Lu (Department of Radiology, The Third People's Hospital of Shenzhen, Guangdong Medical University)

George Thoma (Lister Hill National Center for Biomedical Communications, National Library of Medicine, National Institutes of Health, USA)


## Source Information

Official Website: https://lhncbc.nlm.nih.gov/LHC-downloads/downloads.html#tuberculosis-image-data-sets

Download Link: https://openi.nlm.nih.gov/imgs/collections/NLM-MontgomeryCXRSet.zip

Article Address: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4256233/

Publication Date: 2021.6

## Citation

``` 
@article{jaeger2014two,
  title={Two public chest X-ray datasets for computer-aided screening of pulmonary diseases},
  author={Jaeger, Stefan and Candemir, Sema and Antani, Sameer and W{\'a}ng, Y{\`\i}-Xi{\'a}ng J and Lu, Pu-Xuan and Thoma, George},
  journal={Quantitative imaging in medicine and surgery},
  volume={4},
  number={6},
  pages={475},
  year={2014},
  publisher={AME Publications}
}
```

Original introduction article is [here](https://zhuanlan.zhihu.com/p/679980121).