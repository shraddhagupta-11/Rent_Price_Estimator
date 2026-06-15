# 🏠 Rent Price Estimator

A Machine Learning project that predicts monthly apartment rent prices in major Indian cities using housing rental data and regression models.

---

## 📖 About the Project

Determining the right rental price for a property can be challenging because many factors influence rent, including apartment size, location, furnishing status, tenant preferences, and the number of bedrooms and bathrooms.

This project uses Machine Learning techniques to analyze historical rental listings and estimate monthly rent based on apartment characteristics.

The project was built to demonstrate the complete machine learning workflow, including:

- Data Collection
- Data Cleaning
- Exploratory Data Analysis (EDA)
- Data Visualization
- Feature Engineering
- Model Training
- Model Evaluation
- Interactive Rent Prediction

---

## ⭐ Project Highlights

- Analyzed more than 4,700 apartment rental listings.
- Performed data cleaning and preprocessing.
- Created visualizations to understand rental market trends.
- Trained and compared Linear Regression and Random Forest models.
- Selected Random Forest as the final model based on performance.
- Achieved an R² Score of 0.754.
- Built an interactive rent prediction system.
- Developed entirely using Python and Google Colab.

---

## 📂 Dataset Source

This project uses the House Rent Prediction Dataset available on Kaggle.

Dataset Link:

https://www.kaggle.com/datasets/iamsouravbanerjee/house-rent-prediction-dataset

The dataset contains more than 4,700 apartment rental listings across multiple Indian cities.

Features available in the dataset include:

- Rent
- BHK
- Apartment Size
- City
- Furnishing Status
- Tenant Preference
- Number of Bathrooms

The dataset was used for educational and portfolio purposes.

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Joblib
- Google Colab

---

## 🔍 Project Workflow

### 1. Data Loading

The rental dataset is loaded into a Pandas DataFrame for analysis.

### 2. Data Cleaning

The dataset is cleaned by:

- Removing duplicate records
- Removing unnecessary columns
- Filtering extreme rent outliers
- Preparing data for machine learning

### 3. Exploratory Data Analysis (EDA)

Visualizations were created to study:

- Rent distribution
- Average rent by city
- Furnishing status impact
- Apartment size vs rent
- Feature correlations

### 4. Feature Engineering

Categorical variables such as city names and furnishing status were converted into numerical values using Label Encoding.

### 5. Model Training

Two machine learning models were trained and compared:

- Linear Regression
- Random Forest Regressor

### 6. Model Evaluation

Model performance was evaluated using:

- R² Score
- Mean Absolute Error (MAE)

### 7. Rent Prediction

An interactive prediction function allows users to estimate rent based on apartment details.

---

## 📈 Model Performance

### Random Forest Regressor

| Metric | Result |
|----------|----------|
| R² Score | 0.754 |
| Mean Absolute Error (MAE) | ₹11,008 |

### Interpretation

The model explains approximately **75.4% of the variation in rental prices** within the dataset.

On average, predictions differ from actual rental prices by approximately **₹11,008 per month**.

These results demonstrate a solid baseline model for rental price prediction using publicly available housing data.

---

## 🏙 Supported Cities

The current model was trained on apartment listings from:

- Bangalore
- Chennai
- Delhi
- Hyderabad
- Kolkata
- Mumbai

Predictions can only be generated for cities that were present in the training data.

---

## 🧪 Example Prediction

### Input

| Feature | Value |
|----------|----------|
| BHK | 2 |
| Size | 1000 sq ft |
| City | Bangalore |
| Furnishing Status | Semi-Furnished |
| Tenant Preference | Family |
| Bathrooms | 2 |

### Predicted Output

**₹16,767 per month**

---

## 📁 Project Structure

```text
rent-price-estimator/
│
├── Rent_Price_Estimator.ipynb
├── requirements.txt
├── cleaned_rent_data.csv
├── rent_model.pkl
├── label_encoders.pkl
└── README.md
```

### File Description

| File | Description |
|--------|-------------|
| Rent_Price_Estimator.ipynb | Main notebook containing all code, visualizations, training, evaluation and predictions |
| requirements.txt | List of Python dependencies |
| cleaned_rent_data.csv | Cleaned dataset generated during preprocessing |
| rent_model.pkl | Trained Random Forest model |
| label_encoders.pkl | Saved encoders used for categorical variables |
| README.md | Project documentation |

---

## ▶️ Installation & Execution Guide

### Option 1: Run Using Google Colab (Recommended)

No installation is required.

#### Step 1

Open Google Colab:

https://colab.research.google.com

#### Step 2

Upload:

```text
Rent_Price_Estimator.ipynb
```

#### Step 3

Download the dataset from Kaggle:

https://www.kaggle.com/datasets/iamsouravbanerjee/house-rent-prediction-dataset

#### Step 4

Upload:

```text
House_Rent_Dataset.csv
```

to Google Colab.

#### Step 5

Run all notebook cells sequentially from Cell 1 through Cell 15.

#### Step 6

Enter apartment details in the prediction section to receive a rent estimate.

---

### Option 2: Run Locally on Your Computer

#### Requirements

- Python 3.10 or newer
- Jupyter Notebook
- VS Code (optional)

#### Install Dependencies

Open a terminal and run:

```bash
pip install -r requirements.txt
```

Or install manually:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn joblib
```

#### Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/rent-price-estimator.git
```

#### Move into the Project Folder

```bash
cd rent-price-estimator
```

#### Start Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
Rent_Price_Estimator.ipynb
```

and run all cells from top to bottom.

---

## 🎯 Learning Outcomes

This project provided hands-on experience with:

- Python Programming
- Data Cleaning
- Data Visualization
- Exploratory Data Analysis
- Feature Engineering
- Regression Models
- Random Forest Algorithms
- Model Evaluation
- Machine Learning Workflows
- Google Colab
