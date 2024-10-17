
# CNN on Student Performance Dataset

This project applies **Convolutional Neural Networks (CNNs)** to a numerical dataset from a famous educational website (Kaggle). Two different CNN architectures are implemented to predict students' exam scores based on various factors such as parental involvement, access to resources, extracurricular activities, and more. Performance metrics like **Accuracy**, **F1 Score**, and **Precision** are calculated and visualized to evaluate the models.

## Dataset

The dataset contains several factors affecting student performance, including:
- **Categorical variables** such as `Parental_Involvement`, `School_Type`, `Gender`, etc.
- **Numerical variables** like `Hours_Studied`, `Attendance`, `Sleep_Hours`, etc.

The target variable is the `Exam_Score`, which we aim to predict using CNNs.

### Preprocessing Steps:
1. **Label Encoding**: Categorical columns are converted to numeric values using label encoding.
2. **Standardization**: Numerical columns are normalized using `StandardScaler`.
3. **Reshaping**: The data is reshaped to a 3D format `(samples, features, 1)` suitable for CNN models.

## Models

Two different CNN models are used:

### Model 1 (Simple CNN):
- 1 Convolutional Layer (32 filters, kernel size 3)
- MaxPooling Layer (pool size 2)
- Flatten Layer
- Dense Layer (64 units, ReLU activation)
- Output Layer (1 unit for regression)

### Model 2 (Deeper CNN):
- 1 Convolutional Layer (64 filters, kernel size 3)
- MaxPooling Layer (pool size 2)
- Dropout Layer (20% dropout)
- 1 Convolutional Layer (32 filters, kernel size 3)
- MaxPooling Layer (pool size 2)
- Flatten Layer
- Dense Layer (128 units, ReLU activation)
- Output Layer (1 unit for regression)

Both models use the **Adam** optimizer and **mean squared error** as the loss function.

## Results

### Model Performance:
After training the models for 10 epochs, the following results were obtained:

| Metric      | Model 1 | Model 2 |
|-------------|---------|---------|
| **Accuracy**| 17.40%  | 15.51%  |
| **F1 Score**| 17.42%  | 14.98%  |
| **Precision**| 17.50% | 16.41%  |

The models showed low accuracy, F1 scores, and precision, highlighting that CNNs are not typically well-suited for numerical data.

### Performance Visualization:
The validation loss comparison of both models is visualized using `matplotlib`:

```python
plt.plot(history_1.history['val_loss'], label='Model 1 Validation Loss')
plt.plot(history_2.history['val_loss'], label='Model 2 Validation Loss')
plt.title('Validation Loss Comparison')
plt.legend()
plt.show()
```

## CNN for Numerical Data - Explanation

CNNs are primarily used for image data or sequential data, where local dependencies are important (like pixels in an image or words in a sentence). When applied to numerical data, CNNs can still learn patterns, but they may not capture the relationships between features as effectively as other models like decision trees or linear models.

In this project:
- **Why CNN?**: By reshaping the numerical data into a 3D format, we allow CNNs to try learning local patterns across features, treating them as analogous to pixels in an image.
- **Limitations**: CNNs often struggle with tabular/numerical data, where feature relationships may not be spatially structured. This is reflected in the lower performance of both models.

## How to Run

1. Install required packages:
    ```bash
    pip install numpy pandas scikit-learn tensorflow matplotlib
    ```

2. Run the Python script to train the CNN models and evaluate the results:
    ```bash
    python cnn_student_performance.py
    ```

## Dependencies

- Python 3.x
- TensorFlow
- scikit-learn
- Matplotlib
- Pandas
- NumPy

## Conclusion

This project demonstrates that CNNs, although powerful for image processing, are not typically ideal for numerical/tabular datasets. While CNNs can be used for numerical data by reshaping it to fit a convolutional structure, other models like Random Forests or Gradient Boosted Trees are often more effective for such tasks.

---
