# PyTorch Learning Workspace

This folder is a small PyTorch learning project. It starts from the basics, moves into autograd, and then ends with a simple diabetes prediction project.

The work here is written in a step-by-step way, so it is easy to follow even if you are still new to PyTorch.

## What is inside this folder

### 1. `what_is_pytorch`

This file explains PyTorch in simple words.

It covers:
- what PyTorch is
- where it is used
- what tensors are
- what autograd does
- why PyTorch is popular
- the main benefits of learning PyTorch

This is a good starting point before opening the notebooks.

### 2. `pytorch_basics.ipynb`

This notebook is the introduction notebook.

It compares NumPy and PyTorch side by side and shows how the same math works in both.

Topics covered in this notebook:
- matrix transpose
- dot product
- matrix multiplication
- softmax
- logarithms
- entropy and cross-entropy intuition

The goal of this notebook is to make tensor operations feel familiar before moving into model training.

### 3. `pytorch_autograd.ipynb`

This notebook explains autograd from the ground up.

It includes:
- setting up PyTorch
- understanding `requires_grad`
- forward pass
- backward pass
- how gradients are stored
- why gradients accumulate
- chain rule with small examples
- a simple neuron with weight and bias
- loss calculation
- manual weight updates
- learning rate explanation
- building and training a tiny neural network
- testing the trained model

This notebook is helpful for understanding what happens during training instead of only calling library functions.

### 4. `calculations/`

This folder contains image files related to loss calculations:
- `0_loss_calculation.png`
- `1_loss_calculations.png`
- `2_loss_calculations.png`

These images look like supporting notes or visual references for understanding how loss is calculated step by step.

### 5. `project/`

This folder contains the main hands-on project in this workspace.

#### `classification_project.ipynb`

This notebook builds a beginner-friendly binary classification project using PyTorch and a diabetes dataset.

Work done in this notebook:
- set the dataset path
- import NumPy, pandas, and PyTorch
- load the CSV file
- preview the raw dataset
- convert text categories like gender and smoking history into numbers
- inspect the encoded table
- standardize continuous columns like age, BMI, HbA1c level, and blood glucose level
- convert the prepared data into PyTorch tensors
- build a simple neural network with `torch.nn.Sequential`
- train the model using `BCEWithLogitsLoss`
- make a sample prediction
- convert model output into probability using sigmoid
- apply a threshold of `0.5` to decide the final class

This notebook shows a full beginner workflow from raw CSV data to model prediction.

#### `project/dataset/`

This folder stores the dataset used in the classification project.

Files inside:
- `diabetes_prediction_dataset.csv`

This dataset is used to train and test the diabetes prediction model.

### 6. `requirements.txt`

This file lists the main packages used in the project:
- `numpy`
- `torch`
- `ipykernel`
- `pandas`

These are enough to run the notebooks in this workspace.

## Learning flow of this project

The folder is arranged in a simple learning order:

1. Read `what_is_pytorch`
2. Start with `pytorch_basics.ipynb`
3. Continue with `pytorch_autograd.ipynb`
4. Finish with `project/classification_project.ipynb`

So the learning path goes like this:

basic PyTorch concepts -> tensor math -> autograd -> neural network training -> real classification project

## In short

This workspace covers three main things:
- learning PyTorch basics
- understanding autograd and training logic
- building one real beginner project with tabular data

If someone opens this folder for the first time, the easiest place to begin is `what_is_pytorch`, then the basics notebook, then the autograd notebook, and finally the classification project.
