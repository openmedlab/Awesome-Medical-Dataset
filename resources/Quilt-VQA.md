# Quilt-VQA

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/Quilt-VQA_0.png"></a>
</div>
<p style="text-align:center;font-size:10px;"><em></em></p>

## Dataset Information

Quilt-VQA is a dataset specifically designed for visual question answering (VQA) tasks on pathology images, containing 1,283 question-answer pairs based on pathology images. These pairs are categorized into different types, with the dataset comprising 985 associated images. The questions are divided into **open-ended** (940 pairs) and **closed-ended** (343 pairs) categories. In addition to medical knowledge, Quilt-VQA evaluates the model's ability to follow instructions in multimodal conversations. To this end, 326 additional questions were constructed, including 256 dialog-type questions and 70 descriptive-type questions.

This dataset is significant for assessing the knowledge application and conversational understanding capabilities of models like Quilt-LLaVA in the medical domain. Quilt-VQA serves as a valuable benchmark tool for multimodal large language models in the field of pathology, driving advancements in pathology image analysis.

## Dataset Meta Information

| Task Type | Language | Quantity | File Format |
|-----------|----------|----------|-------------|
| VQA       | English  | 1283     | .json       |

## Dataset Statistics Information

| Q–A Pairs | Images | Open | Closed |
|-----------|--------|------|--------|
| 1283      | 985    | 940  | 343    |

## Visualization

<div align="center">
    <a href="https://github.com/openmedlab/"><img width="700px" height="auto" src="appendix/Quilt-VQA_0.png"></a>
</div>
<p style="text-align:center;font-size:10px;"><em>Some examples from the QUILT-VQA dataset. The first two rows show question-answer pairs related to images, while the last two rows present commonsense question-answer pairs. The original questions posed by the video narrator are highlighted in yellow.</em></p>

## File Structure

``` 
.               
├──quilt_vqa.zip
├──quiltvqa_test_w_ans.json
├──quiltvqa_test_wo_ans.jsonl
```

## Authors and Institutions

Mehmet Saygin Seyfioglu (University of Washington)

Wisdom O. Ikezogwo (University of Washington)

Fatemeh Ghezloo (University of Washington)

Ranjay Krishna (University of Washington)

Linda Shapiro (University of Washington)

## Source Information

Official Website: https://quilt-llava.github.io/

Download Link: https://huggingface.co/datasets/wisdomik/Quilt_VQA

Article Address: https://quilt-llava.github.io/

Publication Date: 2024-02

## Citation

``` 
@inproceedings{seyfioglu2024quilt,
  title={Quilt-LLaVA: Visual Instruction Tuning by Extracting Localized Narratives from Open-Source Histopathology Videos},
  author={Seyfioglu, Mehmet Saygin and Ikezogwo, Wisdom O and Ghezloo, Fatemeh and Krishna, Ranjay and Shapiro, Linda},
  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
  pages={13183--13192},
  year={2024}
}
```

Original introduction article is [here](https://zhuanlan.zhihu.com/p/952870679).