# Medical Appointment No-Shows Analysis

[📊 **Click Here to View the Full Analysis Report (Rendered HTML)**](https://dilgetakasu.github.io/Medical-Appointment-No-Shows/Investigate_Appointment_No_Shows.html)

This project investigates a dataset of 100k medical appointments in Brazil to identify factors associated with patients missing their scheduled appointments ("No-shows"). The analysis focuses on Exploratory Data Analysis (EDA) to uncover trends related to demographics, health conditions, and notification systems.## 📌 Project Overview
* **Goal:** To answer the question: *"What factors are important for us to know in order to predict if a patient will show up for their scheduled appointment?"*
* **Methodology:** Data Wrangling, Cleaning, and Exploratory Data Analysis (EDA) using Python libraries (Pandas, NumPy, Matplotlib).
* **Context:** Developed as part of the Udacity Data Analyst Nanodeg.

## 📂 Dataset Description
The dataset is originally from [Kaggle](https://www.kaggle.com/datasets/joniarroba/noshowappointments). It contains 110,527 medical appointments and its 14 associated variables (characteristics).

**Key Features:**
* `ScheduledDay`: The day the patient set up their appointment.
* `AppointmentDay`: The day of the actual medical appointment.
* `Neighborhood`: Location of the hospital.
* `Scholarship`: Indicates if the patient is enrolled in the *Bolsa Família* welfare program.
* `SMS_received`: 1 or more messages sent to the patient.
* `No-show`: **Target Variable.** (Encoded as 'No' if the patient **showed up**, 'Yes' if they *e linrovided above.

## 🔍 Key Findings & Insights
Based on the exploratory analysis, the following trends were observed:

1.  **Impact of SMS Reminders:** Patients who received an SMS reminder were significantly more likely to show up compared to those who did not.
2.  **Age Factor:** Younger patients (especially young adults) tend to miss appointments more frequently than older demographics.
3.  **Wait Time:** While not explicitly modeled in this EDA, preliminary observation suggests a relationship between the time gap (Scheduled vs. Appointment day) and cancellation rates.
4.  **Gender:** Gender does not appear to be a strong differentiator for no-show behavior; distributions aremilar for both groups.

## ⚠️ Limitations
* **Correlation vs. Causation:** This analysis relies on descriptive statistics. While we can observe correlations (e.g., between SMS and attendance), we cannot imply causation without controlled experiments.
* **Data Period:** The data covers a specific period (approx. 3 months). Seasonality or specific events in Brazil during that time might bias the results.
* **Distance:** We lack data on the distance between the patient's home and the clinic, which c be a major hidden factor.

## 🛠️ Technologies Used
* **Python 3**
* **Pandas** (Data manipulation)
* **NumPy** (Numerical operations)
* **Matplot / Seaborn** (Data Visualization)

## 🚀 How to Run
1.  Clone the repository.
2.  Download the dataset from Kaggle and place it in the project root.
3.  Install dependencies:
    ```bash
    pip install pandas numpy matplotlib seaborn
    ```
4.  Run the Jupyter Notebook:
    ```bash
    jupyter notebook Investigate_a_Dataset.ipynb
    ```