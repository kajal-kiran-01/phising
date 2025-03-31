# Phishing Detection using Machine Learning

## Overview
This project implements a machine learning model to detect phishing websites. It utilizes an XGBoost classifier trained on extracted features from URLs to classify websites as either legitimate or phishing.

## Features
- **Dataset Balancing**: Uses SMOTE (Synthetic Minority Over-sampling Technique) to balance the dataset.
- **Model Training**: Trains an XGBoost classifier with hyperparameter tuning.
- **Website Classification**: Extracts features from a given URL and predicts whether the website is phishing or legitimate.
- **Model Saving**: Saves the trained model for later use.
- **Command-line Interface**: Allows users to input a URL and get a classification result.

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/kajal-kiran-01/phishing-detection.git
   cd phishing-detection
   ```
2. Install the required dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Ensure you have `whois` and `requests` installed for URL feature extraction.

## Usage
### Training the Model
Run the following command to train the model and save it:
```sh
python train_model.py
```

### Predicting Website Legitimacy
Run the classifier script and enter a URL when prompted:
```sh
python predict.py
```
Example output:
```
Enter a website URL: www.google.com
The website www.google.com is: Legitimate
```

## File Structure
```
├── phishing.csv            # Dataset
├── train_model.py          # Training script
├── predict.py              # URL classification script
├── phishing_model.pkl      # Trained model file
├── requirements.txt        # Dependencies
├── README.md               # Project documentation
```

## Model Performance
- **Accuracy**: 96.5%
- **Precision, Recall, and F1-score**: See `train_model.py` output for full evaluation.

## License
This project is licensed under the MIT License.

## Contact
For queries, please reach out via GitHub issues or email at `kajal.kiran.cs28@iilm.edu`.

