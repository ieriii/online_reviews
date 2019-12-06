# Fake review identification using transfer learning

**Amazon_v2.ipynb** notebook contains the following:
- Fake reviews classifier using transfer learning (ULMFiT)
- Performance metrics and interpretation analysis using Sequential Jacobian and LIME
- Sensitivity and robustness checks

**Amazon_mlp.ipynb** contains the architecture, training and testing of a MultiLayer Perceptron (MLP).
We use MLP as one of the baseline to compare our fake review classifier against.

# Running the code
To run the code please do the following:
- create a folder in a separate 'data' folder
- extract Amazon.zip file
- if necessary, amend the `path` variable in the codeblock `Settings` of each jupyter notebook.

# Installation and requirements
The code has been run on Salamander server (www.salamander.ai) which supports Pytorch v1 and Fastai library.
If you want to run the jupyter notebooks on another server provider or personal server, please refer to the Fastai installation guidelines: https://docs.fast.ai/install.html

# Other dependencies
Pleaes note that the interpretation analysis in `Amazon_v2.ipynb` requires the installation of the lime library.
To do so, run `!pip install lime` in the notebook