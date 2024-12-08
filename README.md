# **Crop Recommendation System - Machine Learning Model** 🌱

## **Made by Subrata Dhibar (2nd Year Project)**

This project leverages machine learning techniques to predict the most suitable crops for a given farm based on several environmental factors. The model analyzes input data such as nitrogen (N), phosphorus (P), potassium (K), temperature, humidity, pH, and rainfall to provide tailored recommendations for farmers, thereby aiding in precision agriculture.

### **Technologies Used:**
- **Python**: The main programming language.
- **Machine Learning Libraries**: scikit-learn, joblib
- **Data Analysis**: pandas, numpy, seaborn, matplotlib, plotly
- **Web Interface**: Streamlit for interactive dashboard.

---

## **Project Overview:**

### **Key Features:**
1. **Data Exploration**: The dataset is analyzed for structure, types, and uniqueness. It handles missing values, outliers, and duplicates.
2. **Model Training**: Various machine learning models are trained, including:
   - Logistic Regression (LR)
   - Linear Discriminant Analysis (LDA)
   - K-Nearest Neighbors (KNN)
   - Decision Trees (CART)
   - Gaussian Naive Bayes (NB)
   - Support Vector Machine (SVM)
   - Ensemble Methods like Random Forest, Gradient Boosting, and AdaBoost.
3. **Model Selection**: The most suitable model is chosen based on cross-validation scores, and the model is optimized using grid search.
4. **Evaluation**: The model’s performance is evaluated using confusion matrices, accuracy scores, and classification reports to ensure precision in predictions.
5. **User Interface**: 
   - **Streamlit** is used to create an interactive and user-friendly web interface.
   - Farmers can input various environmental parameters and get the predicted crop recommendations.
   - Features like crop information and working mechanism are included in the sidebar for better user engagement.

---

### **Main Code Structure**:
- **Data Handling**: 
  - The dataset is loaded, duplicates are removed, and outliers are handled for cleaner data.
  - The dataset is split into training and testing subsets.
- **Model Training**:
  - Multiple machine learning models are tested, and the best performing model is selected for crop prediction.
- **Prediction and Output**:
  - The trained model is deployed in a web interface where users can input farm data, and the model will predict suitable crops.
  - The result is displayed in real-time on the web page.
- **Web App Deployment**: 
  - **Streamlit** provides an easy-to-use platform where users can interact with the model, input parameters, and view results instantly.

---

### **Detailed Functionality**:
1. **explore_data()**: 
   - Explores and displays dataset information, including shape, column names, and data types.
   
2. **checking_removing_duplicates()**: 
   - Identifies and removes duplicate records to ensure data quality.

3. **read_in_and_split_data()**: 
   - Splits the dataset into features and labels, then further divides it into training and testing sets.

4. **GetModel()**:
   - Returns a list of machine learning algorithms for model selection.

5. **ensemblemodels()**:
   - Implements ensemble models like Random Forest and AdaBoost to improve prediction accuracy.

6. **NormalizedModel()**:
   - Applies normalization techniques and trains models with different scaling methods like MinMaxScaler and StandardScaler.

7. **fit_model()**:
   - Trains the selected models using cross-validation and computes their accuracy.

8. **classification_metrics()**:
   - Displays model performance with confusion matrices, accuracy, and classification reports.

9. **save_model()**:
   - Saves the trained model for future use using joblib.

10. **Streamlit App**: 
   - The app allows users to input parameters like Nitrogen, Phosphorus, Potassium, Temperature, etc., and get real-time crop recommendations.

---

### **Installation & Setup**:

To run the project locally, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone <repository_url>

2. **INSTALL Dependencies**
   ```bash 
   pip install -r requirements.txt

3. **Run the Streamlit App**
    ```bash 
    streamlit run app.py


### Screenshots:
Web Interface: A clean, interactive dashboard created using Streamlit, where users can input farm data.
Prediction Results: After input, users can view real-time crop recommendations generated by the machine learning model.

### Conclusion:
This Crop Recommendation System is a comprehensive tool for farmers to optimize crop selection based on various environmental factors. The machine learning models provide reliable predictions, contributing to the development of precision agriculture, reducing crop failure risks, and improving farming efficiency.

### Future Work:
Integration with more environmental factors for even more precise predictions.
Expansion of the model to incorporate additional datasets, including historical crop yield data.

### Project Developed By: Subrata Dhibar, 2nd Year, Computer Science Engineering, GIET Gunupur



### Final Step:
After saving your file, you can push the changes to your repository (if using version control like Git):

```bash
git add README.md
git commit -m "Updated README with project details"
git push
    
