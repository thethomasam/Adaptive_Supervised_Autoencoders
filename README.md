# Adaptive Weighted Supervised Autoencoder
This project contains the code for an adaptive weighted supervised autoencoder. The purpose of this autoencoder is to learn a low-dimensional representation of input data while also predicting a set of target variables. The weighting of the loss function is dynamically updated during training to ensure that both the reconstruction loss and the regression loss are given appropriate consideration.

### Requirements
This code requires Python 3.6 or later. Additionally, the following Python libraries are required:

numpy
pandas
scikit-learn
tensorflow
Getting Started
To use this code, clone the repository to your local machine:

bash
Copy code
git clone https://github.com/your-username/adaptive-weighted-supervised-autoencoder.git
cd adaptive-weighted-supervised-autoencoder
Next, install the required Python libraries:

Copy code
pip install -r requirements.txt
Data
The code expects input data in CSV format. The first column of the CSV file should contain the target variables, and the remaining columns should contain the input data.

Training
To train the autoencoder, run the following command:

css
Copy code
python train.py --data_path path/to/data.csv
By default, the code will train the autoencoder using an adaptive weighting factor and a mean squared error loss function. The model will be saved to a file named model.h5.

### Inference
To use the trained model for inference, run the following command:



python predict.py --data_path path/to/data.csv --model_path path/to/model.h5
The code will load the trained model from the specified file and generate predictions for the input data.

### Acknowledgments
This project is based on the work of Rifai et al. and Bhatt et al. (see references in references.bib).

### License
This project is licensed under the MIT License - see the LICENSE.md file for details.
