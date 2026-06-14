# dog-vs-cat-classifier-
A binary image classifier (dog vs cat) built from scratch using only NumPy
# Dog vs Not-Dog Classifier (Built from Scratch with NumPy)

A binary image classifier that distinguishes dogs from cats, built using 
**only NumPy** — no deep learning frameworks. Implements logistic regression 
as a single-neuron neural network from the ground up, including forward 
propagation, backward propagation, and gradient descent.

This project was built while studying Andrew Ng's Deep Learning Specialization 
(Course 1: Neural Networks and Deep Learning).

## What's Implemented

- Custom image loading and preprocessing pipeline
- Image flattening and normalization (vectorized)
- Sigmoid activation function
- Forward propagation
- Cost function (binary cross-entropy)
- Backward propagation (gradient computation)
- Gradient descent optimizer
- Prediction function

## Dataset

[Kaggle Dogs vs Cats Dataset](https://www.kaggle.com/datasets/bhavikjikadara/dog-and-cat-classification-dataset)
(Not included in this repo — download separately)

## Results & Experiments

| Iterations | Train Accuracy | Test Accuracy |
|---|---|---|
| 500  | 66.9% | 57.5% |
| 2000 | 77.5% | 52.5% |
| 5000 | 81.9% | 47.5% |

## Key Learning: Overfitting

As iterations increased, training accuracy improved while test accuracy 
declined — a clear hands-on demonstration of overfitting. This showed that 
"more training" isn't always better, and motivated the need for techniques 
like regularization and deeper architectures (covered in later courses).

## Tech Stack

- Python
- NumPy
- Matplotlib
- Pillow (PIL)

## How to Run

1. Clone this repo
2. Install requirements: `pip install -r requirements.txt`
3. Download the dataset and place images in `Dog/` and `Cat/` folders
4. Run the notebook: `dog_vs_cat_classifier.ipynb`

## Next Steps

- Implement a deeper neural network (multiple layers)
- Add regularization to reduce overfitting
- Try CNNs for better feature extraction (Course 4)
