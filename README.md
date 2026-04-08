# Mobile Phone Price Range Classification 📱💰

## 📌 Project Overview
This project aims to classify mobile phones into four distinct price ranges (0: Low, 1: Medium, 2: High, 3: Very High) based on their hardware specifications. This is a multi-class classification problem designed to help mobile phone companies estimate the price segment of a new device based on its features.

## 💼 Business Problem
Price estimation is a crucial task for mobile phone manufacturers. By analyzing competitive features such as RAM, Battery Power, and Camera quality, companies can strategically position their products in the market. This project utilizes machine learning to automate this classification process with high accuracy.

## 📊 Dataset Description
The dataset contains 2,000 records with 21 features. Key attributes include:
- **RAM**: Random Access Memory in MB.
- **Battery Power**: Total energy a battery can store (mAh).
- **Internal Memory**: Storage capacity in GB.
- **Camera (FC/PC)**: Front and Primary camera megapixels.
- **Display**: Screen height, width, and resolution (px_height/px_width).
- **Connectivity**: Support for 4G, 3G, Bluetooth, and WiFi.
- **Price Range (Target)**: 0 (low cost), 1 (medium cost), 2 (high cost), 3 (very high cost).

## 🛠️ Technical Stack
- **Language:** Python
- **Libraries:** - Data Analysis: `pandas`, `numpy`
  - Visualization: `matplotlib`, `seaborn`
  - Machine Learning: `scikit-learn` (Decision Tree, Random Forest, SVM)

## 🚀 Project Workflow
1.  **Exploratory Data Analysis (EDA):** Analyzed feature distributions and correlations. Identified that **RAM** has the strongest positive correlation (~0.91) with the price range.
2.  **Data Preprocessing:** Handled invalid records (e.g., filtering out zero screen width/height) and applied `MinMaxScaler` for feature normalization.
3.  **Modeling:** Implemented and compared multiple classifiers:
    - **Decision Tree**
    - **Random Forest** (with Hyperparameter Tuning)
    - **Support Vector Machine (SVM)** (using GridSearchCV)
4.  **Evaluation:** Models were evaluated based on Accuracy, Precision, Recall, and F1-Score.
5.  **Prediction:** Developed an interactive script to predict the price group for new mobile data.

## 📈 Key Results
- **SVM Classifier:** Achieved the highest performance (typically >95% accuracy) after hyperparameter tuning using RBF kernel.
- **Feature Importance:** RAM, Battery Power, and Pixel resolution were the most significant predictors of price.

  
