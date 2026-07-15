# TCGA virtual spatial transcriptomics atlas

## Dataset Information

The TCGA virtual spatial transcriptomics atlas provides DeepSpot-M predicted transcriptome-wide spatial gene expression for The Cancer Genome Atlas (TCGA) H&E whole-slide images. Predictions cover 28,664 diagnostic slides (17,372 fresh-frozen and 11,292 FFPE) from 10,865 patients across 32 cancer types (~295.3 million spots). Expression was inferred from histology alone (TCGA has no matched spatial transcriptomics). For 14 cancer types represented in the DeepSpot-M spatial training corpus, cancer-specific finetuned models were used; the remaining 18 cancers were predicted zero-shot. Each sample is a gzip-compressed AnnData (`.h5ad.gz`) with predicted log1p-CPM expression for the protein-coding transcriptome (19,338 genes) and an embedded H&E thumbnail. The resource is released as an open (gated, CC-BY-NC-SA-4.0) Hugging Face dataset to support biomarker discovery and benchmarking of virtual spatial transcriptomics methods at population scale.

## Dataset Meta Information

| Task Type  | Language | Number | File Format |
|------------|----------|--------|-------------|
| image-gene | English  | 28664  | .h5ad.gz    |

## Dataset Information Statistics

| Slides | Patients | Cancer types | Spots   | Genes  | FF / FFPE |
|--------|----------|--------------|---------|--------|-----------|
| 28,664 | 10,865   | 32           | 295.3M  | 19,338 | 17,372 / 11,292 |

## File Structure

```
data/<TCGA_TYPE>/<FF|FFPE>/<sample_id>.h5ad.gz
metadata_YYYY-MM-DD.csv
```

## Authors and Institutions

Kalin Nonchev (ETH Zurich)

Sebastian Dawo (University of Basel / University Hospital Basel)

Karina Silina (ETH Zurich)

Viktor Hendrik Koelzer (University of Basel / University Hospital Basel)

Gunnar Rätsch (ETH Zurich)

## Source Information

Official Website: https://github.com/ratschlab/DeepSpotM

Download Link: https://huggingface.co/datasets/ratschlab/TCGA_virtual_spatial_transcriptomics_atlas

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
