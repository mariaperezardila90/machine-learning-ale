# Machine Learning Course Project

# Author: Alejandra Perez

This project is part of the **Practical Machine Learning** course, where a **Random Forest model** is trained to classify human activity based on sensor data.

# 📂 Project Structure

- **`pml-training.csv`**: Training dataset used for model building.
- **`pml-testing.csv`**: Testing dataset for final predictions.
- **`Machine.html`**: HTML report containing analysis and results.
- **`final_predictions.csv`**: Output file with predictions for the test set.
- **`machine_learning_project.Rmd`**: R Markdown script with the full implementation.

# 📊 Methodology

1. **Data Preprocessing**:
   - Load training and testing datasets.
   - Remove variables with too many missing values.
   - Remove irrelevant identifier columns.
   - Convert the target variable (`classe`) into a factor.

2. **Data Splitting**:
   - The training dataset is split into **75% training data** and **25% validation data**.

3. **Model Training**:
   - A **Random Forest model** is trained using cross-validation (`cv = 5`).

4. **Model Evaluation**:
   - The trained model is tested on the validation dataset.
   - Performance is evaluated using a **confusion matrix**.

5. **Predictions on the Test Set**:
   - The trained model predicts on the test dataset.
   - Results are saved in `final_predictions.csv`.

# 🚀 Results & Future Improvements

- The **Random Forest model** provides robust classification.
- Future improvements may include:
  - Trying **Gradient Boosting** or **Neural Networks**.
  - Exploring **feature engineering** techniques.

# 🔧 Installation & Dependencies

To run this project, you need the following **R libraries**:

```r
install.packages(c("caret", "randomForest", "ggplot2"))
