# KPMP virtual spatial transcriptomics atlas

## Dataset Information

The KPMP virtual spatial transcriptomics atlas provides DeepSpot-M predicted transcriptome-wide spatial gene expression for H&E whole-slide images of kidney biopsies from the Kidney Precision Medicine Project (KPMP). Predictions cover 1,534 whole-slide images from 476 KPMP participants (~5.46 million spots), with 19,338 genes per spot and linked clinical and histopathological annotations. Each sample is an AnnData (`.h5ad`) file. The resource accompanies a study that extends DeepSpot-M beyond oncology to non-cancerous kidney disease, linking histopathology to molecular programs of kidney injury, repair, fibrosis and kidney function. It is released as a gated (CC-BY-NC-SA-4.0) Hugging Face dataset.

## Dataset Meta Information

| Task Type  | Language | Number | File Format |
|------------|----------|--------|-------------|
| image-gene | English  | 1534   | .h5ad       |

## Dataset Information Statistics

| Slides | Participants | Spots  | Genes  |
|--------|--------------|--------|--------|
| 1,534  | 476          | ~5.46M | 19,338 |

## File Structure

```
data/<CONDITION>/<FF|FFPE>/<sample_id>.h5ad
metadata.csv
```

## Authors

Kalin Nonchev

Y. Jang

S. Nlandu Khodo

Viktor Hendrik Koelzer

Gunnar Rätsch

M. B. Moor

## Source Information

Official Website: https://github.com/ratschlab/projects2026-kidney-kpmp-analysis

Download Link: https://huggingface.co/datasets/ratschlab/KPMP_virtual_spatial_transcriptomics_atlas

Article Address: https://www.medrxiv.org/content/10.64898/2026.11.17.26368273v1

Publication Date: 2026-11

## Citation

```
@article{nonchev2026kidney,
  title={Virtual spatial transcriptomics links kidney histopathology to disease-associated molecular programs},
  author={Nonchev, Kalin and Jang, Y. and Nlandu Khodo, S. and Koelzer, Viktor Hendrik and Raetsch, Gunnar and Moor, M. B.},
  journal={medRxiv},
  year={2026},
  doi={10.64898/2026.11.17.26368273},
  url={https://www.medrxiv.org/content/10.64898/2026.11.17.26368273v1}
}
```
