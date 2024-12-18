# gender-bias-in-headlines

This project implements a machine learning model to detect and analyze gender bias in news articles. Using a combination of lexicon-based analysis and supervised learning techniques, the model identifies various forms of gender bias across different categories of news content.
Overview
The project analyzes news articles for eight distinct categories of gender bias:

- Professional Undermining
- Personal Focus
- Emotional Stereotyping
- Achievement Undermining
- Power Dynamics
- Voice Suppression
- Intersectional Bias

## Usage
The main functionality is in the gender-bias-in-headlines directory. To use the model, enter your text where indicated in this notebook:
```
from bias_detector import BiasClassificationSystem

# Load the model
classifier = BiasClassificationSystem()

# Analyze an article
text = "Your article text here"
result = classifier.predict(text)

# Get bias scores and analysis
print(f"Bias prediction: {'Biased' if result['prediction'] else 'Unbiased'}")
print(f"Confidence: {result['confidence']:.3f}")
```

**Example:**
![image](https://github.com/user-attachments/assets/ff775b61-70ef-4ca5-b407-db44901b9158)
![image](https://github.com/user-attachments/assets/3c8daea1-71fa-4422-bafc-11c33267755d)



## Model Performance
The system uses two classifiers:
Text Classifier (SVM):

Accuracy: 0.940 ± 0.001
Precision: 0.744 ± 0.010
Recall: 0.485 ± 0.012
F1: 0.587 ± 0.008

Category Classifier (Random Forest):

Accuracy: 0.994 ± 0.001
Precision: 0.956 ± 0.004
Recall: 0.977 ± 0.007
F1: 0.967 ± 0.004

## Documentation
For detailed information about the project methodology and findings, please refer to the project report.
