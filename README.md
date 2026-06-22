# Attension-in-NLP
Attention in NLP: Visualising Which Words Influence Sentiment Predictions
Overview
This repository contains the code and tutorial materials for an NLP deep learning tutorial on attention mechanisms for sentiment classification. The tutorial demonstrates how a neural network can classify IMDB movie reviews as positive or negative while also producing attention weights that help visualise which words influenced the prediction.
The main focus is not to build a production-level sentiment classifier, but to explain how attention works in an NLP pipeline.
Tutorial Topic
Title: Attention in NLP: Visualising Which Words Influence Sentiment Predictions
This tutorial explains how text is processed through the following stages:
1.Tokenisation 
2.Padding 
3.Word embedding 
4.Bidirectional LSTM 
5.Attention layer 
6.Sentiment prediction 
The attention mechanism is used to assign importance weights to word positions in a review, making the model easier to inspect and interpret.
Repository Structure
attention-nlp-sentiment-tutorial/
│
├── README.md
├── LICENSE
├── requirements.txt
├── attention_nlp_sentiment_tutorial.ipynb
├── tutorial.pdf
│
└── figures/
    ├── figure_1_tokenisation_padding.png
    ├── figure_2_attention_based_nlp_pipeline.png
    ├── figure_3_training_validation_accuracy.png
    └── figure_4_attention_weights.png
Dataset
The tutorial uses the IMDB movie review sentiment classification dataset available through Keras. The dataset contains movie reviews labelled as:
0 = Negative sentiment 
1 = Positive sentiment 
A small subset of the dataset is used so that the notebook runs quickly and remains suitable for tutorial demonstration.
Model Architecture
The model used in the notebook follows this structure:
Layer	Function
Input layer	Receives the padded review sequence.
Embedding layer	Converts word indexes into dense word vectors.
Bidirectional LSTM	Learns contextual sequence representations.
Attention layer	Assigns importance weights to word positions.
Dense layer	Learns higher-level sentiment patterns.
Sigmoid output	Produces a positive or negative sentiment probability.
How to Run the Notebook
1.Clone or download this repository. 
2.Install the required packages: 
pip install -r requirements.txt
1.Open the notebook: 
Gopi_code_ml.ipynb
1.Run all cells from top to bottom. 
The notebook will:
Load the IMDB dataset 
Pad review sequences 
Decode reviews into readable text 
Build a BiLSTM-attention model 
Train the model briefly 
Plot training and validation accuracy 
Visualise attention weights for selected words 
Print prediction examples 
Required Libraries
The notebook uses:
TensorFlow 
Keras 
NumPy 
Matplotlib 
A simple requirements.txt file can contain:
tensorflow
numpy
matplotlib
Figures Used in the Tutorial
The tutorial includes the following figures:
Figure 1: Tokenisation and padding example 
Figure 2: Attention-based NLP pipeline 
Figure 3: Training and validation accuracy 
Figure 4: Attention weights for selected words 
Each figure is created or saved as part of the tutorial materials.
