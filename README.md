# Heart Attack Dataset Poisoning Experiment

This project evaluates the impact of label poisoning on the performance of various machine learning models using the "Heart Attack" dataset.

## Dataset
The dataset used in this project includes the following columns:
- `age`: Age of the individual
- `gender`: Gender of the individual
- `impluse`: Heart rate or pulse
- `pressurehight`: High blood pressure reading
- `pressurelow`: Low blood pressure reading
- `glucose`: Glucose level
- `kcm`: Cholesterol level
- `troponin`: Troponin level
- `class`: Target class (`positive` or `negative` for heart attack)

## Dependencies
The following libraries are required to run the code:
- Python 3.6+
- Pandas
- NumPy
- scikit-learn
- Matplotlib

## Code Description

1. **Data Loading**:
   The dataset is loaded using `pandas`. The first few rows are displayed to understand its structure.

2. **Preprocessing**:
   - Features (`X`) and target labels (`y`) are separated.
   - Categorical columns are encoded using `LabelEncoder`.
   - The target labels are also encoded: `positive` → `1`, `negative` → `0`.

3. **Model Training**:
   The following models are trained on the dataset:
   - Support Vector Machine (SVM)
   - Logistic Regression
   - Random Forest Classifier
   - Decision Tree Classifier

4. **Evaluation**:
   - Models are first trained and evaluated on clean data (0% poisoning).
   - Label poisoning is simulated at rates of 5%, 10%, and 20% by flipping a portion of the training labels to incorrect values.
   - The accuracy of each model is evaluated after training on the poisoned datasets.

5. **Visualization**:
   - The accuracy of each model at different poisoning rates is plotted.

## Results
The accuracy results for each model at various poisoning rates are summarized below:

| Model                | Clean Data | 5% Poisoning | 10% Poisoning | 20% Poisoning |
|----------------------|------------|--------------|---------------|---------------|
| **SVM**             | 0.69       | 0.68         | 0.67          | 0.64          |
| **Logistic Regression** | 0.78       | 0.76         | 0.73          | 0.70          |
| **Random Forest**    | 0.99       | 0.98         | 0.98          | 0.98          |
| **Decision Tree**    | 0.99       | 0.93         | 0.87          | 0.78          |

## Usage

### Running the Code
1. Ensure all dependencies are installed:
   ```bash
   pip install pandas numpy scikit-learn matplotlib
