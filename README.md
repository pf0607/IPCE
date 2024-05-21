# AIGC image quality assessment via image-prompt correspondence

## Requirement

torch 1.8+

torchvision

Python 3

pip install ftfy regex tqdm

pip install git+https://github.com/openai/CLIP.git

## Data Preparation

Download the competition test dataset from the specified website and unzip it into the "./data/AIGCQA-30K-Image/test" directory.

## Trained Weights

## Evaluation on AIGCQA-30k-Image test-set

After preparing the code environment and downloading the data and model weights, run the following code to obtain the output.txt file.

```bash
python AIGC_DB_prompt_final.py
```

## Citation

This code is built on [LIQE](https://github.com/zwx8981/LIQE). We thank the authors for sharing their codes. 

```bash
@inproceedings{zhang2023liqe,  
  title={Blind Image Quality Assessment via Vision-Language Correspondence: A Multitask Learning Perspective},  
  author={Zhang, Weixia and Zhai, Guangtao and Wei, Ying and Yang, Xiaokang and Ma, Kede},  
  booktitle={IEEE Conference on Computer Vision and Pattern Recognition},  
  pages={14071--14081},
  year={2023}
}
```
