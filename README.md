# Machine Learning Lab Work

Practical sessions from the MSc in Artificial Intelligence and Robotics. Each notebook takes one method and works through it on real data, with the reasoning written out rather than only the code.

## Notebooks

**`Linear Regression Practice.ipynb`**
Linear regression, first on a synthetic dataset where the ground truth is known, then on the diabetes dataset. Covers polynomial features and where they start to overfit, and uses PCA and t-SNE to look at the data in lower dimensions.

**`Logistic regression.ipynb`**
Logistic regression on Iris, then on MNIST and Fashion MNIST, with standardised features and accuracy compared across the three.

**`SVM.ipynb`**
Support vector machines, starting with two class separation on Iris and moving to Fashion MNIST. Compares kernels and reads the results off confusion matrices rather than accuracy alone.

**`ActiveLearning-2022.ipynb`**
Active learning with an SVM on MNIST. Instead of training on everything, the model repeatedly picks which examples it would most like labelled next, which shows how much of a dataset is actually doing useful work.

**`Labwork_clustering.ipynb`**
Clustering rhodopsin membrane proteins. The input is not feature vectors but TM scores, a structural similarity measure computed between every pair of proteins, so part of the exercise is that a similarity is not a distance and cannot be fed to a clustering algorithm unchanged. Uses K-Means and agglomerative clustering, PCA for visualisation, and silhouette scores to judge the result.

## Stack

Python, scikit-learn, TensorFlow and Keras for the MNIST and Fashion MNIST loaders, NumPy, Matplotlib.

## Running them

```
pip install numpy scikit-learn matplotlib tensorflow
jupyter notebook
```

Each notebook is self contained and downloads its own dataset, apart from the clustering one, which needs the rhodopsin TM score file.
