# KPMP Xenium virtual spatial transcriptomics

## Dataset Information

This dataset releases DeepSpot-M predicted single-cell transcriptome-wide spatial profiles for 49 H&E sections of Kidney Precision Medicine Project (KPMP) 10x Xenium kidney biopsies (~1.64 million cells). Xenium measures a targeted gene panel; DeepSpot-M extends each cell to 19,338 genes, and the measured Xenium panel is included. Files are AnnData (`.h5ad`). The resource accompanies a study that extends DeepSpot-M beyond oncology to non-cancerous kidney disease. It is gated (CC-BY-NC-SA-4.0) on Hugging Face.

## Dataset Meta Information

| Task Type  | Language | Number | File Format |
|------------|----------|--------|-------------|
| image-gene | English  | 49     | .h5ad       |

## Dataset Information Statistics

| Sections | Cells  | Genes  | Resolution |
|----------|--------|--------|------------|
| 49       | ~1.64M | 19,338 | Cell-level |

## File Structure

```
data/<CONDITION>/<sample_id>.h5ad
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

Download Link: https://huggingface.co/datasets/ratschlab/KPMP_Xenium_virtual_spatial_transcriptomics

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
