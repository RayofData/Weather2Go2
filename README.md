# Weather2Go2

**Weather2Go2** is a Python machine learning project that estimates **weather-related driving risk** for a planned trip in Michigan.

This project is a revised version of my original [Weather2Go / SpartaHack 11 hackathon project](https://github.com/RayofData/Weather2Go_Spartahack11) The original demo proved the concept, but it tended to classify too many conditions as high risk. In this version, I improved the data strategy by using two sources:

* [**Kaggle US Accidents data**](https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents) to learn patterns from hazardous driving conditions
* [**Open-Meteo API weather data**](https://www.weather.gov/documentation/services-web-api) for 30 Michigan cities to represent normal and safer driving conditions

This helped improve accuracy and produce more realistic predictions instead of labeling nearly every situation as high risk.

---

## What It Does

Given a Michigan city, date, time, and live weather conditions, the app outputs:

* A **5-level driving risk category**

  * Low
  * Moderate-Low
  * Moderate
  * Heavy
  * Severe
* A short weather summary
* Safety guidance based on the predicted risk level

The model focuses on **weather-driven driving risk**, not crash prediction, insurance scoring, or individual driver behavior.

---

## Project Scope

* **Geography:** Michigan only
* **Cities:** 30 Michigan cities
* **Model:** Random Forest classifier
* **Interface:** Streamlit web app
* **Purpose:** Data science portfolio project

---

## Tech Stack

* Python
* pandas
* NumPy
* scikit-learn
* Random Forest
* Open-Meteo API
* Streamlit

---

## Current Status

The project is a functional end-to-end demo.

The app:

* Fetches live weather data
* Converts weather data into model features
* Predicts a 5-level driving risk score
* Displays weather summaries and safety guidance

This version meets the intended portfolio goal and demonstrates data sourcing, feature engineering, supervised modeling, model evaluation, deployment, and user-facing interpretation.

---

## Disclaimer

This project is for **educational and demonstration purposes only**. It does not provide real-world driving, safety, legal, or insurance advice.
