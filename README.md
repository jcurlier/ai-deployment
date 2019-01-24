# AI Deployment Research

## Installation

1. Clone the directory
2. Run `git lfs install` (see https://git-lfs.github.com/)
3. Install jupyter notebooks and run `jupyter notebook`

## Status

Type | Deployment | Framework | Status
----- | ----- | ----- | -----
Prediction | Google ML | Tensorflow | [Done](./deployment/prediction-googlecloudml-tensorflow.ipynb)
Prediction | Google ML | Keras | [Done](./deployment/prediction-googlecloudml-keras.ipynb)
Prediction | Seldon | Tensorflow | In progess
Prediction | Seldon | Keras |
Prediction | SageMaker | Tensorflow | 
Prediction | SageMaker | Keras |
Classification | Google ML | Keras | [Done](./deployment/classification-googlecloudml-keras.ipynb)
Classification | Seldon | Keras |
Classification | SageMaker | Keras |

## Model types

### Prediction

Predict the earnings of the sale of a new video games based on past game earnings.

Input: Array of float
Output: Value
Transformer: X and Y scaler

*Note:* The input/output have data transformation (scaler)

### Classification

Input: Image
Output: Array of classes

Training of the model should use GPU (about 3 minutes per epoch)

*Note:* The input/output have data transformation (0 to 1 input and score to label output)

## Deployment Flavors

- Google ML
- Seldon / kubeflow
- AWS SageMaker
- kubeflow

## Frameworks

- Tensorflow
- Keras
- pyTorch
