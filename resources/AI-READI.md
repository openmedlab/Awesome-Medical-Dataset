# AI-READI Dataset
Flagship Dataset of Type 2 Diabetes from the AI-READI Project

## Dataset Information
This dataset is created by the Artificial Intelligence Ready and Exploratory Atlas for Diabetes Insights (AI-READI) project as part of the NIH Bridge2AI program. The project seeks to create a flagship dataset to enable future generations of artificial intelligence/machine learning (AI/ML) research to provide critical insights into type 2 diabetes mellitus (T2DM), including salutogenic pathways to return to health. The current version of the dataset (version 2) released in November 2024 contains data from 1067 participants that was collected between July 19, 2023 and July 31, 2024. Data from multiple modalities are included, including 3D OCT, 3D OCTA, 2D fundus, and en face images. A full list is provided in the Data Standards section included in the [Dataset Meta Information](#dataset-meta-information). The data is accessible through a new data repository we are developing called [FAIRhub](https://fairhub.io/datasets/2). The data in this dataset contain no protected health information (PHI). Information related to the sex and race/ethnicity of the participants as well as medication used has also been removed. More details about the project is available in the project website and the dataset documentation listed below under Source Information.

## Dataset Meta Information

### Retinal FLIO (Fluorescence Lifetime Imaging Ophthalmoscopy)

| Manufacturer | Manufacturers Model Name | Laterality | Wavelength                          | Height | Width | Number of Frames |
| ------------ | ------------------------ | ---------- | ----------------------------------- | ------ | ----- | ---------------- |
| Heidelberg   | FLIO                     | R or L     | Short-wavelength or Long-wavelength | 256    | 256   | 1024             |

### Retinal OCT (Optical Coherence Tomography)
| Manufacturer | Manufacturer's Model (device) | Protocol Name                | Anatomic Regions | Width | Height      | Number of frames | Notes                                                                                           |
| ------------ | ----------------------------- | ---------------------------- | ------------------ | ----- | ----------- | ---------------- | ----------------------------------------------------------------------------------------------- |
| Heidelberg   | Spectralis                    | Spec-ONH-RC-HR-OCT           | Optic Disc         | 496   | 768         | 27               |                                                                                                 |
| Heidelberg   | Spectralis                    | Spec-MAC-HR-OCT              | Macula             | 496   | 768 or 1536 | 61               | Two versions of the protocols were used for the pilot but in the future 496, 1536 will be used. |
| Topcon       | Maestro2                      | Maestro2-3D-Wide             | Macula             | 885   | 512         | 128              |                                                                                                 |
| Topcon       | Maestro2                      | Maestro2-3D-Macula           | Macula             | 885   | 512         | 128              |                                                                                                 |
| Topcon       | Maestro2                      | Maestro2-Mac-6x6             | Macula             | 885   | 360         | 60               | 6 files have different dimensions (885, 320, 320)                                               |
| Topcon       | Triton                        | Triton-3D(H)+Radial 12x9-OCT | Optic Disc         | 992   | 512         | 256              |                                                                                                 |
| Topcon       | Triton                        | Triton-Macula 6x6-OCTA       | Macula             | 992   | 320         | 320              |                                                                                                 |
| Topcon       | Triton                        | Triton-Macula 12x12-OCTA     | Macula             | 992   | 512         | 512              |                                                                                                 |


### Retinal OCTA (Optical Coherence Tomography Angiography)
| Manufacturer  | Manufacturer's Model (device)  |  Protocol Name                        |  Anatomic Regions |  Imaging |  Notes                                                                                                                                                                                                                                          |
|---------------|--------------------------------|---------------------------------------|-------------------|----------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|  Topcon       |  Maestro2                      |  Maestro2-Mac 6x6-360x360-(rep3)-OCTA |  Macula, 6 x 6    |  OCTA    | <br>      Each OCTA scan produces: 1 reference retinal photography file (IR or color photo) 1 OCT<br>      (structural scan) file, 2 flow cube files (processed and raw data), 1 heightmap segmentation<br>      file, 4 en face images<br>     |
|  Topcon       |  Triton                        |  Triton-Macula 6x6-OCTA               |  Macula, 6 x 6    |  OCTA    |
|  Topcon       |  Triton                        | Triton-Macula 12x12-OCTA              | Macula, 12 x 12   |  OCTA    |


### Retinal photography
| Manufacturer | Manufacturer's Model (device) | Anatomic Regions                        | Imaging Types                                           | Dilation |
| ------------ | ----------------------------- | ----------------------------------------- | --------------------------------------------------------- | -------- |
| Optomed      | Aurora                        | Macula, Optic Disc                        | Color Photography                                         | No       |
| iCare        | Eidon                         | Macula, Nasal, Temporal Periphery, Mosaic | Color Photography, Infrared Reflectance, Autofluorescence | Yes      |
| Topcon       | Maestro2                      | Macula, Wide Field                        | Color Photography, Infrared Reflectance                   | Yes      |
| Topcon       | Triton                        | Macula, Optic Disc                        | Color Photography                                         | Yes      |
| Heidelberg   | Spectralis                    | Macula, Optic Disc                        | Infrared Reflectance                                      | Yes      |



## Label Information Statistics

The AI-READI dataset provides a rich set of labels suitable for a wide variety of machine learning tasks in medical imaging. One of the primary classification targets is **diabetes status**, categorized into:


| Category | Number |
|----------|--------|
| No DM     | 372    |
| Lifestyle | 242    |
| Oral      | 323    |
| Insulin   | 130    |


- **No DM** : Participants who do not have Type 1 or Type 2 Diabetes
- **Lifestyle**: Participants with pre-Type 2 Diabetes and those with Type 2 Diabetes whose blood sugar is controlled by lifestyle adjustments
- **Oral**: Participants with Type 2 Diabetes whose blood sugar is controlled by oral or injectable medications other than insulin
- **Insulin**: Participants with Type 2 Diabetes whose blood sugar is controlled by insulin

In addition to these categorical labels, the dataset offers **a wide range of patient-level clinical measurements** that can be used as continuous or categorical targets for training. These include, but are not limited to:

- **Age-related Macular Degeneration (AMD)**
- **Glaucoma**
- **Hemoglobin A1c (HgbA1c)**
- **MoCA** (Montreal Cognitive Assessment)
- and many more...

To facilitate model development, the dataset comes with a [PyTorch-based dataloader](https://github.com/AI-READI/aireadi_loader/) that allows users to easily construct image–target pairs for tasks such as classification, regression, and segmentation.


## Demographic Breakdown of Data Splits

The AI-READI dataset comes with a **predetermined train/validation/test split** to support reproducible research and fair benchmarking. Below is the breakdown of the number of patients in each split by demographic categories such as sex, race, and diabetes status.

|                         | Train         |           |       |         | Val          |           |       |         | Test         |           |       |         | Total        |           |       |         |
| ----------------------- | ------------- | --------- | ----- | ------- | ------------ | --------- | ----- | ------- | ------------ | --------- | ----- | ------- | ------------ | --------- | ----- | ------- |
|                         | Hispanic      | Asian     | Black | White   | Hispanic     | Asian     | Black | White   | Hispanic     | Asian     | Black | White   | Hispanic     | Asian     | Black | White   |
| Race/ethnicity (count)  | 144           | 167       | 211   | 225     | 40           | 40        | 40    | 40      | 40           | 40        | 40    | 40      | 224          | 247       | 291   | 305     |
|                         | Male          | Female    |       |         | Male         | Female    |       |         | Male         | Female    |       |         | Male         | Female    |       |         |
| Sex (count)             | 302           | 445       |       |         | 80           | 80        |       |         | 80           | 80        |       |         | 462          | 605       |       |         |
|                         | No DM         | Lifestyle | Oral  | Insulin | No DM        | Lifestyle | Oral  | Insulin | No DM        | Lifestyle | Oral  | Insulin | No DM        | Lifestyle | Oral  | Insulin |
| Diabetes status (count) | 292           | 162       | 235   | 58      | 40           | 40        | 47    | 33      | 40           | 40        | 41    | 39      | 372          | 242       | 323   | 130     |
| Mean age (years ± sd)   | 60.3  ± 11.13 |           |       |         | 60.2 ±  10.5 |           |       |         | 60.4 ±  11.0 |           |       |         | 60.3 ±  11.1 |           |       |         |
| Total                   | 747           |           |       |         | 160          |           |       |         | 160          |           |       |         | 1067         |           |       |         |




## Visualization

### Retinal FLIO (Fluorescence Lifetime Imaging Ophthalmoscopy)
<figure>
  <img src="https://docs.aireadi.org/img/retinal-flio/fig1.png" />
  <figcaption>
    Figure 1. Demonstrating outputs of Fluorescence Lifetime Imaging Ophthalmoscopy in eyes with
    age-related macular degeneration. These images are preprocessed, overlaid, and plotted as a
    heatmap. FAF: fundus autofluorescence, AMD: age-related macular degeneration, SSC: short
    spectral channel, LSC: long spectral channel. The image is used with permission from Lydia
    Sauer, Christopher B. Komanski, Alexandra S. Vitale, Eric D. Hansen, and Paul S. Bernstein from
    their study titled `Fluorescence Lifetime Imaging Ophthalmoscopy (FLIO) in Eyes With Pigment
    Epithelial Detachments Due to Age-Related Macular Degeneration,` published in Invest.
    Ophthalmol. Vis. Sci. 2019;60(8):3054-3063, [DOI:
    https://doi.org/10.1167/iovs.19-26835](https://doi.org/10.1167/iovs.19-26835).
  </figcaption>
</figure>

<figure>
  <img src="https://docs.aireadi.org/img/retinal-flio/fig2.png" />
  <figcaption>
    Figure 2. Fundus autofluorescence and lifetime images from short- and long-spectral channels of
    an eye with subretinal hyperreflective material, which is indicated using white arrows. The
    image is used with permission from Lydia Sauer, Christopher B. Komanski, Alexandra S. Vitale,
    Eric D. Hansen, and Paul S. Bernstein from their study titled `Fluorescence Lifetime Imaging
    Ophthalmoscopy (FLIO) in Eyes With Pigment Epithelial Detachments Due to Age-Related Macular
    Degeneration,` published in Invest. Ophthalmol. Vis. Sci. 2019;60(8):3054-3063,
    [https://doi.org/10.1167/iovs.19-26835](https://doi.org/10.1167/iovs.19-26835).
  </figcaption>
</figure>


### Retinal OCT (Optical Coherence Tomography)

<figure>
  <img src="https://docs.aireadi.org/img/retinal-oct/fig2.jpg" />
  <figcaption>Figure 1. ONH Heidelberg Spectralis (Spec-ONH-RC-HR-OCT).</figcaption>
</figure>



<figure>
  <img src="https://docs.aireadi.org/img/retinal-oct/fig3.png" />
  <figcaption>
    Figure 2. Posterior pole Macula high-resolution OCT (Spec-PPole Mac-HR-61 lines-OCT) Heidelberg
    Spectralis
  </figcaption>
</figure>

### Retinal OCTA (Optical Coherence Tomography Angiography)
<figure>
  <img src="https://docs.aireadi.org/img/retinal-octa/fig1a.png" />
  <img src="https://docs.aireadi.org/img/retinal-octa/fig1b.png" />
  <figcaption>
    Figure 1. Topcon, Maestro2, Maestro2-Mac 6x6-360x360-(rep3)-OCTA, own source (UCSD), en face
    (superficial, deep, outer retina and choriocapillaris) and OCT B-scan.
  </figcaption>
</figure>

<figure>
  <img src="https://docs.aireadi.org/img/retinal-octa/fig2a.png" />
  <img src="https://docs.aireadi.org/img/retinal-octa/fig2b.png" />
  <figcaption>
    Figure 2. Topcon, Triton, Triton-Macula 6x6-OCTA, own source (UCSD), en face slabs (superficial,
    deep, outer retina, choriocapillaris) and Angio OCT B-scan.
  </figcaption>
</figure>

<figure>
  <img src="https://docs.aireadi.org/img/retinal-octa/fig3a.png" />
  <img src="https://docs.aireadi.org/img/retinal-octa/fig3b.png" />
  <figcaption>
    Figure 3. Topcon, Triton, Triton-Macula 12x12-OCTA, own source (UCSD), OCT flow cube and
    structural B-scan and en-face images.
  </figcaption>
</figure>

### Retinal Photography

<figure>
  <img src="https://docs.aireadi.org/img/retinal-photography/fig4.jpg" />
  <figcaption>
    Figure 1: Fundus photographs (50°) of patients with (a) and without (b) signs of diabetic
    retinopathy acquired with the hand-held Optomed Aurora fundus camera. Reference: Lupidi M,
    Danieli L, Fruttini D, et al. Artificial intelligence in diabetic retinopathy screening:
    clinical assessment using handheld fundus camera in a real-life setting. Acta Diabetol.
    2023;60(8):1083-1088. doi:10.1007/s00592-023-02104-0.
  </figcaption>
</figure>

<figure>
  <img src="https://docs.aireadi.org/img/retinal-photography/fig5.jpg" />
  <figcaption>
    Figure 2: Color fundus photos show different stages of diabetic retinopathy (DR). (a) No DR. (b)
    Mild non-proliferative DR. (c) Moderate non-proliferative DR. (d) Severe non-proliferative DR.
    (e) Proliferative DR.
  </figcaption>
</figure>


## File Structure

The file structure for the eye imaging data in the AI-READI dataset is as follows:

``` 
dataset
├── retinal_flio
│   ├── flio
│   │   └── heidelberg_flio
│   │       └── 0001
│   │           ├── 0001_flio_long_wavelength.dcm
│   │           └── ...
│   └── manifest.csv
├── retinal_oct
│   ├── structural_oct
│   │   ├── heidelberg_spectralis
│   │   │   └── 0001
│   │   │       └── 0001_spectralis_onh_rc_hr_oct.dcm
│   │   │       └── ...
│   │   ├── topcon_maestro2
│   │   │   └── 0001
│   │   │       └── 0001_maestro2_3d_macula_oct.dcm
│   │   │       └── ...
│   │   ├── topcon_triton
│   │   │   └── 0001
│   │   │       └── 0001_triton_macula_6x6_oct.dcm
│   │   │       └── ...
│   │   └── zeiss_cirrus
│   │       └── 0001
│   │           └── 0001_cirrus_disc_6x6_octa_oct.dcm
│   │           └── ...
│   └── manifest.csv
├──retinal_octa
│   ├── enface
│   │   ├── topcon_maestro2
│   │   │   └── 0001
│   │   │       └── 0001_maestro2_macula_6x6_enface.dcm
│   │   │       └── ...    
│   │   ├── topcon_triton
│   │   │   └── 0001
│   │   │       └── 0001_triton_macula_6x6_enface.dcm
│   │   └── zeiss_cirrus
│   │       └── 0001
│   │           └── 0001_cirrus_disc_6x6_octa_enface.dcm
│   │           └── ...
│   ├── flow_cube
│   │   ├── topcon_maestro2
│   │   │   └── 0001
│   │   │       └── 0001_maestro2_macula_6x6_flow_cube.dcm
│   │   ├── topcon_triton
│   │   │   └── 0001
│   │   │       └── 0001_triton_macula_6x6_flow_cube.dcm
│   │   └── zeiss_cirrus
│   │       └── 0001
│   │           └── 0001_cirrus_disc_6x6_octa_flow_cube.dcm
│   │           └── ...
│   ├── segmentation
│   │   ├── topcon_maestro2
│   │   │   └── 0001
│   │   │       └── 0001_maestro2_macula_6x6_segmentation.dcm
│   │   │       └── ...    
│   │   ├── topcon_triton
│   │   │   └── 0001
│   │   │       └── 0001_triton_macula_6x6_segmentation.dcm
│   │   │       └── ...
│   │   └── zeiss_cirrus
│   │       └── 0001
│   │           └── 0001_cirrus_disc_6x6_octa_segmentation.dcm
│   │           └── ...
│   └── manifest.csv
├──retinal_photography
│   ├── cfp
│   │   ├── icare_eidon
│   │   │   └── 0001
│   │   │       └── 0001_eidon_mosaic_cfp.dcm
│   │   │       └── ...
│   │   ├── optomed_aurora
│   │   │   └── 0001
│   │   │       └── 0001_optomed_mac_or_disk_centered_cfp.dcm
│   │   │       └── ...
│   │   ├── topcon_maestro2
│   │   │   └── 0001
│   │   │       └── 0001_maestro2_3d_macula_cfp.dcm
│   │   │       └── ...
│   │   └── topcon_triton
│   │       └── 0001
│   │           └── 0001_triton_macula_6x6_cfp.dcm
│   │           └── ...
│   ├── faf
│   │   └── icare_eidon
│   │       └── 0001
│   │           └── 0001_eidon_uwf_central_faf.dcm
│   │           └── ...
│   ├── ir
│   │   ├── heidelberg_spectralis
│   │   │   └── 0001
│   │   │       └── 0001_spectralis_onh_rc_hr_ir.dcm
│   │   │       └── ...
│   │   ├── icare_eidon
│   │   │   └── 0001
│   │   │       └── 0001_eidon_uwf_central_ir.dcm
│   │           └── ...
│   │   ├── topcon_maestro2
│   │   │   └── 0001
│   │   │       └── 0001_maestro2_macula_6x6_ir.dcm
│   │   │       └── ...
│   │   ├── topcon_triton
│   │   │   └── 0001
│   │   │       └── 0001_triton_macula_6x6_ir.dcm
│   │   │       └── ...
│   │   └── zeiss_cirrus
│   │       └── 0001
│   │           └── 0001_cirrus_disc_6x6_octa_ir.dcm
│   │           └── ...
│   └── manifest.csv
└── ...
```

## Authors and Institutions

AI-READI Consortium (details in the Article linked in the Source Information section)

## Source Information

Official Website: https://fairhub.io/datasets/2

Download Link: https://fairhub.io/datasets/2

Article Address: https://doi.org/10.1038/s42255-024-01165-x

Documentation Link: https://docs.aireadi.org/

Data Loader Tool Link: https://github.com/AI-READI/aireadi_loader 

Publication Date: 2024-11-08

## Citations

``` 
AI-READI Consortium. (2024). "AI-READI: rethinking data collection, preparation and
sharing for propelling AI-based discoveries in diabetes research and beyond."
Nature metabolism. https://doi.org/10.1038/s42255-024-01165-x
```
``` 
AI-READI Consortium. (2024). Flagship Dataset of Type 2 Diabetes from the
AI-READI Project (2.0.0) [Data set]. FAIRhub.
https://doi.org/10.60775/fairhub.2
```
