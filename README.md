<h1>📉 Customer Churn Prediction</h1>

<p>
Customer Churn Prediction is an end-to-end machine learning project focused on predicting whether a customer will leave a company.
The project uses demographic and billing data to build a binary classification model and deploys it as an interactive Streamlit web application.
</p>

<hr>

<h2>🎯 Business Problem</h2>

<p>
Customer churn is a critical challenge for businesses, especially in the telecommunications industry.
Early churn prediction helps companies reduce revenue loss and improve customer retention by taking proactive actions.
</p>

<hr>

<h2>📊 Dataset</h2>

<p>
The project uses the dataset <b>customer_churn_data.csv</b>.
</p>

<h3>Target Variable</h3>
<ul>
  <li><b>Churn</b>: 1 — Customer churned, 0 — Customer retained</li>
</ul>

<h3>Features Used</h3>
<ul>
  <li><b>Age</b> — Customer age</li>
  <li><b>Gender</b> — Customer gender (Female = 1, Male = 0)</li>
  <li><b>Tenure</b> — Length of customer relationship</li>
  <li><b>MonthlyCharges</b> — Monthly billing amount</li>
</ul>

<hr>

<h2>🔍 Exploratory Data Analysis (EDA)</h2>

<p>
Exploratory data analysis was performed to understand customer behavior and identify factors influencing churn.
The analysis included checking missing values and duplicates, visualizing churn distribution, and analyzing relationships
between churn and numerical features.
</p>

<p>
Key insights:
</p>
<ul>
  <li>Customers with shorter tenure are more likely to churn</li>
  <li>Monthly charges have a significant impact on churn behavior</li>
  <li>Age and gender also contribute to churn patterns</li>
</ul>

<hr>

<h2>🧠 Machine Learning Pipeline</h2>

<h3>Data Preprocessing</h3>
<ul>
  <li>Encoding categorical features</li>
  <li>Feature scaling using <b>StandardScaler</b></li>
  <li>Train-test split (80% training, 20% testing)</li>
</ul>

<p>
The fitted scaler is saved as <b>scaler.pkl</b>.
</p>

<h3>Model Training and Evaluation</h3>

<p>
The following machine learning models were trained and evaluated:
</p>

<ul>
  <li>Logistic Regression</li>
  <li>K-Nearest Neighbors (GridSearchCV)</li>
  <li>Support Vector Machine (GridSearchCV)</li>
  <li>Decision Tree (GridSearchCV)</li>
  <li>Random Forest (GridSearchCV)</li>
</ul>

<p>
Model performance was evaluated using the <b>accuracy score</b>.
</p>

<hr>

<h2>🏆 Model Selection</h2>

<p>
After hyperparameter tuning and evaluation, the best-performing model selected for deployment is:
</p>

<ul>
  <li><b>Support Vector Classifier (SVC)</b></li>
</ul>

<p>
The trained model is saved as <b>model.pkl</b>.
</p>

<hr>

<h2>🖥️ Web Application</h2>

<p>
The trained model and scaler are deployed using <b>Streamlit</b>.
The web application allows users to input customer information and receive churn predictions in real time.
</p>

<hr>

<h2>🛠️ Tech Stack</h2>

<ul>
  <li>Python</li>
  <li>Pandas</li>
  <li>NumPy</li>
  <li>Matplotlib</li>
  <li>Scikit-learn</li>
  <li>Joblib</li>
  <li>Streamlit</li>
</ul>

<hr>

<h2>📁 Project Structure</h2>

<pre>
Customer_Churn_Prediction/
│
├── app.py
├── model.pkl
├── scaler.pkl
├── customer_churn_data.csv
├── requirements.txt
└── README.md
</pre>

<hr>

<h2>⚙️ Installation & Usage</h2>

<pre>
pip install -r requirements.txt
streamlit run app.py
</pre>

<hr>

<h2>🔮 Future Improvements</h2>

<ul>
  <li>Add churn probability output</li>
  <li>Use additional evaluation metrics (ROC-AUC, F1-score)</li>
  <li>Model interpretability using SHAP</li>
  <li>Extend feature set</li>
  <li>Cloud deployment</li>
</ul>

<hr>

<h2>👩‍💻 Author</h2>

<p>
This project was developed for learning and portfolio purposes to demonstrate skills in Data Science and Machine Learning.
</p>
