# Similarity-driven adversarial testing of deep networks

We provide jupyter notebooks with the implementation (and instructions) for different target label choosing strategies based on similarity (WordNet semantic similarity and deep networks' perception of similarity). We also provide the notebooks in the HTML format. Generated labels can be used as targets in targeted and non-targeted attacks (e.g. in gradient-based attacks such as FGSM [1]).

[1] Ian J Goodfellow, Jonathon Shlens, and Christian Szegedy. Explaining and harnessing adversarial examples. arXiv preprint arXiv:1412.6572, 2014

We implemented our methods in such a way as to make them flexible for the easy reproduction of the presented experiments but also for potential studies of other researchers.
Note, that we present only some examples (but the methods are compatible with freely available models from Keras Applications) just to show the operation of the notebooks and to make the use of our materials easy for other researchers.

## There are three notebooks:
* TargetLabelGenerationNeuralNetwork.ipynb
* TargetLabelGenerationWordNetPath.ipynb
* TargetLabelGenerationWordNetWuPalmer.ipynb

The last part of the notebook's name informs about the method used to generate Class Similarity Matrices for the Least Similar (LS) and the Most Similar (MS) class choice: based on neural network's weights (1), based on WordNet path similarity measure (2) and based on WordNet WuPalmer similarity measure (3).

(1) - learned visual similarity, (2, 3) - semantic similarity

## We use the following Python libraries:
* tensorflow (version 2.11.0)
* nltk (version 3.8.1)
* matplotlib (version 3.6.2)
* numpy (version 1.24.0)
* sklearn (version 1.1.3)
