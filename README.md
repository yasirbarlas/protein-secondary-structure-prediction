# INM701: Protein Secondary Structure Prediction

Note: This repository and its contents support the coursework of the INM701 module at City, University of London.

## Background

Protein structure prediction is an important area of bioinformatics and computational biology. By understanding the 3-D structure of a protein from its amino acid sequence, researchers and scientists can understand the biological function of proteins and how proteins can interact with one another. In recent years, powerful tools such as DeepMind's AlphaFold have been able to predict over 200 million protein structures. We investigate the use of simple machine learning algorithms to predict the secondary structure of proteins.

Specifically, we look at using (for classification) the:

- Non-parametric k-nearest neighbors algorithm
- Non-parametric random forests
- Parametric neural networks

## Dataset

The dataset used is a subset of the [RCSB Protein Data Bank](https://www.rcsb.org/), obtained jointly using various programs by [@alfrandom](https://www.kaggle.com/alfrandom) and [@kirkdco](https://www.kaggle.com/kirkdco). The dataset can be found [here](https://www.kaggle.com/datasets/kirkdco/protein-secondary-structure-2022?select=2022-08-03-ss.cleaned.csv). After some processing, we filtered the dataset by selecting proteins that had length in range [16, 100]. The filtered dataset containing the protein sequences for this study can be found [here](../main/datasets/prot-seq-filtered.csv).
