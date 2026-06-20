# experience-to-salary-model
# Experience-Based Salary Predictor

A straightforward machine learning project that predicts an employee's salary based on their years of experience using Simple Linear Regression. 

## Dataset Description
The model is trained on `Salary_dataset.csv`, which contains continuous numerical data. The primary features used are:
* **YearsExperience:** The independent variable (X) representing the number of years an individual has worked.
* **Salary:** The dependent target variable (y) representing the compensation amount.

## Methodology
1. **Data Ingestion & Cleaning:** Loaded the dataset using Pandas and verified the absence of null values to ensure data integrity.
2. **Data Splitting:** Partitioned the data into training (80%) and testing (20%) sets using Scikit-learn's `train_test_split` to allow for objective model evaluation.
3. **Modeling:** Instantiated and trained a `LinearRegression` model on the training data.

## Results & Insights
The trained Simple Linear Regression model identified a strong positive correlation between experience and compensation. 
* **Model Coefficient (Slope):** ~9,423.82 (Indicating that for every additional year of experience, the expected salary increases by this amount).
* **Model Intercept:** ~24,380.20 (The baseline starting salary for zero years of experience according to the model's line of best fit).
* **Prediction:** The model successfully outputted continuous predictions for the test set, mapping closely to the actual recorded salaries.

## How to Run Locally
1. Clone this repository to your local machine.
2. Ensure you have Python installed along with the required libraries: `pip install numpy pandas scikit-learn jupyter`.
3. Place `Salary_dataset.csv` in the same directory as the notebook.
4. Open your terminal or command prompt, navigate to the folder, and run `jupyter notebook`.
5. Open `experience-to-salary-model.ipynb` and run the cells sequentially.
