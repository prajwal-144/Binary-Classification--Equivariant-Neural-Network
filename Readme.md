# Models for Binary Classification using Equivariant Neural Network

## PROJECT

Specific Test IV. Exploring Equivariant Neural Networks associated with the project Equivariant Neural Networks for Dark Matter Morphology with Strong Gravitational Lensing.

## GOAL

Use an Equivariant Neural Network to build a robust and efficient model for binary classification on the provided dataset.

## EVALUATION METRICS

ROC curve (Receiver Operating Characteristic curve) and AUC score (Area Under the ROC Curve)

## APPROACH

* I have used General E(2)-Equivariant Steerable CNNs to implement the solution for the task.

* [Test_4_Cyclic.ipynb](https://github.com/prajwal-144/DeepLense_Tests_2023/blob/main/Task_4/Test_4_Cyclic.ipynb) builds a model equivariant to 8 rotations. We indicate the group of N discrete rotations as  C<sub>N</sub>  which means the Cyclic Group of order N. We implement C<sub>8</sub>.

* [Test_4_Dihedral.ipynb](https://github.com/prajwal-144/DeepLense_Tests_2023/blob/main/Task_4/Test_4_Dihedral.ipynb) builds a model based on Dihedral group D<sub>2N</sub> which is group of N discrete planar rotations and reflections. D<sub>N</sub> has an order of 2N. We implement D<sub>4</sub> in this notebook which expand to 4 rotations and 4 reflections.

* [Task_4_Report.pdf](https://github.com/prajwal-144/DeepLense_Tests_2023/blob/main/Task_4/Task_4_Report.pdf) contains the documentation of the the work done. The model weights for the network can be downloaded and used from:

* **Model Weights for Dihedral Group Equivariance** : https://drive.google.com/file/d/1pgGjBwAUHTiXejiWA3hpHuHRB1BkIwEf/view?usp=sharing

* **Colab Notebook for Dihedral** : https://colab.research.google.com/drive/1q6E-qFMwR7hxYfBbnV9YUZqR6VfAQDJ-?usp=sharing

* **Model Weights for Cyclic Group Equivariance** : https://drive.google.com/file/d/1AKAGe-cecKObsnBrK76LTBHNqFwz1bOa/view?usp=sharing

* **Colab Notebook for Cyclic** : https://colab.research.google.com/drive/1tHji-woLdPQsZFJ0ZD4NjD--GjtgFqwP?usp=sharing

## ACCURACIES

| Model         | Architecture                | Accuracy in % (on testing data) |
| ------------- |:---------------------------:|:-------------------------------:|
| C<sub>8</sub> | C<sub>8</sub> Steerable CNN |99.6                             |
| D<sub>4</sub> | D<sub>4</sub> Steerable CNN |99.4                             |

## AUC SCORE

| Model         | AUC Score |
| ------------- |:---------:|
| C<sub>8</sub> | 1.0       |
| D<sub>4</sub> | 1.0       |

