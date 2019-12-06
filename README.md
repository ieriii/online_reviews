# Fake reviews identification using transfer learning
We study the effectiveness of transfer learning for the detection of fake reviews. We develop the Universal Language Model Fine-tuning [Howard and Ruder, 2018](https://arxiv.org/abs/1801.06146) for fake reviews detection.

## Notebooks
**Amazon_ulmfit.ipynb** notebook contains the following:
- Fake reviews classifier using transfer learning (ULMFiT model)
- Performance metrics and interpretation analysis using Sequential Jacobian and LIME
- Sensitivity and robustness checks

**Amazon_mlp.ipynb** notebook contains the architecture, training and testing of a MultiLayer Perceptron (MLP).
We use MLP as one of the baseline to compare the performance of our fake review classifier in Amazon_ulmfit.ipynb

## Running the code
To run the code please do the following:
- create a separate `data` folder in your repo
- extract Amazon.zip file in the `data` folder
- if necessary, amend the `path` variable in the `Settings` codeblock of each jupyter notebook.

### Installation requirements
The code has been developed and run on Salamander server (www.salamander.ai) which supports Pytorch v1 and Fastai v1 library.  
If you want to run the jupyter notebooks on another server provider (e.g. Kaggle) or personal server, please refer to the Fastai installation guidelines: https://docs.fast.ai/install.html

**Note**: the code has been developed using Fastai v1.0.58

### Other dependencies
Please note that the interpretation analysis in `Amazon_v2.ipynb` requires the installation of the lime library.
To do so, run `!pip install lime` in the notebook.