# INM701: Protein Secondary Structure Prediction

Note: This repository and its contents support the coursework of the INM701 module at City, University of London.

## Background

Protein structure prediction is an important area of bioinformatics and computational biology. By understanding the 3-D structure of a protein from its amino acid sequence, researchers and scientists can understand the biological function of proteins and how proteins can interact with one another. In recent years, powerful tools such as DeepMind's AlphaFold have been able to predict over 200 million protein structures. We investigate the use of simple machine learning algorithms to predict the secondary structure of proteins.

Specifically, we look at using (for classification) the:

- Non-parametric $k$-nearest neighbours
- Non-parametric random forests
- Parametric neural networks

## Dataset

The dataset used is a subset of the [RCSB Protein Data Bank](https://www.rcsb.org/), obtained jointly using various programs by [@alfrandom](https://www.kaggle.com/alfrandom) and [@kirkdco](https://www.kaggle.com/kirkdco). The dataset can be found [here](https://www.kaggle.com/datasets/kirkdco/protein-secondary-structure-2022?select=2022-08-03-ss.cleaned.csv). After some processing, we filtered the dataset by selecting proteins that had length in range [16, 100]. The filtered dataset containing the protein sequences for this study can be found [here](../main/datasets/prot-seq-filtered.csv).

## $k$-nearest neighbours

$k$-nearest neighbours ($k$-NN) is a non-parametric machine learning algorithm, which is also a type of lazy learning algorithm. The algorithm classifies data by assigning labels to observations based on the majority class amongst their "$k$-nearest neighbours". We construct models based on $k$-NN, and the related work can be found in the [random-forests](../main/random-forests/) folder.

## Random Forests

Random forests is a non-parametric machine learning algorithm and a type of ensemble method. The random forests algorithm works by constructing a multitude of decision trees during the training phase. We construct models based on random forests, and the related work can be found in the [random-forests](../main/random-forests/) folder.

## Neural Networks

Artificial neural networks are parametric machine learning algorithms that try to mimic the way information is processed in the brain. The idea is to create models of biological neurons that have connections between nodes, with weights attached. These weights are to be optimised through the use of methods such as gradient descent with backpropagation. We construct models based on neural networks, and the related work can be found in the [neural-networks](../main/neural-networks/) folder.
