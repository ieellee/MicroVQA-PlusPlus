---
license: cc-by-sa-4.0
configs:
- config_name: default
  data_files:
  - split: train
    path: data/train-*
dataset_info:
  features:
  - name: image_name
    dtype: string
  - name: image
    dtype: image
  - name: question
    dtype: string
  - name: choices
    list: string
  - name: correct_index
    dtype: int64
  - name: correct_answer
    dtype: string
  - name: cot
    dtype: string
  - name: task_str
    dtype: string
  - name: image_caption
    dtype: string
  - name: images_source
    dtype: string
  splits:
  - name: train
    num_bytes: 3637003
    num_examples: 15
  download_size: 3636881
  dataset_size: 3637003
---

# MicroVQA++: High-Quality Microscopy Reasoning Dataset with Weakly Supervised Graphs for Multimodal Large Language Model


### Meta information

Here, we are initially releasing 15 demo samples. The complete training and test data will be fully published after the review process and optimization.


| Field Name     | Data Type        | Description                                                  |
| -------------- | ---------------- | ------------------------------------------------------------ |
| image_name     | string           | Image name in BIOMEDICA                                      |
| image          | Image            | Image for the question                                       |
| question       | string           | Final question                                               |
| choices        | Sequence(string) | List of answer choices                                       |
| correct_index  | int64            | Index of the correct answer in choices                       |
| correct_answer | string           | Correct answer                                               |
| cot            | string           | Explanation of the correct answer                            |
| task_str       | string           | String label for the task type                               |
| image_caption  | string           | Caption describing the image                                 |
| images_source  | string           | From BIOMEDICA. License varies depending on the dataset subset |

