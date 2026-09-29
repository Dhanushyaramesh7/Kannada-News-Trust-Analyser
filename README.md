# Kannada News Trust Analyser

A Kannada news content analysis system that uses a transformer-based NLP model to classify Kannada news headlines into **Neutral, Offensive, and Biased** categories.

## Project Overview

The system uses **Google MuRIL (Multilingual Representations for Indian Languages)**, fine-tuned for Kannada news classification. It also supports speech and image-based inputs by converting them into Kannada text before classification.

### Key Features

- Kannada news classification using **MuRIL**
- Three-class classification:
  - Neutral
  - Offensive
  - Biased
- Speech-to-text using **Whisper**
- Kannada text extraction from images using **EasyOCR**
- Text-to-speech using **gTTS**
- Interactive interface using **Gradio**
- Model evaluation using accuracy, F1-score, and confusion matrix
  
  ## System Workflow
Text Input ────────────────┐
                           │
Speech Input → Whisper ────┤
                           ▼
Image Input → EasyOCR ───→ Kannada Text
                           │
                           ▼
                      MuRIL Model
                           │
                           ▼
              Neutral / Offensive / Biased
  

##Technologies Used:

- Python
- PyTorch
- Hugging Face Transformers
- MuRIL
- Pandas
- Scikit-learn
- OpenAI Whisper
- EasyOCR
- Gradio
- gTTS
- Matplotlib
- Seaborn
##Dataset:

The project uses a Kannada news headline dataset stored in:  data/kannada_news_headlines.csv
The dataset is processed and used to train and evaluate the classification model.
Model
The base model used is:
google/muril-base-cased

The model is fine-tuned for three-class Kannada news classification.

##Project Structure:

Kannada-News-Trust-Analyser/
│
├── data/
│   └── kannada_news_headlines.csv
│
├── Kannada_News_Trust_Analyser_MuRIL.ipynb
├── requirements.txt
├── README.md
└── .gitignore

##How to Run:

The project is developed using Google Colab and is recommended to be run with a GPU runtime.
1. Open the notebook in Google Colab.
2. Install the required dependencies.
3. Provide the Kannada news dataset.
4. Run the preprocessing and training cells.
5. Evaluate the trained model.
6. Use the text, speech, or image input options for classification.
##Evaluation
The model is evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
  
##Future Enhancements:

- Support for additional Indian languages
- Larger and more diverse datasets
- Improved OCR preprocessing
- Real-time speech input
- Web deployment of the classification system
  



Author
Dhanushya Ramesh
IT Engineering Student
Madras Institute of Technology, Anna University
