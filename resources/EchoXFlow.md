# EchoXFlow

## Dataset Information

EchoXFlow is a multimodal echocardiography dataset of 35,377 recordings from 666 routine-care examinations. It preserves scanner-native beamspace B-mode and Doppler streams before scan conversion, with synchronized ECG, geometry, calibration, and timestamps. Imaging includes time-resolved 1D, 2D, multiplane, and 3D B-mode, with color, tissue, pulsed-wave, and continuous-wave Doppler.

Research applications include cross-modal Doppler estimation, cardiac segmentation, ECG-conditioned video generation, and acquisition-aware multimodal learning. The release is single-centre and single-vendor, and is not validated for clinical deployment.

## Dataset Meta Information

| Dimensions | Modality | Task Type | Anatomical Structures | Anatomical Area | Number of Categories | Data Volume | File Format |
|---|---|---|---|---|---|---|---|
| Time-resolved 1D, 2D, multiplane and 3D | Ultrasound, Doppler, ECG | Cross-modal estimation; segmentation; conditioned video generation | Cardiac chambers and myocardium; LV endocardial surfaces | Heart | Task-dependent; no single global class count | 35,377 recordings / 666 examinations | Zarr v2 in per-examination TAR; Croissant JSON metadata |

### Resolution Details

Native array dimensions and sampling rates vary by recording and modality. Shapes, timestamps, and acquisition calibration are recorded in the Croissant catalog and recording stores. A single global image size or voxel spacing is not specified.

## Label Information Statistics

Annotation availability varies by recording. The release includes 2D speckle-tracking contours, 3D left-ventricular endocardial meshes, sample-volume locations, clinical measurement points/lines, and spectral traces. Contours and meshes are supplied annotations; pixel/voxel masks can be derived from them.

Patient-level five-fold assignments are supplied separately. Counts in this entry follow the current Hugging Face release; the arXiv preprint describes an earlier version.

## Visualization

Example multimodal recordings are shown in the [official dataset card](https://huggingface.co/datasets/Ahus-AIM/EchoXFlow).

## File Structure

```text
EchoXFlow/
├── croissant.json
├── splits.csv
├── view_classifier_probabilities.csv
├── LICENSE
└── exams/
    └── <exam_id>.tar
        └── exams/<exam_id>/<recording_id>.zarr/
            ├── data/
            ├── derived/
            ├── coordinates/
            ├── timestamps/
            └── annotations/
```

## Authors and Institutions

Elias Stenhede, Joanna Sulkowska, Eivind Bjørkan Orstad, Henrik Schirmer, and Arian Ranjbar. See the paper for affiliations.

## Source Information

Official dataset and download: https://huggingface.co/datasets/Ahus-AIM/EchoXFlow

Readers and benchmark code: https://github.com/Ahus-AIM/EchoXFlow

Paper: https://arxiv.org/abs/2605.05447

Paper submission date: 2026-05-06.

Dataset license: [CC BY-NC-SA 4.0](https://huggingface.co/datasets/Ahus-AIM/EchoXFlow/blob/main/LICENSE).

## Citation

```bibtex
@misc{stenhede2026echoxflow,
  title = {EchoXFlow: A Beamspace Echocardiography Dataset for Cardiac Motion, Flow, and Function},
  author = {Stenhede, Elias and Sulkowska, Joanna and Orstad, Eivind Bj{\o}rkan and Schirmer, Henrik and Ranjbar, Arian},
  year = {2026},
  eprint = {2605.05447},
  archivePrefix = {arXiv},
  primaryClass = {cs.CV},
  doi = {10.48550/arXiv.2605.05447},
  url = {https://arxiv.org/abs/2605.05447}
}
```
