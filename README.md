# Banknote Authentication Neural Network

This project demonstrates a neural network model for banknote authentication using TensorFlow. The model is trained on a dataset of banknote features and labels, and it predicts whether a given banknote is genuine or counterfeit.

## Prerequisites

Before running the code, make sure you have the following dependencies installed:

- Python (version 3.6 or higher)
- TensorFlow (version 2.0 or higher)
- Scikit-Learn (version 0.24 or higher)
- Pandas (version 1.2 or higher)

## Dataset

The dataset used in this project is stored in the file `banknotes.csv`. It contains the following columns:

- `V1`: Variance of Wavelet Transformed image (continuous)
- `V2`: Skewness of Wavelet Transformed image (continuous)
- `V3`: Curtosis of Wavelet Transformed image (continuous)
- `V4`: Entropy of image (continuous)
- `Class`: Class (0 for genuine, 1 for counterfeit)

## Usage

1. Clone this repository to your local machine or download the files.

2. Install the required dependencies using pip or conda:

```shell
pip install tensorflow scikit-learn pandas
```

3. Run the `banknote_authentication.py` script:

```shell
python banknote_authentication.py
```

4. The script will train the neural network model on the dataset and output the accuracy of the model on the testing data.

## Model Architecture

The neural network model consists of two layers:

- **Input Layer**: The input layer has 4 units, corresponding to the 4 features of a banknote. It uses the ReLU activation function.

- **Output Layer**: The output layer has 1 unit, representing the prediction of the model (0 for genuine, 1 for counterfeit). It uses the sigmoid activation function.

The model is compiled with the Adam optimizer and binary cross-entropy loss function.

## Results

After training the model, the script evaluates its performance on the testing data and outputs the loss and accuracy metrics. It acheives an average accuracy of 92%.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more information.
