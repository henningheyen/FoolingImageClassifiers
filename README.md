# FoolingImageClassifiers

Welcome to this notebook!

The goal of this project is to show how state-of-the-art image classifiers behave when the
input images are **out of distribution**. 

# Content

1. **Collecting a test set with epistemic uncertainty and passing it through image classifiers**:
     - We use different images of umbrellas that are potentially out of distribution and investigate how common Imagenet pre-trained models classify those images.
3. **Building an uncertainty quantification ensemble**:
     - We use probabilistic averaging to build an ensemble model and take the maximum probability to measure its uncertainty.
5. **Fooling one of the models**:
     - We use various perturbed images of flamingos and zebras and pass them through the _xception_ model.
7. **Analysing saliency maps for the images**:
     - We use saliency methods to attempt to visualise how important parts of the perturbed images were to the neural network. We try to reason about why the model was fooled.
9. **Discussion within the context of Responsible AI**:
     - The last section aims to point out some of the most important challenges related to AI robustness and security and then outline how the AI community aims to tackle them.

# Repository

The repository consists of the `notebook`, an in depth `report`, the `imagenet_class_index.json` file for section 4 and the `images` used in this notebook. Please note that all outputs in the `.ipynb` file had to be cleared due to size constraints in GitHub which is why I uploaded a `.pdf` version of the notebook that contains all outputs. 

# Getting started

To run this notebook please use [Google Colab](https://colab.google/) as all libraries (especially TF Keras) are preinstalled there. Just upload the `images` folder and the `imagenet_class_index.json` file and change the path if necessary. 
