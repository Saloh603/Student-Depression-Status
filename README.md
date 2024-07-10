# Student-Depression-Status

## Project Overview
The Student Depression Status project is a machine learning-based application designed to measure the depression index of students based on various factors such as age, gender, academic performance, social habits, and lifestyle choices. This tool utilizes Python along with libraries like sklearn, joblib, numpy, and pandas to predict the depression index, categorized into three levels: low (0), moderate (1), and high (2).

## Features
1. Predictive modeling using sklearn
2. Data handling with pandas and numpy
3. Serialization of models using joblib
4. API for easy payload interaction

## Installation
Ensure that you have Python installed on your system. You can download Python from here.

To set up this project locally, follow these steps:
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/student-depression-status.git
   cd student-depression-status
   ```
2. Install required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
To use the API, you need to send a JSON payload with the student's data. Below is an example of how to use the API with Python:
  ```python
  import requests
  
  url = "http://localhost:5000/predict"  # Replace with the correct URL if hosted
  payload = {
      'Age': 23,
      'Gender': 'Male',
      'AcademicPerformance': 'Excellent',
      'TakingNoteInClass': 'Sometimes',
      'FaceChallangesToCompleteAcademicTask': 'No',
      'LikePresentation': 'Yes',
      'SleepPerDayHours': 8,
      'NumberOfFriend': 80.0,
      'LikeNewThings': 'Yes'
  }
  
  response = requests.post(url, json=payload)
  print("Depression Index Level:", response.json())
```

## Model Details
This section explains the criteria and the methodology used for training the model along with its accuracy and performance metrics. (Please include specifics about the model training, data used, evaluation metrics, etc.)

## Contributing
We welcome contributions from the community. If you wish to contribute to this project, please fork the repository and submit a pull request.
