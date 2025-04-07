# Disease Prediction using Machine Learning

This project aims to accurately classify diseases using a Random Forest model, while also exploring the impact of dimensionality reduction using Principal Component Analysis (PCA).

## Project Goal

The primary goal is to achieve high classification accuracy in disease prediction. Additionally, the project investigates whether similar evaluation metrics can be maintained with a reduced feature set using PCA.

## Dataset

The dataset consists of two CSV files: `Training.csv` and `Testing.csv`. Each file contains 133 columns, where 132 represent symptoms experienced by a person, and the last column indicates the prognosis (disease). The dataset covers 42 different diseases.

## Methodology

1. **Data Preprocessing:**
    - Handling missing values (if any).
    - Visualizing the distribution of the target variable (prognosis).
2. **Model Training:**
    - A Random Forest classifier is trained on the training data.
    - Hyperparameter tuning is performed using RandomizedSearchCV to optimize model performance.
3. **PCA for Dimensionality Reduction:**
    - PCA is applied to reduce the number of features while retaining as much variance as possible.
    - The model is trained again using the reduced feature set.
4. **Evaluation:**
    - Model performance is evaluated using metrics such as accuracy, precision, recall, and F1-score.
    - Confusion matrices are generated to visualize the classification results.

## Results

- Both the original model and the PCA-transformed model achieved 100% accuracy, precision, recall, and F1-score on the test data.
- PCA successfully reduced the number of features from 133 to 65 without significantly impacting model performance.

## Conclusion

Applying PCA for dimensionality reduction proved to be beneficial in this project. It reduced the feature space, leading to computational efficiency without compromising accuracy.

## Future Improvements

- Explore other dimensionality reduction techniques.
- Evaluate the model on a larger and more diverse dataset.
- Implement feature engineering to potentially improve model performance.

## Usage

1. Upload the `Training.csv` and `Testing.csv` files to your Google Colab environment.
2. Execute the notebook cells sequentially to perform data preprocessing, model training, PCA, and evaluation.
3. Review the results and conclusions.

## Author

Samanyu

## Acknowledgments

This project utilizes the scikit-learn library for machine learning tasks and pandas for data manipulation.

## License

[Specify the license if applicable]
