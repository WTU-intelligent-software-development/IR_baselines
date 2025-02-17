#  IR_baselines
The codes about the combination of information retrieval and requirements traceability: VSM and LSI Models.
The datasets are provided by the Center of Excellence for Software & Systems Traceability (CoEST) and can be found at http://www.coest.org/.

#  Environment Setup
python==3.9.13	

chardet==5.2.0	

gensim==4.3.3	

nltk==3.9.1	

pandas==1.3.4	

xlrd==2.0.1	

#  How to Run
This experiment uses the following datasets: iTrust, Albergate, eTOUR, EasyClinic, CM1, EBT subset (RE-TC), WRAC, GANNT.

1. Feature Extraction
For iTrust and Albergate, use JavaParser to extract four types of features (method names, class names, variable names, comments) along with filenames.
For the eTOUR dataset, use regular expressions to extract features.
Run the code in read.py for additional feature extraction (e.g., re, tc, uc features).

2. Feature Combination
Run the combine.py file to combine the features.

3. Data Cleaning
Run Data_clear.py to clean features from datasets.

4. Result Calculation
For the EasyClinic dataset, run Easy_verification.py (with both VSM and LSI).
For other datasets, run verification.py, specifying the file paths for each dataset (both VSM and LSI).
