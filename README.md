# Positional Bias suppression for LLM-based Radiology Report Generation

## Introduction
![overview](https://github.com/zailongchen/Attention_Suppression/blob/main/images/position_characteristic.png)

## Getting Started
### Installation

**1. Prepare the code and the environment**

Git clone our repository and install the requirements.

```bash
https://github.com/zailongchen/Attention_Suppression.git
cd Attention_Suppression
pip install -r requirements.txt
```


**2. Prepare the training dataset**

IU-xray: download the dataset from [here](https://drive.google.com/file/d/1c0BXEuDy8Cmm2jfN0YYGkQxFZd2ZIoLg/view)

Mimic-cxr: you can download our preprocess annotation file from [here](https://drive.google.com/file/d/14689ztodTtrQJYs--ihB_hgsPMMNHX-H/view?usp=sharing) and download the images from [official website](https://physionet.org/content/mimic-cxr-jpg/2.0.0/)

After downloading the data, place it in the ./data folder.

### Training

For MIMIC-CXR

```bash
bash scripts/run_mimic.sh
```

For IU-Xray

```bash
bash scripts/run_iuxray.sh
```

### Testing (For MIMIC-CXR)

For MIMIC-CXR

```bash
bash scripts/test_mimic.sh
```

For IU-Xray

```bash
bash scripts/test_iuxray.sh
```


## Acknowledgement

+ [R2GenGPT](https://github.com/wang-zhanyu/R2GenGPT) Some codes of this repo are based on R2GenGPT.
+ [Llama2](https://github.com/facebookresearch/llama) The fantastic language ability of Llama-2 with only 7B parameters is just amazing.


## License
This repository is under [MIT License](LICENSE.md).
