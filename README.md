# Multi-Perspective Fraud Detection for E-Commerce Transactions

A web-based machine learning system designed to detect fraudulent activities in multi-participant e-commerce environments using a combination of process mining and machine learning techniques.

---

## Features

- Analyze user behavior from multiple perspectives — time, resource, and control flow  
- Predict whether a transaction is fraudulent or legitimate  
- Role-based login for Remote Users and Service Providers  
- Visualize model accuracy with bar, pie, and line charts  
- Integrated SVM-based classification with Django backend  
- Upload and process datasets from the admin interface  

---

## Tech Stack

| Layer | Technologies |
|:------|:--------------|
| **Frontend** | HTML, CSS, JavaScript |
| **Backend** | Python, Django |
| **Database** | MySQL (MySQL Workbench) |
| **Machine Learning** | SVM, Decision Tree, Logistic Regression, Naive Bayes, Random Forest |
| **Visualization** | Matplotlib |
| **Version Control** | Git, GitHub |

---

## Requirements

Install dependencies using one of the following methods.

### Option 1 — Using `requirements.txt`
```bash
pip install -r requirements.txt
```
### Option2 - Manual Installation
```bash
pip install django mysqlclient numpy pandas scikit-learn matplotlib joblib
```
## Project Setup
### 1. Clone the Repository
```bash
git clone https://github.com/VithanalaLakshminarasimhaSwamy/Multi-Perspective-Fraud-Detection-System.git
cd Multi-Perspective-Fraud-Detection-System

```
### 2. Create and Activate a Virtual Environment
```bash
python -m venv venv
venv\Scripts\activate       # Windows
source venv/bin/activate  # macOS / Linux
```
### 3. Install Dependencies
Follow the steps mentioned in the Requirements section above.
### 4. Configure the MySQL Database
Open MySQL Workbench.

Create a new database named multi_db.

Update the database settings in a_multiperspective_fraud_detection/settings.py:
```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'multi_db',
        'USER': 'root',
        'PASSWORD': 'root',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}
```
### 5.Apply Migrations
```bash
python manage.py makemigrations
python manage.py migrate
```
### 6. Run the Development Server
```bash
python manage.py runserver
```
### 7. Access the Application
Open your browser and visit:
http://127.0.0.1:8000/

## Future Enhancements
Integration of deep learning models (LSTM / ANN)

Real-time transaction monitoring

Hybrid anomaly detection for improved accuracy
## Author

Gugulothu Jagan 
Email: 228r1a6686@gmail.com  
GitHub: [https://github.com/GugulothuJagan](https://github.com/GugulothuJagan)


## License
This project is intended for academic and educational purposes only.
Not for commercial use.

