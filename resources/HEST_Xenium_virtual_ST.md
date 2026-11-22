# HEST Xenium virtual spatial transcriptomics

## Dataset Information

This dataset releases DeepSpot-M predicted single-cell transcriptome-wide spatial profiles for all 59 HEST-1k 10x Xenium H&E samples, spanning 22 tissue types (~13.3 million cells). Xenium measures a targeted gene panel; DeepSpot-M extends each cell to the protein-coding transcriptome (19,338 genes, log1p-CPM) while preserving cell coordinates and H&E context. Predictions are cell-level (not Visium spot-level). Files are gzip-compressed AnnData (`.h5ad.gz`) keyed by HEST sample id, with clinical and technical metadata aligned to the canonical HEST table. The resource is gated (CC-BY-NC-SA-4.0) on Hugging Face and is intended for virtual single-cell spatial transcriptomics analysis and benchmarking beyond fixed Xenium panels.

## Dataset Meta Information

| Task Type  | Language | Number | File Format |
|------------|----------|--------|-------------|
| image-gene | English  | 59     | .h5ad.gz    |

## Dataset Information Statistics

| Samples | Tissue types | Cells  | Genes  | Resolution |
|---------|--------------|--------|--------|------------|
| 59      | 22           | ~13.3M | 19,338 | Cell-level |

## File Structure

```
data/<sample_id>.h5ad.gz
metadata.csv
```

## Authors and Institutions

Kalin Nonchev (ETH Zurich)

Sebastian Dawo (University of Basel / University Hospital Basel)

Karina Silina (ETH Zurich)

Viktor Hendrik Koelzer (University of Basel / University Hospital Basel)

Gunnar Rätsch (ETH Zurich)

## Source Information

Official Website: https://github.com/ratschlab/DeepSpotM

Download Link: https://huggingface.co/datasets/ratschlab/HEST_Xenium_virtual_spatial_transcriptomics

Article Address: https://www.medrxiv.org/content/10.64898/2026.06.19.26356060v1

Publication Date: 2026-06

## Citation

```
@article{nonchev2026deepspotm,
  title={DeepSpot-M: a multimodal foundation model for transcriptome-wide virtual spatial transcriptomics from histology},
  author={Nonchev, Kalin and Dawo, Sebastian and Silina, Karina and Koelzer, Viktor Hendrik and Raetsch, Gunnar},
  journal={medRxiv},
  year={2026},
  doi={10.64898/2026.06.19.26356060},
  url={https://www.medrxiv.org/content/10.64898/2026.06.19.26356060v1}
}
```
