# Project Name: Phishing E-mail detection and reply system powered by LLMs

## Introduction:
This project features the utilization of advanced deep learning methodologies, specifically Bidirectional Encoder Representations from Transformers (BERT), in conjunction with Mistral 7B Instruct - a sophisticated Large Language Model (LLM), to detect and counter phishing emails. Our work encompasses data preprocessing, feature extraction, and model training, followed by the evaluation of the model's performance in classifying emails accurately. Furthermore, we showcase responses generated based on the provided input and prompt template. The results indicate that the BERT-based model achieved 99.3\% accuracy in distinguishing between phishing and non-phishing emails.

## Features:
- **Email classification:** We created and trained a BERT model capable of classifying emails with 99.3% accuracy.
- **Reply generation:** We use Mistral 7B Instruct to generate replies based on the provided email.

## Prerequisites:
Before you begin, ensure you have met the following requirements:
- **Python:** We recommend Python 3.9 because running this project requires specific versions of libraries, which are not available on the latest version of Python.
- **Ram:**  Running both models requires at least 8GB of RAM, we recommend 16.

## Installation:
1. **Clone the repository:** `git clone https://github.com/mrmrjing/PhishingEmailClassification.git`
2. **Navigate to the project directory:** `cd PhishingEmailClassification`
3. **Install dependencies:** `pip install -r requirements.txt`
4. **Run the _AntiPhishingSystem.ipynb_ Jupiter notebook**

*Warning* Running the program for the first time will trigger a download of the Mistral 7B model, which takes ~5GB of disk space.

*Warning v2* Git clone will try to download _email_classification_model.h5_ and _combined_data.csv_, which are big files. It might be required to download them separately.

## Usage:
This system takes in a file named _email.json_ and returns _reply.json_, both files have the same structure. See the example:
```bash
{
    "sender": "af25@outlook.com",
    "subject": "Threat detection",
    "body": "Our system indicates that there has been suspicious activity detected on your account and we require your immediate attention to verify your account information to prevent any unauthorized access. Please click on the following link to proceed with the verification process: Failure to verify your account within the next 24 hours may result in temporary suspension or permanent closure of your account."
}
```
