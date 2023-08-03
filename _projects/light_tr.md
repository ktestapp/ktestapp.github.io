---
layout: works-single

# preview details
title: "TLT : Transformer Lightning Language Model"
category: NLP
category_slug: nlp
image: assets/img/projects/lig_cover.png
short: TLT

# full details
full_image: assets/img/projects/lig_cover.png
preview_link: https://github.com/Khamies/Transformer_Lightning
info:
  - label: Project Description
    value: A simple implementation of a transformer based language model using Pytorch-Lightning.

  - label: Tags
    value: pytorch, transformer, language-model, cross-entropy, pytorch-lightning

  - label: Year
    value: 2021
---

## TLT : Transformer Lightning Language Model


### Table of Contents

- **[Introduction](#Introduction)**
- **[Setup](#Setup)**
- [**Run the code**](#Run-the-code)
- **[Training](#Training)**
- **[Sample Generation](#Sample-Generation)**
- **[Connect with me](#Connect-with-me)**
- **[License](#License)** 

### Introduction

This is an implementation of a transformer based language model using [Pytorch-Lightning framework](https://www.pytorchlightning.ai/). The model consists of two transformer layers with 2 heads each combined with embedding and linear layers. The code uses pytorch-lightning framework that is built for fast research prototyping. Although the code does not leverage all the features of the lightning framework, but it has achieved good result in the language modelling task. For learning purposes, a Pytorch classical version from this project is also provided [here](https://colab.research.google.com/drive/1zRm0tfD2gYyL2WNd6o_mVC2IY3prAzPV?usp=sharing) (inspired from Pytorch team  :heart:).

<img src="/assets/img/projects/lig_transformer.jpg" align="center" height="750" width="800" >

### Setup

The code is using `pipenv` as a virtual environment and package manager. To run the code, all you need is to install the necessary dependencies. open the terminal and type:

- `$ git clone https://github.com/Khamies/Transformer_Lightning.git` 
- `$ cd Transformer_Lightning`
- `$ pipenv install`

or

- `$ pip install requirements.txt `

And you should be ready to go to play with code and build upon it!

### Run the code

- To train the model, run: `python main.py`

- To train the model with specific arguments, run: `python main.py --batch_size=64`. The following command-line arguments are available:
  - Train batch size: `--bsz_train`
  - Test batch size: `--bsz_test`
  - bptt: `--bptt`
  - Learning rate: `--lr`
  - Embedding size: `--embed_size`
  - Size of FeedForward Neural Network (1st layer): `--ffnn_size`
  - Attention Heads: `--nhead`
  - Transformer Layers: `--nlayers`

### Training

The model is trained on `10 epochs` using Adam as an optimizer with a `learning rate = 0.001` and `batch size = 32`, you can find all the model settings in [settings.py]( https://github.com/Khamies/Transformer_Lightning/blob/main/settings.py). Here is the loss curve for the training step:

- **Cross Entropy Loss**

  <img src="/assets/img/projects/lig_train_loss.jpg" align="center" height="300" width="500" >

### Sample Generation

Here are some generated samples from the model:

```markdown
<time> warner owns n million francs.
<media> concern said it is a share n million.
```

### Citation

```
 @misc{Khamies2021Transformer_Lightning,
author = {Khamies, Waleed},
title = {A pytorch implementation of transformer based language model using Pytorch-Lightning framework.},
year = {2021},
publisher = {GitHub},
journal = {GitHub repository},
howpublished = {\url{ https://github.com/Khamies/Transformer_Lightning}},
}
```


### License 

![](https://img.shields.io/github/license/Khamies/Transformer_Lightning)

