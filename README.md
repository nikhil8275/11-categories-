

🌐 Website Category Prediction Using Multi-Label Classification
This project uses machine learning to classify websites into multiple categories by extracting and analyzing their textual content. It combines TF-IDF vectorization, Random Forest classification, and real-time web scraping to provide accurate multi-label predictions.

📁 Project Workflow
1. Data Preparation
The dataset includes fields like text, html_title, h1, h2, and p representing different parts of a webpage. These fields are merged into a single text column to create a unified input for each website.

2. Text Cleaning
All text data is cleaned by converting to lowercase, removing special characters, and normalizing white spaces. This ensures consistent formatting for vectorization.

3. Vectorization
The cleaned text is converted into numerical features using TF-IDF vectorization. This helps represent the importance of terms in documents relative to the whole dataset.

4. Model Training
A Random Forest classifier is trained on the TF-IDF-transformed data. The model is capable of handling multi-label outputs, meaning each sample can be associated with more than one category.

5. Thresholding for Multi-Label Prediction
Predicted probabilities are converted into binary labels using a defined threshold (e.g., 0.7). This step helps determine which categories a website belongs to based on confidence levels.

6. Model Evaluation
The model is evaluated using precision, recall, F1-score, and support metrics for each label. This helps assess the performance across all categories individually.

7. Live Website Prediction
The project includes a utility that scrapes a given URL, extracts meaningful content, and runs it through the trained model. The output shows predicted categories and their associated confidence scores.


The trained Random Forest model used for classification is larger than 25MB and cannot be directly uploaded to GitHub.
You can download the model file from the link below:
🔗 Download Trained Model (https://drive.google.com/file/d/1fu4vzMkCfubaTwxdguqFVEgpYgZZIx2W/view?usp=drive_link.pkl)

🔗 Download Trained Model (https://drive.google.com/file/d/1wwBYNgpwNwk23z62u-RPeMhANbz09VG_/view?usp=drive_link.pkl)

