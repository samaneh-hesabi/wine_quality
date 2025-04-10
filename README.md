# Wine Quality Prediction Project

## Overview
This project aims to predict wine quality using machine learning techniques. The goal is to compare different classification models to determine which one performs best in predicting wine quality based on various chemical properties.

## Dataset
The project uses the WineQT dataset, which contains information about various chemical properties of wines and their quality ratings. The dataset includes features such as:
- Fixed acidity
- Volatile acidity
- Citric acid
- Residual sugar
- Chlorides
- Free sulfur dioxide
- Total sulfur dioxide
- Density
- pH
- Sulphates
- Alcohol

The target variable is 'quality', which is rated on a scale from 3 to 8.

## Project Structure
- `aaa.ipynb`: Jupyter notebook containing the machine learning implementation and analysis
- `WineQT.csv`: Original dataset file
- `WineQT_cleaned.csv`: Cleaned and processed dataset file
- `model_comparison.png`: Visualization of model performance comparison
- `requirements.txt`: Project dependencies
- `environment.yml`: Conda environment configuration

## Methodology

### Data Preprocessing
1. Loaded the dataset using pandas
2. Separated features (X) and target variable (y)
3. Mapped quality ratings to start from 0 (original scale: 3-8, mapped scale: 0-5)
4. Split the data into training (80%) and testing (20%) sets

### Models Implemented
1. **Decision Tree Classifier**
   - Simple tree-based model
   - Uses recursive partitioning to make predictions
   - Good for understanding feature importance

2. **Random Forest Classifier**
   - Ensemble of decision trees
   - Reduces overfitting through bagging
   - Provides feature importance scores

3. **XGBoost Classifier**
   - Gradient boosting framework
   - Handles class imbalance
   - Known for high performance in classification tasks

### Evaluation Metrics
- Accuracy Score
- Classification Report (Precision, Recall, F1-score)

## Results
The project compares the performance of three different machine learning models in predicting wine quality. The results are visualized in a bar plot showing the accuracy scores of each model.

Key findings:
1. The models' performance is compared based on their accuracy scores
2. The visualization clearly shows which model performs best
3. Detailed classification reports provide insights into model performance for each quality class

## How to Run
1. Set up the environment using either:
   - Conda: `conda env create -f environment.yml`
   - pip: `pip install -r requirements.txt`

2. Required dependencies:
   ```
   pandas==2.2.0
   numpy==1.26.4
   matplotlib==3.8.2
   seaborn==0.13.2
   jupyter==1.0.0
   ```

3. Open and run the Jupyter notebook:
   ```
   jupyter notebook aaa.ipynb
   ```

4. The notebook will:
   - Train all three models
   - Print accuracy scores and classification reports
   - Generate and save a comparison plot

## Project Goals
1. Compare different machine learning models for wine quality prediction
2. Identify the most accurate model for this specific task
3. Provide a clear visualization of model performance
4. Demonstrate the application of machine learning in quality prediction

## Future Improvements
1. Feature engineering to improve model performance
2. Hyperparameter tuning for each model
3. Cross-validation to ensure robust results
4. Additional visualization of feature importance
5. Implementation of more advanced models

## Conclusion
This project successfully implements and compares three different machine learning models for wine quality prediction. The results provide valuable insights into which model performs best for this specific task, and the visualization makes it easy to understand the comparison. The project demonstrates the practical application of machine learning in quality prediction and can serve as a foundation for more advanced analysis in the future.
