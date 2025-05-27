# 🏠 House Price Prediction System

A complete end-to-end **AI-powered house price prediction system** that emphasizes both model performance and real-world deployability using **MLOps best practices**.  this project walks through every stage—from data analysis and engineering to model deployment.

## 💡 Project Highlights

- 🧠 Built with practical **MLOps principles** to simulate a real-world AI project
- 🏗️ Uses the **Factory Design Pattern** for scalable data ingestion
- 📊 Performs in-depth **data analysis and visualization**
- 🧹 Implements robust strategies for **missing data handling**
- 🧪 Trains a regression model with a focus on interpretability
- 🚀 Includes a **deployment-ready pipeline** with dynamic model loading

---

## 🧰 Tech Stack

| Component          | Technology             |
|--------------------|------------------------|
| Programming        | Python                 |
| Data Processing    | Pandas, NumPy          |
| Visualization      | Matplotlib, Seaborn    |
| Machine Learning   | Scikit-learn           |
| Web Framework      | Flask                  |
| Deployment         | REST API (Flask)       |
| MLOps Concepts     | Factory Pattern, Pipelines |

---

## 🗂️ Project Structure

house-price-prediction/
├── app.py # Flask app for web interface and inference
├── artifacts/ # Folder for model artifacts (e.g., .pkl files)
├── data/ # Raw and processed data files
├── model_training.ipynb # EDA and model training notebook
├── src/
│ ├── init.py
│ ├── components/ # Data ingestion, transformation, etc.
│ ├── config/ # Configuration and schema definitions
│ ├── pipelines/ # Training and prediction pipelines
│ └── utils/ # Helper functions and classes
├── templates/
│ └── index.html # Frontend for predictions
├── static/
│ └── style.css # Styles for the web app
├── requirements.txt
└── README.md

yaml


---

## 🚀 How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/pebin_Joseph/house-price-prediction.git
cd house-price-prediction
2. Install Dependencies

pip install -r requirements.txt
3. Prepare the Data
Place the dataset (housing.csv) in the data/ directory.

If zipped, extract it manually or use Python utilities from the project.

4. Train the Model
Run the training pipeline from Jupyter Notebook:


jupyter notebook model_training.ipynb
Or, run a Python training script if available:


python src/pipelines/train_pipeline.py
5. Start the Flask App

python app.py
Go to http://127.0.0.1:5000 in your browser.

📈 Data Analysis & Insights
Heatmaps for missing value inspection (yellow = missing, purple = valid)

Distribution plots for key features

Correlation analysis shows Overall Quality and Living Area as strong predictors

Handling missing values using:

Dropping (rows/columns based on threshold)

Imputation (mean, median, mode, constant)

Visual outlier detection and impact on target variable

🧱 MLOps & Design Principles
✅ Factory Design Pattern for clean data ingestion and transformation

⚙️ Modular architecture to easily add new preprocessing or model components

🧪 Abstract model interface for future expansion (e.g., XGBoost, CatBoost)

🔁 Model retraining and deployment via continuous deployment pipeline

📦 Dynamic model loader for real-time inference

🧪 Sample Prediction
Input:

Area: 3000 sq. ft

Bedrooms: 4

Bathrooms: 3

Location: Bangalore

Output:

Predicted Price: ₹75.2 Lakhs

🎯 Future Enhancements
Deploy on cloud platforms (AWS, Heroku, etc.)

Add model monitoring and logging

Integrate CI/CD pipeline

Implement user authentication for access control

🤝 Contributing
Feel free to fork this repo, raise issues, or submit pull requests.

📄 License
This project is licensed under the MIT License.
