### Introduction

The file, `train_model.ipynb`, helps you quickly train and test a multi-label classification model based on our [Quda](https://github.com/freenli/quda) corpus. 

After some data processing of Quda, we use the [Simple Transformers](https://github.com/ThilinaRajapakse/simpletransformers) to initialize and train a model based on a pretrained model, [bert](https://github.com/google-research/bert/).

### Installation

1. Install Anaconda or Miniconda Package Manager from [here](https://www.anaconda.com/distribution/).

2. Create a new virtual environment and install packages.
   `conda create -n simpletransformers python pandas tqdm`
   `conda activate simpletransformers`
   If using cuda:
   `conda install pytorch cudatoolkit=10.0 -c pytorch`
   else:
   `conda install pytorch cpuonly -c pytorch`
   `conda install -c anaconda scipy`
   `conda install -c anaconda scikit-learn`
   `pip install transformers`
   `pip install seqeval`
   `pip install tensorboardx`

3. Install Apex if you are using fp16 training. Please follow the instructions [here](https://github.com/NVIDIA/apex). (Installing Apex from pip has caused issues for several people.)

4. Install simpletransformers.
   `pip install simpletransformers`

5. Install other python packages.

   `pip install sklearn`

Reference: [Multi-Label Classification using BERT, RoBERTa, XLNet, XLM, and DistilBERT with Simple Transformers](https://towardsdatascience.com/multi-label-classification-using-bert-roberta-xlnet-xlm-and-distilbert-with-simple-transformers-b3e0cda12ce5)

