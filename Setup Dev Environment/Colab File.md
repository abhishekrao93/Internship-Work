Please find the link below to the Colab Notebook for the Quality rating Bar Chart.

https://colab.research.google.com/drive/1X8MrzVSodmpNxzYhNqsz7-ytHvBANRkf?usp=sharing

Steps to load the Dataset in Colab:

1) In Your kaggle account, go to the API section and create a new API Token and download the kaggle.json file
2) Upload the kaggle File in a folder
3) Create a new Jupyter Notebook and Mount your Google Drive
4) Provide the config path to the JSON File and then change the working directory
5) Download the kaggle dataset using the below command:
6) unzipping the zip files and deleting the zip files using the below command 
7) Ready to start working on the Task. 

# Commands to implement the above:

from google.colab import drive
drive.mount('/content/gdrive')
import os
os.environ['KAGGLE_CONFIG_DIR'] = "/content/gdrive/My Drive/Kaggle"
%cd /content/gdrive/My Drive/Kaggle
!kaggle datasets download -d "API Link"
!unzip \*.zip  && rm *.zip
