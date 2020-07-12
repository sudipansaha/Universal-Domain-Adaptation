# Universal Domain Adaptation

Code release for  **[Universal Domain Adaptation(CVPR 2019)](https://youkaichao.github.io/files/cvpr2019/1628.pdf)** 

## Updates in this fork
- Updated requirements.txt
- More info in data folder
- In the train and test config files, in line 5 and 6, source and target domain index need to be mentioned. For Officehome dataset, Art: 0, Clipart: 1, Product: 2, Real_World: 3


## Requirements
- python 3.6+
- PyTorch 1.0

`pip install -r requirements.txt`

## Usage

- download datasets

- write your config file

- `python main.py --config /path/to/your/config/yaml/file`

- train (configurations in `officehome-train-config.yaml` are only for officehome dataset):

  `python main.py --config officehome-train-config.yaml`

- test

  `python main.py --config officehome-test-config.yaml`
  
- monitor (tensorboard required)

  `tensorboard --logdir .`

## Checkpoints

We provide the checkpoints for officehome datasets at [Google Drive](https://drive.google.com/drive/folders/1Kw3Lfw4dPdTZ8RQ1cUQVDpE5odp8th7J?usp=sharing).

## Citation
please cite:
```
@InProceedings{UDA_2019_CVPR,
author = {You, Kaichao and Long, Mingsheng and Cao, Zhangjie and Wang, Jianmin and Jordan, Michael I.},
title = {Universal Domain Adaptation},
booktitle = {The IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},
month = {June},
year = {2019}
}
```

## Contact
- youkaichao@gmail.com
- longmingsheng@gmail.com
