# Fake reviews identification using transfer learning
We study the effectiveness of transfer learning for the detection of fake reviews. We apply the Universal Language Model Fine-tuning (ULMFiT) by [Howard and Ruder, 2018](https://arxiv.org/abs/1801.06146) to fake reviews detection and demonstrate that it can successully detect fake reviews.

## Notebooks
**Amazon_ulmfit.ipynb** notebook contains the following:
- Fake reviews classifier using transfer learning (ULMFiT model)
- Performance metrics and interpretation analysis using Sequential Jacobian and LIME
- Sensitivity and robustness checks

**Amazon_mlp.ipynb** notebook contains the architecture, training and testing of a MultiLayer Perceptron (MLP).
We use MLP as one of the baseline to compare the performance of our fake review classifier in Amazon_ulmfit.ipynb

**Utils_unzip_data.ipynb** contains a short code snippet to unzip data.

## Running the code

### Data
- create a separate `data` folder in your repo (and `train`, `test`, `unsup` subfolders if uploading extracted data manually);
- extract zip file or locate relevant files in the `data` folder (and relevant subfolders if uploading extracted data manually); and
- if necessary, amend the `path` variable in the `Settings` codeblock of each jupyter notebook.

**Note**: 
The `train` and `test` data can be downloaded from: https://myleott.com/op-spam.html
We use additional `unsup` data to train the language model from: http://odds.cs.stonybrook.edu/yelpchi-dataset/

### Installation requirements
The code has been developed and run on Salamander server (www.salamander.ai) which supports Pytorch v1 and Fastai v1 library. If you want to run the jupyter notebooks on another server provider (e.g. Kaggle) or personal server, please refer to the Fastai installation guidelines: https://docs.fast.ai/install.html

**Note**: the code has been developed using Fastai v1.0.58

### Other dependencies
Please note that the interpretation analysis in `Amazon_v2.ipynb` requires the installation of the lime library.
To do so, run `!pip install lime` in the notebook.