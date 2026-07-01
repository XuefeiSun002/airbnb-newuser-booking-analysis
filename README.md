# Airbnb New User Booking Conversion Analysis

## Project Overview

This project analyzes Airbnb new user booking behavior using user profile data and web session logs from the Kaggle Airbnb New User Bookings dataset.

The goal is to understand what factors influence a new user's first booking conversion, identify key drop-off points in the user journey, and build a machine learning model to predict booking tendency.

Main business questions:

1. Which acquisition channels bring higher-quality users?
2. Which user groups are more likely to complete their first booking?
3. Where is the major drop-off point in the booking funnel?
4. Can we predict whether a new user will complete their first booking?

---

## Dataset

Data source: Kaggle Airbnb New User Bookings.

Main files used:

- `train_users_2.csv`: user profile and booking destination data
- `sessions.csv`: user web session behavior logs
- `countries.csv`: destination country information
- `age_gender_bkts.csv`: age, gender and destination summary data

The target variable is:

```text
is_booked = 1 if country_destination != "NDF"
is_booked = 0 if country_destination == "NDF"
Raw data is not uploaded due to Kaggle competition rules. Please download the dataset from Kaggle and place it under data/raw/.
---

## Notebook

The full analysis is included in one Jupyter Notebook:

- `notebooks/Airbnb_New_User_Booking_Analysis.ipynb`

The notebook includes data cleaning, feature engineering, exploratory analysis, behavior funnel analysis, high-intent user segmentation, and booking prediction modeling.
