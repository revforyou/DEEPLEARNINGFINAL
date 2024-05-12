---
dataset_info:
  features:
  - name: resume_str
    dtype: string
  - name: category
    dtype: string
  - name: __index_level_0__
    dtype: int64
  splits:
  - name: train
    num_bytes: 12496606
    num_examples: 1987
  - name: test
    num_bytes: 1631312
    num_examples: 248
  - name: validation
    num_bytes: 1604207
    num_examples: 249
  download_size: 7940604
  dataset_size: 15732125
configs:
- config_name: default
  data_files:
  - split: train
    path: data/train-*
  - split: test
    path: data/test-*
  - split: validation
    path: data/validation-*
---
