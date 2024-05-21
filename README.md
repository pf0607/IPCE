## AIGC Image Quality Assessment via Image-Prompt Correspondence (IPCE, Image-Prompt Correspondence Estimator)
The official repo of AIGC Image Quality Assessment via Image-Prompt Correspondence. (CVPRW2024, the first place in the image track of the NTIRE 2024 Quality Assessment for AI-Generated Content challenge)

## Requirement

torch 1.8+

torchvision

Python 3

pip install ftfy regex tqdm

pip install git+https://github.com/openai/CLIP.git

## Data Preparation

Download [AGIQA-1K](https://github.com/lcysyzxdxc/AGIQA-1k-Database), [AGIQA-3K](https://github.com/lcysyzxdxc/AGIQA-3k-Database), [AIGCIQA2023](https://github.com/wangjiarui153/AIGCIQA2023) and [AIGCQA-30K-Image](https://www.modelscope.cn/datasets/lcysyzxdxc/AIGCQA-30K-Image/summary) datasets and unzip them into the "<u>./data</u>" directory.

## Training and Testing

After preparing the code environment and downloading the data, run the following codes to train and test model.

```bash
#AIGCQA-30K-Image
python train_aigcqa30k.py
#AGIQA-1K
python train_aigc_agiqa1k.py
#AGIQA-3K
python train_aigc_agiqa3k.py
#AIGCIQA2023
python train_aigc_aigciqa2023.py
```

For AIGCQA-30-Image dataset, run the following codes to get val and test output.

```bash
AIGC_DB_AIGCQA30K_VAL.py
AIGC_DB_AIGCQA30K_TEST.py
```
## Citation

If you find our work useful in your research, please consider citing our paper:
