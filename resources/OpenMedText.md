# OpenMedText

## Dataset Information

A comprehensive biomedical text corpus consisting of MDPI journal articles and open-source medical textbooks for language model training and research.

OpenMedText is a large-scale biomedical text dataset that includes:
- **Med-MDPI**: 121,489 biomedical journal articles across 37 categories from MDPI journals
- **Med-Textbooks**: 29 open-source medical textbooks covering various medical disciplines

## Dataset Meta Information

### MDPI Journals Details

The Med-MDPI component contains 121,489 biomedical journal articles covering 37 diverse topics, emphasizing the breadth of biomedical subjects and leveraging open access to ensure a wide-ranging representation of contemporary biomedical research.

| Journal Category | Number of Journals | Number of Tokens |
|------------------|--------------------|--------------------|
| Allergies | 25 | 140,865 |
| Antibiotics | 3,604 | 26,572,807 |
| Antibodies | 380 | 3,248,253 |
| Behavioral Science | 1,047 | 7,553,809 |
| Biologics | 32 | 261,410 |
| Biomedicines | 3,909 | 34,783,559 |
| Biomedical Informatics | 26 | 201,656 |
| Biomolecules | 5,861 | 54,189,205 |
| Biotechnology | 43 | 301,367 |
| Brain Science | 4,205 | 31,937,526 |
| Cancers | 16,218 | 144,418,262 |
| Cardiogenetics | 42 | 210,720 |
| Clinical Medicine | 16,063 | 104,432,430 |
| Clinics and Practice | 499 | 1,395,833 |
| Clinical and Translational Neuroscience | 21 | 196,310 |
| Current Oncology | 759 | 4,458,455 |
| Dermatopathology | 78 | 289,595 |
| Diabetology | 45 | 290,812 |
| Diagnostics | 5,321 | 33,576,475 |
| Diseases | 455 | 2,596,123 |
| Endocrines | 73 | 437,962 |
| Environmental Research and Public Health | 43,763 | 306,603,512 |
| Epidemiologia | 60 | 416,064 |
| Gastroenterology | 66 | 311,194 |
| Gastrointestinal Disorders | 103 | 566,192 |
| Healthcare | 3,940 | 24,272,007 |
| Hearts | 68 | 398,487 |
| Human Life Science and Medicine | 31 | 143,041 |
| Immunological Research and Clinical Applications | 57 | 428,144 |
| Livers | 30 | 217,950 |
| Medicines | 557 | 3,790,942 |
| Medical Sciences | 457 | 3,028,605 |
| Oral | 48 | 232,320 |
| Pharmacy | 977 | 5,240,834 |
| Uro | 38 | 170,764 |
| Vaccines | 3,647 | 28,197,071 |
| Viruses | 8,941 | 75,109,572 |

### Medical Textbooks Details

The Med-Textbooks component includes 29 open-source medical textbooks selected to provide structured medical knowledge organized for educational purposes, aligning with the objective of using contextual fine-tuning to enhance the learning processes of language models.

| Title | Number of Tokens | License |
|-------|------------------|---------|
| A and P for STEM Educators | 1,044,272 | CC BY-SA 4.0 |
| Acid-base Physiology | 120,400 | CC BY-SA 2.0 |
| Advanced Human Nutrition | 104,889 | CC BY-SA 4.0 |
| An EKG Interpretation Primer | 22,766 | CC BY 4.0 |
| Anatomy and Physiology | 773,297 | CC BY 4.0 |
| Anatomy and Physiology II Laboratory Manual | 25,555 | CC BY 4.0 |
| Atlas of Otolaryngology, Head and Neck Operative Surgery | 792,936 | CC BY-NC 3.0 |
| Biology | 824,597 | CC BY |
| Cell Biology, Genetics, and Biochemistry | 47,612 | CC BY-NC-SA |
| Chemistry - Theory, Analysis, Correlation | 176,091 | CC BY-NC-SA 4.0 |
| Computational Cognitive Neuroscience | 118,470 | CC BY-SA 3.0 |
| Concepts of Biology | 355,836 | CC BY 4.0 |
| Contemporary Health Concerns | 99,534 | CC BY-SA 4.0 |
| Fluid Physiology | 47,128 | CC BY-NC-SA 2.0 |
| Foundations of Epidemiology | 61,369 | CC BY-NC 4.0 |
| Health Case Studies | 88,799 | CC BY-SA 4.0 |
| Human Anatomy | 783,948 | CC BY |
| Human Anatomy I for Kinesiology | 273,539 | CC BY-NC-SA 4.0 |
| Lifetime Fitness and Wellness | 145,720 | CC BY 4.0 |
| Medical Terminology for Healthcare Professions | 224,894 | CC BY 4.0 |
| Microbiology | 584,182 | CC BY 4.0 |
| Neuroscience | 34,240 | CC BY 4.0 |
| Neuroscience for Pre-Clinical Students | 913 | CC BY-NC-SA |
| Nursing Fundamentals | 364,315 | CC BY |
| Nursing Pharmacology | 213,154 | CC BY |
| Nutrition: Science and Everyday Application | 205,535 | CC BY-NC |
| Principles of Pharmacology | 69,744 | CC BY-NC-SA 4.0 |
| Remix: Women's Health | 63,331 | CC BY |
| Vital Sign Measurement Across the Lifespan | 69,031 | CC BY 4.0 |

## Folder Structure

```
OpenMedText/
├── Med-MDPI/               # All under CC BY 4.0 license
│   ├── Allergies/
│   ├── Antibiotics/
│   ├── Antibodies/
│   └── ...                 # More journal categories
│
└── Med-Textbooks/          # Organized by license type
    ├── CC-BY/              # CC BY 4.0 and CC BY licensed books
    ├── CC-BY-SA/           # CC BY-SA 4.0, 3.0, 2.0 books
    ├── CC-BY-NC/           # CC BY-NC 4.0, 3.0 books
    └── CC-BY-NC-SA/        # CC BY-NC-SA 4.0, 3.0, 2.0 books
```

## Licenses

This dataset includes materials with different licenses:

1. **Med-MDPI**: All journal articles are under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) license.

2. **Med-Textbooks**: Textbooks have various licenses:
   - **CC BY**: [Creative Commons Attribution](https://creativecommons.org/licenses/by/4.0/)
   - **CC BY-SA**: [Creative Commons Attribution-ShareAlike](https://creativecommons.org/licenses/by-sa/4.0/)
   - **CC BY-NC**: [Creative Commons Attribution-NonCommercial](https://creativecommons.org/licenses/by-nc/4.0/)
   - **CC BY-NC-SA**: [Creative Commons Attribution-NonCommercial-ShareAlike](https://creativecommons.org/licenses/by-nc-sa/4.0/)

Please respect the license of each component when using this dataset.
## Authors and Institutions

Introduce authors and their institutions of this dataset.


## Source Information

Official Website: https://younwoochoi.github.io/cft-iclr/

Download Link: https://huggingface.co/datasets/ywchoi/OpenMedText

Article Address: https://arxiv.org/abs/2503.09032

Publication Date: March 2025

## Citation

```
@inproceedings{
    choi2025teaching,
    title={Teaching {LLM}s How To Learn with Contextual Fine-Tuning},
    author={Younwoo Choi and Muhammad Adil Asif and Ziwen Han and John Willes and Rahul Krishnan},
    booktitle={The Thirteenth International Conference on Learning Representations},
    year={2025},
    url={https://arxiv.org/abs/2503.09032}
}
```