# Classification of the emotional state of a human by extracting facial features

Our project aims to classify the emotional state of a person, given his/her image, in the following 7 standard 
categories: anger, disgust, joy, neutral, sadness, surprise, and fear. The emotional state of the person is purely on 
the basis of the facial expressions portrayed in the image. This finds a lot of application in numerous domains like 
Transportation (to avoid rage driving), help machines understand the emotional state of the person to provide 
appropriate recommendations (soothing music when one is sad), Marketing (impact of ads on the person), etc.

# Instructions
Run make_model_and_test.py for XGBoost
Run make_logistic_regression_model_and_test.py for Logistic Regresssion

# File Structure
src
 ├── make_dataframe.py
 ├── utils.py
 ├── ext_faces.py
 ├── get_linear_features.py
 ├── get_trig_features.py
 ├── get_elliptical_features.py
 ├── get_landmarks.py
 └── 

Brief about the files:

1. make_dataframe.py          : The main file which when run, outputs a dataframe in the form of a csv.
2. utils.py                   : Following the DRY principle, commonly used functions have been put in this file.
3. ext_faces.py               : Extracts faces, rescaling, grayscaling and saving.
4. get_landmarks.py           : 
4. get_linear_features.py     : Contains functions that compute the linear features.
5. get_trig_features.py       : Contains functions that compute the trigonometric features.
6. get_elliptical_features.py : Contains functions that compute the eccentricity of ellipses.