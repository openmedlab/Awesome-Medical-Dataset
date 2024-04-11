# Awesome-Medical-Dataset [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

🔥🔥🔥 Medical Dataset is very important for Medical Image Analysis. In this repository, we provide an up-to-date list of medical datasets.

## Table of Content

---

:book: **Contents**

- [Imaging](#Imaging)
  - [Whole Body (5)](#whole-body)
  - [Head and Neck (30)](#head-and-neck)
  - [Chest (24)](#chest)
  - [Abdomen (27)](#abdomen)
  - [Heart (6)](#heart)
  - [Bones (4)](#bones)
  - [Endoscopy (19)](#endoscopy)
  - [Retina (22)](#retina)
  - [Skin (6)](#skin)
  - [Microscopic imaging (22)](#microscopic-imaging)
- [Imaging and Text (22)](#Image-text-dataset)
- [Text (13)](#Text-dataset)

---

## Medical Image Datasets

### Whole Body

| Dataset                                                   | Task          | Description                                                         | Official Website                                                                                                        | Download Link                                                                       | Paper                                                                  | Publication Date | Challenge          |
|:----------------------------------------------------------|:--------------|:--------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------|:-----------------------------------------------------------------------|:-----------------|:-------------------|
| [CT-ORG](./resources/CT-ORG.md)                           | Segmentation  | 3D CT, 140 Cases, 6 Categories of Organ Segmentation.               | [Github](https://github.com/bbrister/ctOrganSegmentation)                                                               | [TCIA](https://wiki.cancerimagingarchive.net/pages/viewpage.action?pageId=61080890) | [Scientific Data](https://www.nature.com/articles/s41597-020-00715-8)  | 2020             | -                  |
| [AutoPET](./resources/Auto-PET.md)                        | Segmentation  | 3D PET-CT, 1214 Cases, 1 Category of Whole Body Tumor Segmentation. | [Grand Challenge 1](https://autopet.grand-challenge.org/), [Grand Challenge 2](https://autopet-ii.grand-challenge.org/) | [TCIA](https://wiki.cancerimagingarchive.net/pages/viewpage.action?pageId=93258287) | [Scientific Data](https://www.nature.com/articles/s41597-022-01718-3)  | 2022-04          | MICCAI'2022 & 2023 | 
| [TotalSegmentator](./resources/TotalSegmentator.md)       | Segmentation  | 3D CT, 1204 Cases, 104 Categories of Whole Body Organ Segmentation. | [Github](https://github.com/wasserth/TotalSegmentator)                                                                  | [Zenodo](https://zenodo.org/record/6802614)                                         | [RSNA](https://pubs.rsna.org/doi/10.1148/ryai.230024)                  | 2022-07          | -                  |
| [TotalSegmentator V2](./resources/TotalSegmentator_v2.md) | Segmentation  | 3D CT, 1228 Cases, 117 Categories of Whole Body Organ Segmentation. | [Github](https://github.com/wasserth/TotalSegmentator)                                                                  | [Zenodo](https://doi.org/10.5281/zenodo.6802613)                                    | [RSNA](https://pubs.rsna.org/doi/10.1148/ryai.230024)                  | 2023             | -                  |
| [ULS](./resources/ULS.md)                                 | Segmentation  | 3D CT, 38842 Cases, 1 Category of Whole Body Tumor Segmentation.    | [Grand Challenge](https://uls23.grand-challenge.org/)                                                                   | [Grand Challenge](https://uls23.grand-challenge.org/datasets/)                      | -                                                                      | 2023-10          | -                  |

### Head and Neck

| Dataset                                               | Task                        | Description                                                                            | Official Website                                                                    | Download Link                                                                              | Paper                                                                                                                                                                      | Publication Date | Challenge                      |
|:------------------------------------------------------|:----------------------------|:---------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------------|:-------------------------------|
| [L2R-OASIS](./resources/L2R-OASIS.md)                 | Registration & Segmentation | 3D MRI, 416 Cases, 35 Categories of Brain Segmentation and Registration                | [Grand Challenge](https://learn2reg.grand-challenge.org/Datasets/)                  | [Project Page](https://www.oasis-brains.org/#data)                                         | [Cognitive Neuroscience](https://dash.harvard.edu/bitstream/handle/1/33896768/Buckner_OpenAccess.pdf?sequence=2)                                                           | 2007             | -                              |
| [DDTI](./resources/DDTI.md)                           | Segmentation                | 2D Ultrasound, 637 Cases, 1 Category of Thyroid Nodule Segmentation                    | [Project Page](http://cimalab.intec.co/applications/thyroid/)                       | [Project Page](http://cimalab.intec.co/applications/thyroid/)                              | [SPIE'2015](https://www.spiedigitallibrary.org/conference-proceedings-of-spie/9287/92870W/An-open-access-thyroid-ultrasound-image-database/10.1117/12.2073532.short?SSO=1) | 2015-01          | -                              |
| [Ultrasound Nerve Segmentation](./resources/UNS.md)   | Segmentation                | 2D Ultrasound, 11143 Cases, 1 Category of Cervical Nerve Segmentation                  | [Kaggle](https://kaggle.com/competitions/ultrasound-nerve-segmentation)             | [Kaggle](https://www.kaggle.com/c/ultrasound-nerve-segmentation/data)                      | -                                                                                                                                                                          | 2016-05          | Kaggle                         |
| [BraTS-TCGA-LGG](./resources/BraTS-TCGA-LGG.md)       | Segmentation                | 3D MRI, 65 Cases, 3 Categories of Low Grade Glioma (LGG) Segmentation                  | [TCIA](https://www.cancerimagingarchive.net/analysis-result/brats-tcga-lgg/)        | [TCIA](https://www.cancerimagingarchive.net/analysis-result/brats-tcga-lgg/)               | [Scientific Data](https://www.nature.com/articles/sdata2017117)                                                                                                            | 2017             | BRATS2015                      |
| [BraTS-TCGA-GBM](./resources/BraTS-TCGA-GBM.md)       | Segmentation                | 3D MRI, 102 Cases, 3 Categories of Glioblastoma Multiforme (GBM) Segmentation          | [TCIA](https://www.cancerimagingarchive.net/analysis-result/brats-tcga-gbm/)        | [TCIA](https://www.cancerimagingarchive.net/analysis-result/brats-tcga-gbm/)               | [Scientific Data](https://www.nature.com/articles/sdata2017117)                                                                                                            | 2017             | BRATS2015                      |
| [PDDCA](./resources/PDDCA.md)                         | Segmentation                | 3D CT, 48 Cases, 9 Categories of Head and Neck Organs Segmentation                     | [ImagEngLab](https://www.imagenglab.com/newsite/pddca/)                             | [ImagEngLab](https://www.imagenglab.com/newsite/pddca/)                                    | [Medical Physics](https://aapm.onlinelibrary.wiley.com/doi/10.1002/mp.12197)                                                                                               | 2017-03          | -                              |
| [iSeg](./resources/iSeg.md)                           | Segmentation                | 3D MRI, 13 Cases, 3 Categories of Brain Tissue Segmentation                            | [Project Page](https://iseg2019.web.unc.edu/)                                       | [Project Page](https://iseg2019.web.unc.edu/)                                              | [TMI'2021](https://doi.org/10.1109/TMI.2021.3055428)                                                                                                                       | 2019             | MICCAI'2017 & 2019             |
| [MSD Hippocampus](./resources/MSD_Hippocampus.md)     | Segmentation                | 3D MRI, 394 Cases, 2 Categories of Hippocampus Segmentation                            | [MSD](http://medicaldecathlon.com/)                                                 | [Google Drive](https://drive.google.com/drive/folders/1HqEgzS8BV2c7xYNrZdEAnrHk7osJJ--2)   | [Nature Communication](https://www.nature.com/articles/s41467-022-30695-9)                                                                                                 | 2019-02          | Medical Segmentation Decathlon |
| [WMH](./resources/WMH.md)                             | Segmentation                | 3D MRI, 170 Cases, 1 Category of White Matter Hyperintensity Segmentation              | [Project Page](https://dataverse.nl/dataset.xhtml?persistentId=doi:10.34894/AECRSD) | [Project Page](https://dataverse.nl/dataset.xhtml?persistentId=doi:10.34894/AECRSD)        | [TMI'2019](https://ieeexplore.ieee.org/document/8669968)                                                                                                                   | 2019-11          | -                              |
| [TN-SCUI2020](./resources/TN-SCUI2020.md)             | Segmentation                | 2D Ultrasound, 4554 Cases, 1 Category of Thyroid Nodule Segmentation                   | [Grand Challenge](https://tn-scui2020.grand-challenge.org/Home/)                    | [Grand Challenge](https://tn-scui2020.grand-challenge.org/Source_links/)                   | [Zenodo](https://zenodo.org/records/3715942#.XvBr7GgzaUk)                                                                                                                  | 2020-05          | MICCAI'2020                    |
| [BraTS21](./resources/BraTS2021.md)                   | Segmentation                | 3D MRI, 2040 Cases, 3 Categories of Glioma Segmentation                                | [Synapse](https://www.synapse.org/#!Synapse:syn25829067/wiki/610863)                | [Synapse](https://www.synapse.org/#!Synapse:syn51514105)                                   | [ArXiv'2021](https://arxiv.org/abs/2107.02314)                                                                                                                             | 2021-07          | RSNA-ASNR-MICCAI'2021          |
| [FeTA 2022](./resources/FeTA.md)                      | Segmentation                | 3D MRI, 280 Cases, 7 Categories of Infant Brain Tissue Segmentation                    | [Grand Challenge](https://feta.grand-challenge.org/)                                | [Grand Challenge](https://feta.grand-challenge.org/data-download/)                         | [Scientific Data](https://www.nature.com/articles/s41597-021-00946-3)                                                                                                      | 2021             | MICCAI'2021 & 2022             |
| [ATLAS v2.0 (ISLES 2022)](./resources/ATLASv2.0.md)   | Segmentation                | 3D MRI, 1271 Cases, 1 Category of Lesions After Stroke Segmentation                    | [Grand Challenge](https://atlas.grand-challenge.org/)                               | [Project Page](http://fcon_1000.projects.nitrc.org/indi/retro/atlas.html)                  | [Scientific Data](https://www.nature.com/articles/s41597-022-01401-7)                                                                                                      | 2021-12          | MICCAI'2022                    |
| [cSeg 2022](./resources/cSeg2022.md)                  | Segmentation                | 3D MRI, 13 Cases, 3 Categories of Brain Tissue Segmentation                            | [Project Page](https://tarheels.live/cseg2022/)                                     | [Project Page](https://tarheels.live/cseg2022/data/)                                       | -                                                                                                                                                                          | 2022-04          | MICCAI'2022                    |
| [HECKTOR](./resources/HECKTOR_2022.md)                | Segmentation                | 3D PET-CT, 882 Cases, 2 Categories of Tumor and Lymph Node Segmentation                | [Grand Challenge](https://hecktor.grand-challenge.org/)                             | [Grand Challenge](https://hecktor.grand-challenge.org/Data/)                               | [Springer Link](https://link.springer.com/book/10.1007/978-3-031-27420-6)                                                                                                  | 2022-06          | MICCAI'2022                    |
| [INSTANCE 2022](./resources/INSTANCE_2022.md)         | Segmentation                | 3D CT, 200 Cases, 1 Category of Intracranial Hemorrhage Segmentation                   | [Grand Challenge](https://instance.grand-challenge.org/)                            | [Grand Challenge](https://instance.grand-challenge.org/Dataset/)                           | [Biomedical and Health Informatics ](https://ieeexplore.ieee.org/document/9511297)                                                                                         | 2022-04          | MICCAI'2022                    |
| [ISLES22](./resources/ISLES22.md)                     | Segmentation                | 3D MRI, 400 Cases, 1 Category of Ischemic Stroke Lesion Segmentation                   | [Grand Challenge](https://isles22.grand-challenge.org/)                             | [Zenodo](https://doi.org/10.5281/zenodo.7153326)                                           | [Scientific Data](https://www.nature.com/articles/s41597-022-01875-5)                                                                                                      | 2022-05          | MICCAI'2022                    |
| [Teeth3DS](./resources/Teeth3DS.md)                   | Segmentation                | 3D IOS, 1800 Cases, 32 Categories of Teeth Segmentation                                | [Github](https://github.com/DCBIA-OrthoLab/3DTeethSeg22_challenge)                  | [OSF](https://osf.io/xctdy/)                                                               | [ArXiv'2022](https://arxiv.org/pdf/2210.06094)                                                                                                                             | 2022-10          | MICCAI'2022                    |
| [TN3K](./resources/TN3K.md)                           | Segmentation                | 2D Ultrasound, 3494 Cases, 1 Category of Thyroid Nodule Segmentation                   | [Github](https://github.com/haifangong/TRFE-Net-for-thyroid-nodule-segmentation)    | [Github](https://github.com/haifangong/TRFE-Net-for-thyroid-nodule-segmentation)           | [ISBI'2021](https://ieeexplore.ieee.org/abstract/document/9434087/)                                                                                                        | 2021-05          | ISBI'2021                      |
| [TG3K](./resources/TG3K.md)                           | Segmentation                | 2D Ultrasound, 3585 Cases, 1 Category of Thyroid Nodule Segmentation                   | [Github](https://github.com/haifangong/TRFE-Net-for-thyroid-nodule-segmentation)    | [Github](https://github.com/haifangong/TRFE-Net-for-thyroid-nodule-segmentation)           | [Computers in Biology and Medicine](https://www.sciencedirect.com/science/article/pii/S0010482522010976)                                                                   | 2022-12          | ISBI'2021                      |
| [HaN-Seg](./resources/HaN-Seg.md)                     | Segmentation                | 3D CT & MRI, 42 Cases, 30 Categories of Head and Neck Organs-at-Risk Segmentation      | [Grand Challenge](https://han-seg2023.grand-challenge.org/)                         | [Zenodo](https://zenodo.org/record/7442914#.ZBtfBHbMJaQ)                                   | [Medical Physics](https://aapm.onlinelibrary.wiley.com/doi/10.1002/mp.16197)                                                                                               | 2023-01          | -                              |
| [SMILE-UHURA 2023](./resources/SMILE-UHURA%202023.md) | Segmentation                | 3D 7T High Resoulution MRI, 14 Cases, 1 Category of Cerebral Artery Segmentation       | [Synapse](https://www.synapse.org/#!Synapse:syn47164761/wiki/620033)                | [Synapse](https://www.synapse.org/#!Synapse:syn47164761/wiki/620033)                       | -                                                                                                                                                                          | 2023-03          | ISBI'2023                      |
| [ToothFairy](./resources/ToothFairy.md)               | Segmentation                | 3D CBCT, 443 Cases, 1 Category of Inferior Alveolar Nerve Segmentation                 | [Grand Challenge](https://toothfairy.grand-challenge.org/toothfairy/)               | [Project Page](https://ditto.ing.unimore.it/toothfairy/)                                   | [CVPR'2022](https://openaccess.thecvf.com/content/CVPR2022/html/Cipriano_Improving_Segmentation_of_the_Inferior_Alveolar_Nerve_Through_Deep_Label_CVPR_2022_paper.html)    | 2023-03          | MICCAI'2023                    |
| [SegRap 2023](./resources/SegRap2023.md)              | Segmentation                | 3D CT, 200 Cases, 47 Categories of Head and Neck Organs-at-Risk Segmentation           | [Grand Challenge](https://segrap2023.grand-challenge.org/)                          | [Grand Challenge](https://segrap2023.grand-challenge.org/dataset/)                         | [ArXiv'2023](https://arxiv.org/abs/2312.09576)                                                                                                                             | 2023-04          | MICCAI'2023                    |
| [CAS2023](./resources/CAS2023.md)                     | Segmentation                | 3D MRI, 100 Cases, 1 Category of Cerebral Artery Segmentation                          | [CodaLab](https://codalab.lisn.upsaclay.fr/competitions/9804)                       | [CodeLab](https://codalab.lisn.upsaclay.fr/competitions/9804#participate-get_starting_kit) | -                                                                                                                                                                          | 2023-04          | MICCAI'2023                    |
| [CrossMoDA 2023](./resources/CrossMoDA2023.md)        | Segmentation                | 3D MRI, 983 Cases, 3 Categories of Vestibular Schwannoma (VS) and Cochlea Segmentation | [Project Page](https://crossmoda-challenge.ml/)                                     | [Synapse](https://www.synapse.org/#!Synapse:syn51236108/files/)                            | [MIA'2023](https://www.sciencedirect.com/science/article/pii/S1361841522002560)                                                                                            | 2023-04          | MICCAI'2023                    |
| [BraTS2023-SSA](./resources/BraTS2023-SSA.md)         | Segmentation                | 3D MRI, 105 Cases, 3 Categories of Glioma Segmentation in Africa                       | [Synapse](https://www.synapse.org/#!Synapse:syn51156910/wiki/622556)                | [Synapse](https://www.synapse.org/#!Synapse:syn51514109)                                   | [ArXiv'2023](https://arxiv.org/abs/2305.19369)                                                                                                                             | 2023-05          | ASNR-MICCAI'BRATS2023          |
| [BraTS2023-MEN](./resources/BraTS2023-MEN.md)         | Segmentation                | 3D MRI, 1650 Cases, 3 Categories of Meningioma Segmentation                            | [Synapse](https://www.synapse.org/#!Synapse:syn51156910/wiki/622353)                | [Synapse](https://www.synapse.org/#!Synapse:syn51514106)                                   | [ArXiv'2023](https://arxiv.org/pdf/2305.07642)                                                                                                                             | 2023-05          | ASNR-MICCAI'BRATS2023          |
| [BraTS2023-PED](./resources/BraTS2023-PED.md)         | Segmentation                | 3D MRI, 228 Cases, 3 Categories of Pediatrics Glioma Segmentation                      | [Synapse](https://www.synapse.org/#!Synapse:syn51156910/wiki/622461)                | [Synapse](https://www.synapse.org/#!Synapse:syn51514108)                                   | [ArXiv'2023](https://arxiv.org/abs/2305.17033)                                                                                                                             | 2023-05          | ASNR-MICCAI'BRATS2023          |
| [BraTS2023-MET](./resources/BraTS2023-MET.md)         | Segmentation                | 3D MRI, 328 Cases, 3 Categories of Brain Metastasis Segmentation                       | [Synapse](https://www.synapse.org/#!Synapse:syn51156910/wiki/622553)                | [Synapse](https://www.synapse.org/#!Synapse:syn51514107)                                   | [ArXiv'2023](https://arxiv.org/abs/2306.00838)                                                                                                                             | 2023-06          | ASNR-MICCAI'BRATS2023          |

### Chest

[ATM22](./resources/ATM22.md) (3D CT, 500 Cases, 1 Category)

[AIIB23](./resources/AIIB23.md) (3D CT, 312 Cases, 1 Category)

[Parse 2022](./resources/Parse.md) (3D CT, 200 Cases, 1 Category)

[LUNA16](./resources/LUNA16.md) (3D CT, 888 Cases, 1 Category of Lung Nodule Detection)

[SEG.A.](./resources/SEG.A.md) (3D CTA, 56 Cases, 1 Category)

[SegTHOR](./resources/SegTHOR.md) (3D CT, 60 Cases, 4 Categories)

[FUMPE](./resources/FUMPE.md) (3D CT, 35 Cases, 1 Category)

[TDSC-ABUS2023](./resources/TDSC-ABUS2023.md) (3D Ultrasound, 200 Cases, 1 Category)

[LNDb](./resources/LNDb.md) (3D CT, 294 Cases, 1 Category)

[LNQ 2023](./resources/LNQ2023.md) (3D CT, 513 Cases, 1 Category)

[MSD Lung Tumours](./resources/MSD_Lung_Tumours.md) (3D CT, 96 Cases, 1 Category)

[PleThora](./resources/PleThora.md) (3D CT, 402 Cases,2 Categories for pleural effusion and thoracic segmentation)

[BUSI](./resources/BUSI.md) (3D Ultrasound, 780 Cases, 3 Categories)

[MVSeg-3DTEE 2023](./resources/MVSeg-3DTEE.md) (3D Ultrasound, 175 Cases, 2 Categories for mitral valve segmentation)

[Breast Ultrasound Dataset B](./resources/Breast_Ultrasound_DatasetB.md) (2D Ultrasound, 163 Cases, 1 Category)

[胸部 X 线成像(肺炎)/ Chest X-Ray Imaging_(Pneumonia)](./resources/ChestX-RayImaging_Pneumonia.md) (2D X-ray, 5856 Cases, 2 Categories)

[COVID-19 CHEST X-RAY DATABASE](./resources/COVID-19_CHEST_X-RAY_DATABASE.md) (2D X-ray, 3886 Cases, 3 Categories)

[Chest X-ray PD Dataset](./resources/ChestX-rayPDDataset.md) (2D X-Ray, 4575 Cases, 3 Categories)

[COVIDGR](./resources/COVIDGR.md) (2D X-Ray, 852 Cases, 2 Categories)

[Shenzhen chest X-ray set](./resources/Shenzhen_chest_X-ray.md) (2D X-Ray, 662 cases, 2 Categories for tuberculosis classification)

[COVID_CT_COVID-CT](./resources/COVID_CT_COVID-CT.md) (2D CT, 746 Cases, 2 Categories)

[COVID-19-CT SCAN IMAGES](./resources/COVID-19-CT_SCAN_IMAGES.md) (2D CT, 1400 Cases, 2 Categories pneumonia classification)

[Chest CT-Scan images](./resources/ChestCT-Scan_images.md) (2D CT, 1000 Cases, 4 Categories)

[SARS-COV-2 Ct-Scan](./resources/SARS-COV-2.md) (2D CT, 2482 Cases, 2 Categories)

### Abdomen

[FLARE 2023](./resources/FLARE2023.md) (3D CT, 4500 Cases, 14 Categories)

[FLARE 2022](./resources/FLARE2022.md) (3D CT, 2300 Cases, 13 Categories)

[FLARE 2021](./resources/FLARE2021.md) (3D CT, 511 Cases, 4 Categories)

[AMOS 2022](./resources/AMOS.md) (3D CT&MRI, 600 Cases, 15 Categories)

[WORD](./resources/WORD.md) (3D CT, 150 Cases, 16 Categories)

[AbdomenCT-1K](./resources/AbdomenCT-1K.md) (3D CT, 1112 Cases, 4 Categories)

[BTCV](./resources/BTCV.md) (3D CT, 50 Cases, 13 Categories)

[BTCV Cervix](./resources/BTCV_Cervix.md) (3D CT, 50 Cases, 4 Categories)

[LiTS](./resources/LiTS.md) (3D CT, 201 Cases, 2 Categories)

[KiTS23](./resources/KiTS23.md) (3D CT, 599 Cases, 3 Categories)

[KiTS21](./resources/KiTS21.md) (3D CT, 400 Cases, 3 Categories)

[KiTS19](./resources/KiTS19.md) (3D CT, 300 Cases, 2 Categories)

[KiPA22](./resources/KiPA22.md) (3D CTA, 130 Cases, 4 Categories)

[CHAOS](./resources/CHAOS.md) (3D CT&MRI, 40 Cases, 4 Categories)

[SPPIN](./resources/SPPIN.md) (3D MRI, 111 Cases, 1 Category)

[ATLAS (MICCAI2023)](./resources/ATLAS.md) (3D CE-MRI, 90 Cases, 2 Categories)

[3D-IRCADB](./resources/3D-IRCADB.md) (3D CT, 22 Cases, 40 Categories)

[MSD Pancreas Tumour](./resources/MSD_Pancreas_Tumour.md) (3D CT, 420 Cases, 2 Categories)

[MSD Hepatic Vessel](./resources/MSD_Hepatic_Vessel.md) (3D CT, 443 Cases, 2 Categories)

[MSD Spleen](./resources/MSD_Spleen.md) (3D CT, 61 Cases, 1 Category)

[MSD Colon Cancer](./resources/MSD_Colon_Cancer.md) (3D CT, 190 Cases, 1 Category)

[MSD Prostate](./resources/MSD_Prostate.md) (3D MR, 48 Cases, 2 Categories)

[PI-CAI](./resources/PI-CAI.md) (3D MR, 1500 Cases, 1 Category)

[MOOD2023](./resources/MOOD2023.md) (3D, CT&MR, 1300 Cases)

[LLD-MMRI2023](./resources/LLD-MMRI2023.md) (3D, MRI, 394 Cases, Liver Lesion Detection)

[UW-Madison GI Tract Image Segmentation](./resources/UW-Madison_GI_Tract_Image_Segmentation.md) (2D, MRI, 38496 Cases, 3 Categories gastrointestinal tract segmentation)

[QUBIQ2021](./resources/QUBIQ2021.md) (3D, CT, 90 Cases, 2 Categories of Pancreas & Pancreatic Lesions Segmentation)

### Heart

[LAScarQS 2022](./resources/LAScarQS_2022.md) (3D MRI, 194 Cases, 2 Categories)

[MyoPS 2020](./resources/MyoPS_2020.md) (3D MRI, 45 Cases, 5 Categories)

[MM-WHS](./resources/MM-WHS.md) (3D CT/MRI, 120 Cases, 7 Categories)

[ACDC](./resources/ACDC.md) (3D MRI, 150 Cases, 3 Categories)

[MSD Cardiac](./resources/MSD_Cardiac.md) (3D MRI, 30 Cases, 1 Category)

[CMRxMotion](./resources/CMRxMotion.md) (3D MRI, 360 Cases, 3 Categories)

### Bones

[VerSe](./resources/VerSe.md) (3D CT, 374 Cases, 26 Categories)

[SPIDER](./resources/SPIDER.md) (3D MR, 544 Cases, 19 Categories)

[CTSpine1K](./resources/CTSpine1K.md) (3D CT, 1005 Cases, 25 Categories)

[CTPelvic1K](./resources/CTPelvic1K.md) (3D CT, 1184 Cases, 4 Categories)

### Endoscopy

[Kvasir-SEG](./resources/Kvasir-SEG.md) (2D, Endoscopy, 1160 Cases, 1 Category)

[Kvasir-Capsule](./resources/Kvasir-Capsule.md) (2D, Endoscopy, 4741504 Cases, 14 Categories)

[CVC-ClinicDB](./resources/CVC-ClinicDB.md) (2D, Endoscopy, 612 Cases, 1 Category)

[EndoMapper](./resources/EndoMapper.md) (2D, Endoscopy Video, 59 Cases)

[EndoSLAM](./resources/EndoSLAM.md) (2D, Endoscopy, 64577 Cases)

[m2caiseg](./resources/m2caiseg.md) (2D, Endoscopy, 307 Cases, 19 Categories)

[EAD 2019](./resources/EAD2019.md) (2D, Endoscopy, 2991 Cases, 7 Categories)

[LDPolypVideo](./resources/LDPolypVideo.md) (2D, Endoscopy, 861400帧, 1 Category)

[LIMUC](./resources/LIMUC.md) (2D, Endoscopy, 11276, 4 Categories)

[SUN Colonoscopy Video](./resources/SUN_Colonoscopy_Video.md) (2D, Endoscopy, 158,690 Cases, 100 Categories)

[Colonoscopic](./resources/Colonoscopic.md) (2D, Endoscopy, 152 Cases, 3 Categories)

[Sinus Surgery Endoscopic Image Datasets](./resources/Sinus_Surgery.md) (2D Rhinoscopy, 9003 Cases, 1 Category)

[The Nerthus Dataset](./resources/Nerthus.md) (2D Endoscopy, 5525 Cases, Classification of 4 Categories of intestinal cleansing levels)

[CholecT45 Dataset](./resources/CholecT45.md) (2D Endoscopy, 90489 Cases, 128 Categories of cholecystectomy surgery action recognition)

[CholecSeg8k](./resources/CholecSeg8k.md) (2D Endoscopy, 8080 Cases, 13 Categories of Cholecystectomy Surgery Semantic segmentation)

[FetReg 2021 Task1](./resources/FetReg.md) (2D Fetoscope, 2718 Cases, 3 Categories of Blood vessels, Fetus, Surgical Tools Segmentation)

[Endoscopic Bladder Tissue Classification Dataset](./resources/Endoscopic_Bladder_Tissue_Classification.md) (2D Endoscopy, 1754 Cases, 4 Categories of Cystoscopy Tissue Classification)

[Surgical scene segmentation](./resources/Surgical_Scene_Segmentation.md) (2D Endoscopy, 9156 Cases, 32 Categories of Surgery Scene Segmentation)

[SARAS-ESAD](./resources/SARAS-ESAD.md) (2D Endoscopy, 33398 Cases, 21 Categories of Surgical Action Recognition)

### Retina

[ODIR-5K](./resources/ODIR-5K.md) (2D retinal images, 5000 Cases, 8 Categories)

[RFMiD 2.0](./resources/RFMiD.md) (2D retinal images, 3200 Cases, 45 Categories)

[Multi-Label Retinal Diseases](./resources/Multi-LabelRetinalDiseases.md) (2D retinal images, 2451 Cases, 20 Categories of Eye Diseases Classification)

[STARE](./resources/STARE.md) (2D retinal images, 20 Cases, 1 Category)

[DRIVE](./resources/DRIVE.md) (2D retinal images, 40 Cases, 1 Category)

[CHASE](./resources/CHASE.md) (2D retinal images, 28 Cases, 1 Category)

[HRF](./resources/HRF.md) (2D retinal images, 45 Cases, 1 Category)

[IDRID](./resources/IDRID.md) (2D retinal images, 81 Cases, 5 Categories)

[ORVS](./resources/ORVS.md) (2D retinal images, 49 Cases, 1 Category)

[LES-AV](./resources/LES-AV.md) (2D retinal images, 22 Cases, 1 Category)

[PALM19](./resources/PALM19.md) (2D retinal images, 1200 Cases, 1 Category)

[RITE](./resources/RITE.md) (2D retinal images, 40 Cases, 1 Category)

[Retinal image quality assessment dataset](./resources/Retinal_QA.md) (2D retinal images, 216 Cases, 3 Categories of image quality evaluation)

[DRISHTI-GS](./resources/DRISHTI-GS.md) (2D retinal images, 101 Cases, 2 Categories of Optic Cup and Optic Disc Segmentation)

[Retina](./resources/Retina.md) (2D retinal images, 601 Cases, 4 Categories of Cataracts, Glaucoma Retinopathy)

[Eyepacs](./resources/Eyepacs.md) (2D retinal images, 35126 Cases, 5 Categories of Diabetic Retinopathy Grading)

[Messidor-2](./resources/Messidor-2.md) (2D retinal images, 1748 Cases, 2 Categories of Diabetic Retinopathy Classification)

[OCTA-500](./resources/OCTA-500.md) (2D OCT , 500 Cases, 1 Category)

[ROSE](./resources/ROSE.md) (2D OCT, 229 Cases, 1 Category)

[Retinal OCT-C8](./resources/Retinal_OCT-C8.md) (2D OCT, 24000 Cases, 8 Categories)

[RETOUCH](./resources/RETOUCH.md) (3D OCT, 112例, 3 Categories)

[OCT 2017](./resources/OCT2017.md) (2D OCT, 35126 Cases, 4 Categories of Eye Disease Classification)

### Skin

[ISIC 2017](./resources/ISIC2017.md) (2D dermoscopic images, 2750 Cases, 1 Category)

[ISIC 2020](./resources/ISIC2020.md) (2D dermoscopic images，33126 Cases，2 Categories)

[MED-NODE](./resources/MED-NODE.md) (2D dermoscopic images, 170 Cases, 2 Categories)

[PED-UFES-20](./resources/PED-UFES-20.md) (2D dermoscopic images, 2298 Cases, 6 Categories)

[PH²](./resources/PH2.md) (2D dermoscopic images, 200 Cases, 2 Categories)

[Web-scraped Skin Image](./resources/Web-scraped_Skin_Image.md) (2D dermoscopic images, 804 Cases, 6 Categories of Dermatology Classification)

### Microscopic imaging

[NeurIPS 2022 Cell Seg](./resources/NeurIPS2022CellSeg.md) (2D Microscopic imaging, 3022 Cases, 1 Category)

[Malignant Lymphoma Classification](./resources/MalignantLymphomaClassification.md) (2D Pathological sections, 374 Cases, 3 Categories)

[BioMediTech](./resources/BioMediTech.md) (2D Cell imaging, 1862 Cases, 4 Categories)

[GlaS](./resources/GlaS.md) (2D Pathological Images, 165 Cases, 1 Category)

[LC25000](./resources/LC25000.md) (2D Pathological Images, 25000 Cases, 5 Categories)

[CoNIC2022](./resources/CoNIC2022.md) (2D Pathological Images, 4981 Cases, 7 Categories of Segmentation of Nuclei within Tissues)

[MoNuSeg](./resources/MoNuSeg.md) (2D Microscopic imaging, 53 Cases, 1 Category of Nucleus Segmentation)

[Corneal Nerve Tortuosity](./resources/Corneal_Nerve_Tortuosity.md) (2D Microscopic imaging, 30 Cases, 3 Categories of Degree of Corneal Nerve Distortion)

[Corneal Nerve](./resources/Corneal_Nerve.md) (2D Microscopic imaging, 90 Cases, 2 Categories of Corneal Abnormality Classification)

[CORN](./resources/CORN.md) (2D Microscopic imaging，1698 Cases, 1 Category of Corneal Nerve Segmentation)

[HuSHeM](./resources/HuSHeM.md) (2D Microscopic imaging, 216 Cases, 4 Categories of Sperm Classification)

[Malaria Cell Images](./resources/Malaria.md) (2D Microscopic imaging, 27558 Cases, 2 Categories of Malaria Classification)

[DigestPath2019](./resources/DigestPath2019.md) (2D Pathological imaging, 250 Cases, 1 Category of Digestive System Pathology Segmentation and Detection)

[ICIAR 2018 BACH Task1](./resources/ICIAR_2018_BACH_Task1.md) (2D Histology imaging, 400 Cases, 4 Categories of Breast Cancer Classification)

[ICIAR 2018 BACH Task2](./resources/ICIAR_2018_BACH_Task2.md) (2D Histology imaging, 30 Cases, 3 Categories of Breast Cancer Segmentation)

[Complete Blood Count](./resources/CompleteBloodCount.md) (2D Blood Smear, 360 Cases, 3 Categories of Blood Cell Count)

[ANHIR](./resources/ANHIR.md) (2D Pathological imaging, 481 Cases, Pathological image lung lobes and breast tissue registration)

[SICAPv2](./resources/SICAPv2.md) Prostate Pathology Segmentation Dataset (2D Pathological imaging, 18783 Cases, 4 Categories of Prostate Cancer Grade)

[ICPR-HEp-2](./resources/ICPR-HEp-2.md) (2D Cell Fluorescence Microscopy imaging, 14K, 6 Categories of Cell Classification)

[Bone Marrow Cytomorphology](./resources/BoneMarrowCytomorphology.md) (2D Pathological imaging, 171,375 Cases, 21 Categories of Bone Marrow Cell Morphological Classification)

[PatchCamelyon](./resources/PatchCamelyon.md) (2D Pathological imaging, 327,680 Cases, 2 Categories of Breast Cancer Metastasis Classification)

[Leukemia](./resources/Leukemia.md) (2D Microscopic imaging, 1867 Cases, 2 Categories of Leukemia Cell Classification)

## Image text dataset

[VQA-RAD](./resources/VQA-RAD.md) (VQA, 3515  Cases QA Pair)

[SLAKE](./resources/SLAKE.md) (VQA, 14028  Cases QA Pair)

[PathVQA](./resources/PathVQA.md) (VQA, 32799 Cases QA Pair)

[ROCOV2](./resources/ROCOV2.md) (caption, 80080  Cases image-caption Pair)

[ImageClef-2019-VQA-Med](./resources/ImageClef-2019-VQA-Med.md) (VQA, 15292  Cases QA Pair)

[RP3D-Caption](./resources/RP3D-Caption.md) (caption, 69523 Cases image-caption Pair)

[Montgomery County CXR Set](./resources/MontgomeryCounty.md) (2D X-Ray, 138例, 2 Categories of CXR Image Abnormality Diagnosis)

[PMC-OA](./resources/PMC-OA.md) (VQA, 1.6M QA Pair)

[MMMU Health&Medicine](./resources/MMMU_Health&Medicine.md) (VQA, 1752 Cases QA Pair)

[MedICaT](./resources/MedICaT.md) (VQA, 217060 Cases QA Pair)

[CT-RATE](./resources/CT-RATE.md) chest CT and its radiology diagnostic report data set (Caption, 47149 Cases)

[Quilt-1M](./resources/Quilt-1M.md) Visual-Language Histopathology Dataset (Caption, 768826 Cases)

## Text dataset

[MedQA](./resources/MedQA.md) (QA, 61,097 Cases QA Pair)

[MedMCQA](./resources/MedMCQA.md) (QA, 193,155 Cases QA Pair)

[PubMedQA](./resources/PubMedQA.md) (QA, 1000 Cases Expert annotation QA Pair)

[HealthSearchQA](./resources/HealthSearchQA.md) (QA, 3173 Cases QA Pair)

[webMedQA](./resources/webMedQA.md) (QA, 63,284 Cases QA Pair)

[LiveQA](./resources/LiveQA.md) (QA, 634例 QA Pair)

[CMExam](./resources/CMExam.md) (QA, 68K Cases QA Pair)

[CMB](./resources/CMB.md) (QA, 270K Cases QA Pair)

[MedDialog-CN](./resources/MedDialog-CN.md) (QA, 1.1M Cases QA Pair)

[Chinese Medical Dialogue Dataset](./resources/ChineseMedicalDialogueDataset.md) (QA, 792K Cases QA Pair)

[cMedQA](./resources/cMedQA.md) v2.0 (QA, 108K Cases QA Pair)

[Huatuo-26M](./resources/Huatuo-26M.md) (QA, 26M Cases QA Pair)

[ShenNong-TCM-Dataset/EB](./resources/ShenNong-TCM.md) (QA, 113K Cases QA Pair)

[MedBench](./resources/MedBench.md) (QA, 113K Cases QA Pair)











