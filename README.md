Title: CV Job Matching using Doc2Vec

Description:
This project implements a job-matching system using the Doc2Vec algorithm to match resumes with job descriptions based on semantic content. The system preprocesses text data, converts it into vector representations, and computes the cosine similarity using Doc2Vec to quantify the match between candidates' resumes and job descriptions.

Environment Setup:

Python Version: Python 3.8 or above
Required Libraries:
gensim (for Doc2Vec)
nltk (for text processing)
pandas (for data handling)
numpy (for numerical operations)
spacy (for advanced text processing)

Installation:
Install the required Python libraries using pip:

bash
Copy code
pip install gensim nltk pandas numpy spacy
python -m spacy download en_core_web_sm
Data:

Preprocess the data to include only relevant text fields.

Usage:
Load your datasets.
Preprocess the text data (tokenization, removing punctuation, etc.).
Tag the data and train the Doc2Vec model.
Infer vectors for resumes and job descriptions.
Calculate cosine similarity to determine the match.
Save and evaluate the model performance.
Running the Code:
Run the Python script from the command line or an IDE:

bash
Copy code
python cv_job_matching.py
Expected Output:

A trained Doc2Vec model capable of matching resumes to job descriptions.
Similarity scores that quantify how well resumes match job descriptions.

This project extends the capabilities of the basic Doc2Vec model by integrating a deep-learning model to enhance the job-matching process. The model predicts the compatibility of resumes with job descriptions using advanced neural network techniques.

Environment Setup:

Python Version: Python 3.8 or above
Required Libraries:
gensim (for Doc2Vec)
keras (for building the neural network)
sklearn (for data splitting and metrics)
pandas (for data handling)
numpy (for numerical operations)
Installation:
Install the required Python libraries using pip:

bash
Copy code
pip install gensim keras sklearn pandas numpy


Data:
Job descriptions and resume datasets in CSV format.
Ensure data is preprocessed for use in a neural network (tokenization, vectorization).
Usage:

Load and preprocess the datasets.
Train a Doc2Vec model to convert text data to vectors.
Train a deep learning model using the vectors as features.
Evaluate the model using standard classification metrics.
Running the Code:
Execute the script via the command line or an IDE:

bash
Copy code
python advanced_job_matching.py
Expected Output:

A deep learning model trained to predict job-resume match probabilities.

The following GitHub repository goes over 2 specific Tasks:
1. Provide an Accuracy score in matching any Job Description in the dataset with 1 resume, the higher the score, the better the resume is fit for that given job description. 
2. Train a Deep learning model using Doc2Vec, and for any given input of one Job description, produce the best 5 resumes in the dataset for that given job description.


Resume dataset resources:
1. cv_dataset: Full Tech industry resume documents, with current job titles from https://www.kaggle.com/datasets/palaksood97/resume-dataset/data
2. UpdatedResumeDataSet.csv: tech industry resume data in the table, with matching category (e.g. data science, testing) from https://huggingface.co/datasets/Sachinkelenjaguri/Resume_dataset

Job Description Dataset Resources: 
1. DataScientist.csv: tech industry jobs dataset in table


